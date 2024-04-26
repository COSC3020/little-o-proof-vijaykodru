[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/wM4-KOzy)
# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

$f(n)\in O(g(n)) \iff \exists c,n_0 >0, \forall n\ge n_0: f(n) \le c g(n)$

In little 𝑜, we have f(n) < c.g(n) for any positive constant c. This implies that f(n) grows strictly slower than g(n), as it's always strictly less than c.g(n) for any chosen c. So, if f(n) is always less than c.g(n) for any c, then it must also be less than or equal to c.g(n) for a specific c, which is the defination of big 
O. Thus, if f(n) satisfies the little o definition, it automatically satisfies the big O definition as well. Giving us that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.