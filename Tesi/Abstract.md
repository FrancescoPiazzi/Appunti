Distributed systems that are able to provide a service while one or more of its nodes aren't available are a must for every project that cannot afford to interrupt its service. On top of this, data consistency is also an equally important feature of these systems. 

The Raft consensus algorithm (cite here) provides a solution to both of these problems that is easier to understand and implement compared to previously existing algorithms like Paxos (cite here), other than being able to provide a consensus on a list of commands, instead of a single value, like in Paxos.

This paper presents the development and testing of an implementation of the Raft consensus algorithm (from now on referred to as Raft) using the Rust programming language, and an actor oriented framework called Actum.

After the development, the following section will present how the testing of the algorithm was implemented, both from a more abstract level, where formal specifications were translated into tests, to a lower level, where problems about implementing tests using Actum and possible solutions are discussed.

At the end, some future work that the author considered important for the completion of the project is listed, along with some ideas on how to implement it.
