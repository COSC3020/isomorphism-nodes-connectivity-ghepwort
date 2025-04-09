# Isomorphism

Prove that if two graphs $A$ and $B$ have the same number of nodes and are
completely connected, they must be isomorphic. I have started with the formal
definition of isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

## Answers

Given two graphs $G_1=(V_1,E_1)$ and $G_2=(V_2,E_2)$, where $|V_1=|V_2|=n$, we want to prove that $G_1$ and $G_2$ are isomorphic if they are both also complete graphs. By defanition, we say the two graphs are isomorphic if there exists a bijective function $f: V_1 \rightarrow V_2$ such that $(u,v) \in E_1 \iff (f(u),f(v)) \in E_2$.

Since both $|V_1|$ and $|V_2|$ are equal two n, we can create an explicit bijection between them. For example if we label the nodes in $V_1$ as $v_1, v_2,...,v_n$ and the nodes in $V_2$ as $w_1, w_2,...,w_n$, then we can define a bijective function $f$ by setting $f(v_i)=w_i$. This ensures that the function is bijective as every nodes in mapped to one other.

Applying the bijection $f$ to each vertex in $V_1$, we obtain a transformed set of edges $f(E_1)=\{(f(u),f(v))|(u,v) \in E_1\}$. Since $f$ is a bijection and $G_2$ is also complete, this transformed set of edges must be precisely $E_2$ thus it holds that $f(E_1)=E_2$.

Thus, since there exists a bijection between the nod sets and that preserves the edge structure, we can conclude that $G_1$ and $G_2$ are isomorphic.




## Sources

I used [this Reddit page](https://www.reddit.com/r/learnmath/comments/1bcp6eh/what_is_a_bijection_in_simple_terms/) to help me remember what bijective means.


I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.