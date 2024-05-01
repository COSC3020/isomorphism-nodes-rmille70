[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/AtNXzL3S)
# Isomorphism

Prove that if two graphs $A$ and $B$ do not have the same number of nodes, they
cannot be isomorphic. I have started with the formal definition of isomorphism
below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

## Proof:
 Let G1 and G2 be graphs.

 Say G1 has n nodes and G2 has less than n nodes. This is an example of a pigeon hole problem. Since n pigeons cannot individually fit into n-1 pigeon holes, we can also determine that n nodes in G1 cannot map uniquely to n-1 nodes in G2. 
- So for G1 with n nodes & G2 with less than n nodes, the function from G1 to G2 can be onto but not one-to-one. 

Say G1 has n nodes and G2 has more than n nodes. In order to be one-to-one, all nodes in G1 must map to n unique nodes in G2. However there are more than n nodes in G2, meaning there must be at least one node in G2 that has no corresponding node in G1. 
- So for G1 with n nodes & G2 with more than n nodes, the function from G1 to G2 can be one-to-one but onto.

In conclusion: Unless G1 and G2 have the same number of nodes, the function from G1 to G2 can either be one-to-one or onto but it cannot be one-to-one and onto. Thus because a having a one-to-one and onto function connecting two graphs is a property of isomorphic graphs, we know that two graphs with different numbers of nodes cannot be isomorphic.