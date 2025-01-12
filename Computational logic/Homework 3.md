
# Problem1
Find an application of modal logic in computer science or artificial intelligence and describe it in 150 to 300 words on the Moodle discussion forum. \\ (same as the one published on Moodle)\\ \\
Modal logic, with its set of possible worlds and a relation that describes connections between worlds, is an effective tool for representing program states. Each node can represent a state, and arcs between nodes represent state transitions, analogous to the state transitions in a program. The labeling function $L:W\xrightarrow{}P(Atoms)$ encodes the invariants of each state, offering a precise and expressive representation of the program's behavior. \\
The increase in expressiveness granted by modal logic can be used in program verification for more complicated programs, such as concurrent systems, where the state of the system is represented by the model in which we are currently in, which is described by the states of each component. \\
For example, in a world where a client makes requests to a server that are then answered, the states of the client and the server can be: \\
$C = \{C1 (\text{reading request}), C2 (\text{awaiting response}) \}$  \\
$S = \{S1 (\text{idle}), S2 (\text{processing response}) \}$  \\
For simplicity we assume that exchanging messages is instant and therefore not a state in which we can be at any time. \\
Thanks to the labelling function, we can describe rules for different states of the program: for instance, in the state (C1, S1), we can have an associated formula in FO logic $p:=\forall r \neg \text{ANSWER(r)}$, which translates to “each request r is yet to be answered”, we can also use the new operators box and diamond to reason about neighbouring models, i.e. the formula $\Box \neg (C2, S1)$ means that the state where the client is waiting for a response but the server is idle can never be reached.
This application illustrates modal logic's power in specifying and verifying properties of concurrent systems, ensuring correctness and preventing undesirable states.


# Problem 2
Let $F = (W, R)$ be a modal frame. Prove that $R$ is symmetric if and only if $\varphi\implies\Box\diamond\varphi$ \\ \\
The proof is divided into two parts: $R$ is symmetric $\xrightarrow{} (\varphi\implies\Box\diamond\varphi)$, and $(\varphi\implies\Box\diamond\varphi)$. $\xrightarrow{}$ $R$ is symmetric
Assume $R$ symmetric. If the world $w$ we are in has no neighbours, all the statements starting with $\Box$ are vacuously true, including $\Box\diamond\varphi$. 
If the world $w$ has at least one neighbour, because $R$ is symmetric, each neighbour of $w$ $w_i$ will have $w$ as its neighbour. If $\varphi$ holds in $w$, then $\diamond\varphi$ must hold in each neighbor $w_i$. This is the case, since thanks to the symmetric property, each world $w_i$ has $w$ as his neighbour, where $\varphi$ is true. \\
We now prove the opposite direction, assume for contradiction that $R$ isn't symmetric, let's create the following non symmetric model:
$M = (\{w1, w2, w3\}, \ \{(w1, w2),\ (w2, w3)\},\ (w1, \{\varphi\}))$ \\
We have that $\varphi$ holds in $w1$, but there is no neighbour of $w2$ for which $\varphi$ holds, which contradicts the hypotheses $\varphi\implies\Box\diamond\varphi$

# Problem 3
We say that frame $F = (W, R)$ is Euclidean if the relation $R$ is Euclidean $(\forall x, y, z \in W \ xRy \land xRz \xrightarrow{} yRz)$. Prove that $F$ is Euclidean iff $F \models \diamond\varphi \implies \Box\diamond\varphi$ 

We can prove this in a similar fashion to what we did in Exercise 2:

Assume a frame where R is Euclidean, and a world $w$ in which $\diamond\varphi$.
$w$ has at least one neighbor, otherwise $\diamond\varphi$ would be false, the assumption $\diamond\varphi$ states that at least one of its neighbors entails $\varphi$, let's call this neighbor $u$. We now need to show that for each world $v$ for which we have $wRv$, we also have $\diamond u$ from $v$. Since R is Euclidean, for any $v$ such that $wRv$, we also have $uRv$. Given that u⊨φ, this implies v⊨◊φ because there exists u accessible from v such that u⊨φ. Therefore, w⊨□◊φ.

This means that, ◊φ  ⟹  □◊φ holds in w, and since w was arbitrary, it holds in every world. Therefore, F⊨◊φ  ⟹  □◊φF.

