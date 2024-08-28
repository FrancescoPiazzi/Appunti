# Introduction
## What is a compiler
A compiler translates a program written in high level programming languages into low level machine language
## Phases of a compiler
Phases of a compiler:
+ **Front end** this part of the pipeline is dependent on the grammar of the language
	+ **Lexical analysis** given the program text, divides it into *tokens*, a token can represent a variable name, a keyword, or a number
	+ **Syntax analysis** given the tokens, arranges them into a tree that reflects the structure of the program, this is often called parsing
	+ **Type checking** given the syntax tree, determines whether the program violates certain requirements such as undeclared variables, or misuse of variable types

+ **Middle part** this part is language and architecture agnostic, generating intermediate code is also often the most complicated step
	+ **Intermediate code generation** given the now "correct" syntax tree, the program is translated into a machine independent language, during this phase most complicated optimizations are made
	
+ **Back end** this part of the pipeline is dependent on the targeted architecture
	+ **Register allocation** given the intermediate code, the variables are translated into numbers corresponding to registers in the target machine code
	+ **Machine code generation** given the intermediate code with registers instead of variable names, generates assembly for the target architecture
	+ **Assembly and linking** assembly is translated into binary for that architecture, addresses of variables, functions, etc. are determined

Assembly and linking are done by programs supplied by the machine or operating system vendor, so they will not be covered further.

Each phase, through checking and transformation, establishes stronger invariants on the things it passes on to the next: the type checker can assume absence of syntax errors, the code generation can assume absence of type errors.

## Interpreters
Another way of implementing programming languages are interpreters, interpreters are similar to compilers, but instead of generating code from the syntax tree, the tree is processed directly to evaluate expressions and execute statements, this means that an interpreter may need to process the same statement several times (i.e. code in a loop), making interpreted programs slower than compiled ones, however interpreters are simpler, easier to move to other architectures.
In addition, plain code tends to be smaller than intermediate code, which tends to be smaller than compiled code, programming languages may be implemented as combinations of these i.e. compiling only parts where efficiency is crucial, while leaving the bigger part of the program in plain (i.e. using tensorflow with python) or in intermediate language (i.e. java)
# Lexical analysis
The lexical analyzer, or lexer, will take as input as string and divide it into tokens, filtering out all the garbage useful only to stupid humans like comments, spaces, macros etc.
It is reasonable to write a lexer by hand: the idea is to skip all white spaces, comments, etc. and every time we encounter a token, determine whether it is a variable, a number, or a keyword, however these can be hard to maintain and sometimes it may not be obvious when a token ends (i.e. x=3/2/* this comment is annoying, as the beginning looks like another divisor* /;)
This calls for the use of something to translate human-readable specifications into lexers, for lexers these specifications are often written using *regular expressions*, the generated lexers are in a class of algorithms called *finite automata*
# Regular expressions
An **alphabet** is a set of characters, given an alphabet, a **regular expression** is an algebraic notation that describes a set of strings that can be composed by the alphabet.
Each regular expression has an associated set of strings it can produce, this set is called language of s and denoted as $L(s)$. Notation for regular expressions or regex is as follows:

| Regex         | Language                                            | Description                                                                                       |
| ------------- | --------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| a             | {"a"}                                               | Set containing only the letter "a"                                                                |
| $\varepsilon$ | {""}                                                | Set containing the empty string                                                                   |
| s\|t          | $L(s) \cup L(t)$                                    | Strings from languages s and t                                                                    |
| st            | ${vw \mid v \in L(s), w \in L(t)}$^[^1]             | Strings constructed by concatenating a string from the language s to a string from the language t |
| s*            | $\{````\} \cup \{vw \mid v \in L(s), w \in L(s*)\}$ | Any number of strings of the language s                                                           |
[^1]: The "|" symbol in the definition is the mathematical "such that", not the union operator for languages defined in the row above

The precedence for applying rules is in reverse order compared to the rows of the table (star is tighter than concatenation which is tighter than union)
We will be using a few shorthands for convenience:

| Full                         | Shortcut   |
| ---------------------------- | ---------- |
| a\|b\|0\|1                   | \[ab01\]   |
| 0\|1\|2\|3\|4\|5\|6\|7\|8\|9 | \[0-9\]    |
| *all the letters*            | \[a-zA-Z\] |
| ss*                          | s$^+$      |
| s\|$\varepsilon$             | s?         |
the new operators + and ? bind with the same precedence as *

For example, the expression to describe a variable in C is \[a-zA-Z_\]\[a-zA-Z_0-9\]\*. Integers can be represented as \[+-\]?\[0-9\]$^+$

# Nondeterministic finite automata
A nondeterministic finite automaton (NFA) is a machine with a finite number of states and transitions between these states, a transition between these states is usually labeled by a character in the alphabet read from the input string, but it can be also marked with $\varepsilon$, we will call these transitions *epsilon transitions*.
When parsing a string, we can used an automaton to decide whether a string is part of a set defined by a regex or not, to do this, we select a state as a starting state, in each step, we either follow an epsilon transition to another state, or read a character from the input and follow a transition labelled by that character, because this choice is not deterministic (not part of the rules of the automaton), we call these automata non deterministic, we will see later how to turn a non deterministic automaton into a deterministic one.
When all characters are read, if the automaton is in a state marked as accepting, it means that the string we just read was part of the set generated by the regular expression associated with the automaton.
As we have seen, sometimes we can choose to follow an epsilon transition or not,  this choice can impact the state reached when the string is fully read, most importantly whether the final state is accepting or not, a string is included in a language if it is possible to make a sequence of choices that makes the string lead to an accepting state.
A formal definition of a nondeterministic finite automata can be:
	*A nondeterministic finite automaton consists of a set S of states and a set of T transitions. One of the states, $s_0 \in S$, is called the starting state of the automaton and a subset $F \subseteq S$ of the states are accepting states. Each transition t connects a pair of states $s_1$ and $s_2$ and is labelled with a symbol, which is either a character c from the alphabet $\Sigma$, or the symbol $\varepsilon$, which indicates an epsilon-transition. A transition from state $s$ to state $t$ on the symbol $c$ is written as $s^c t$.*
Accepting states are also called final states.
# Regular expressions into NFA
NFA can be constructed from regex compositionally, meaning an NFA of a regular expression can be constructed from the NFAs constructed from its sub expressions, to be precise, we will build *fragments* of NFA and then compose them into bigger fragments. By itself, a fragment is not a valid NFA, as it will have two incomplete transitions, one pointing into the fragment and one pointing out of it. When an NFA fragment has been constructed with the whole regex, the incoming unlabeled state indicates the starting state, while to the end of the outgoing unlabeled transition we will add an accepting state.

# Deterministic finite automata
Deterministic finite automata, or DFA, are NFA, but in addition:
+ There are no epsilon-transitions
+ There are no two transitions coming out of a state with the same label
This means that we'll never have to make a choice between what the next state should be: the state and the input symbol are enough to determine the next state, hence the name "deterministic".
All NFAs can be converted into DFA, and deciding whether a string is part of a language generated by a DFA is much faster compared to doing the same using an NFA, this is because we never have to "make attempts" while parsing the string.
This however comes at the cost of DFAs potentially being exponentially larger than NFAs, in practice however, DFAs are only modestly larger and therefore most lexical analyzers are based on DFAs

# NFA into DFA
The conversion is done by simulating all possible NFA: when we have several choices for the next state, we form a set with all the possible next states, so we get a transition going from a set of NFA to another. 