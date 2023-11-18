# BBN-Bayesian-Belief-Networks
You may want to build a model where you can specify which variables are dependent, independent, or conditionally independent (this is explained in the next section). You may also want to track real-time how event probabilities change as new evidence is introduced to the model.

This is where the Bayesian Belief Networks come in handy as they allow you to construct a model with nodes and directed edges by clearly outlining the relationships between variables.

Bayesian Belief Networks (BBN) and Directed Acyclic Graphs (DAG).

Bayesian Belief Network (BBN) is a Probabilistic Graphical Model (PGM) that represents a set of variables and their conditional dependencies via a Directed Acyclic Graph (DAG).

Using the above, we can state the relationship between variables (nodes):

•	Independence: A and C are independent of each other. So are B and C. This is because knowing whether C has happened does not change our knowledge about A or B and vice versa.

•	Dependence: B is dependent on A since A is the parent of B. This relationship can be written as a conditional probability: P(B|A). D is also dependent on other variables, and in this case, it depends on two of them — B and C. Again, this can be written as a conditional probability: P(D|B,C).

•	Conditional Independence: D is considered conditionally independent of A. This is because as soon as we know whether event B has happened, A becomes irrelevant from the perspective of D. In other words, the following is true: P(D|B,A) = P(D|B).

