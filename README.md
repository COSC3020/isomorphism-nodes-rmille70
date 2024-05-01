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

 In order for two graphs to be isomorphic, they must be one to one and onto. This means that for every input there must be one unique output (one-to-one), and the set of input must map to all elements in the set of outputs (onto). 
 
 This is an example of a pigeon hole problem. Since n pigeons cannot individually fit into n-1 pigeon holes, we can also determine that v vertices in G1 cannot map uniquely to v-1 vertices in G2 (where G1 and G2 are graphs).
- So for a G1 with v vertices & a G2 with less than v vertices, the function can be onto but not one-to-one. 

Say G1 has v vertices and G2 has more than v vertices. In order to be one-to-one, all vertices in G1 must map to v unique vertices in G2. However there are more than v vertices in G2, meaning we have at least one vertex in G2 that has no corresponding vertex in G1. 
- So for a G1 with v vertices & a G2 with v+1 vertices, the function can be one-to-one but onto.

Thus unless G1 and G2 have the same number of nodes, they can either be one-to-one or onto but not both. QED