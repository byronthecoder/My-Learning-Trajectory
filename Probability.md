# A First Course in Probability
## 1. Axioms of Probability
__Definition 1.1__

​	The set of all possible outcomes of an experiment is known as the ___sample space___ of the experiment, denoted by $S$.

__Definition 1.2__

​	Any subset $E$ of the sample space is known as an ___event___.

__Definition 1.3__

​	If $E_2, E_2, ...$ are events.
​	The ___union___ of these events, denoted by $\bigcup_{n=1f}^\infty E_n$, is defined to be that event which consists of all outcomes that are in $E_n$ for at least one value of $n=1, 2, ...$.
​	The ___intersection___ of the events $E_n$, denoted by $\bigcap _{n=1}^\infty E_n$, is defined to be the event consisting of those outcomes which are in all of the events $E_n, n=1, 2, ...$.

__Definition 1.4__

​	The ___complement___ of $E$,denoted by $E^c$, consists of all outcomes in the sample space $S$ that are not in $E$.

​		 $E^c$ occurs iff $E$ does not occur.

​		 $E \bigcup E^c = S$

​		 $S^c = \emptyset$

__Theorem 1.1__	The DeMorgan's Laws
$$
(\bigcup_{i=1}^n E_i)^c = \bigcap_{i=1}^n E_i^c
$$

$$
(\bigcap_{i=1}^n E_i)^c = \bigcap^n_{i=1} E_i^c
$$

__Definition 1.5__

​	The ___probability___ of the event E is defined as
$$
P(E) = lim_{n \rightarrow \infty} \cfrac{n(E)}{n}
$$
​	For each event $E$ of the sample space $S$, we assume that a number $P(E)$ is defined and satisfies the following three axioms:

​	___Axiom 1___
$$
0 <= P(E) <= 1
$$
​	___Axiom 2___
$$
P(S) = 1
$$
​	___Axiom 3___ 

​	for any sequence of mutually exclusive events $E_1, E_2, ...$ 
$$
P(\bigcup_{i=1}^\infty E_i) = \sum_{i=1}^\infty P(E_i)
$$
__Proposition 1.1__
$$
P(E^c) = 1 - P(E)
$$
__Proposition 1.2__

​	If $E \subset F$, then $P(E) <= P(F)$.

__Proposition 1.3__
$$
P(E \bigcup F) = P(E) + P(F) - P(EF)
$$
__proposition 1.4__
$$
\begin{eqnarray}
P(E_1 \cup E_2 \cup ... \cup E_n) = &\sum_{i=1}^n& P(E_i) - \sum_{i_1<i_2} P(E_{i_1}E_{i_2}) + (-1)^{r+1} \\
&+&...+ \sum_{i_1<i_2<...<i_r}P(E_{i_1}E_{i_2}...E_{i_r}) \\
&+& ...+ (-1)^{n+1}P(E_{i_1}E_{i_2}...E_{i_n})
\end{eqnarray}
$$

## 2. Conditional Probability and Independence

__Definition 2.1__

​	The ___conditional probability___ that $E$ occurs given that $F$ has occurred is denoted by $P(E|F)$. If $P(F)>0$, then
$$
P(E|F)= \cfrac{P(EF)}{P(F)}
$$
__Theorem 2.1__	The multiplication rule
$$
P(E_1E_2E_3...E_n) = P(E_1)P(E_2|E_1)P(E_3|E_1E_2)...P(E_n|E_1...E_{n-1})
$$
__Proposition 2.1__

​	Let $E$ and $F$ be events. We can express $E$ as 
$$
E = EF \ \cup \ EF^c
$$

. By Axiom 3 we have
$$
P(E) = P(E|F)P(F)\ +\ P(E|F^c)[1\ -\ P(F)] 
$$
__Definition 2.2__

​	The ___odds___ of an event $A$ are defined by
$$
\cfrac{P(A)}{P(A^c)} = \cfrac{P(A)}{1\ -\ P(A)}
$$
This tells how much more likely it is that the event $A$ occurs than it is that does not occur. If the odds are equal to $\alpha$, then it is common to say that the odds are "$\alpha$ to 1" in favor of the hypothesis.

​	The new odds after the evidence $E$ are
$$
\cfrac{P(H|E)}{P(H^c|E)} = \cfrac{P(H)}{P(H^c)} \cfrac{P(E|H)}{P(E|H^c)}
$$
__Theorem 2.2__	Bayes's formula
$$
P(F_j|E) = \cfrac{P(EF_j)}{P(E)}= \cfrac{P(E|F_j)P(F_j)}{\sum_{i=1}^n P(E|F_i)P(F_i)}
$$
Bayes's formula shows us how to use new evidence to modify existing opinions 

 - $P(F_j|E)$: the likelihood of event $F_j$ occurring given that $E$ is true.
 - $P(E|F_j)$: 

__Definition 2.3__

​	Two events $E$ and  $F$ are said to be ___independent___ if the following equation holds.
$$
P(EF) = P(E)P(F)
$$
​	Two events $E$ and  $F$ that are not independent are said to be ___dependent___.

__Proposition 2.2__

​	If $E$ and $F$ are independent, then so are $E$ and $F^c$.  

__Definition 2.4__

​	Three events $E_1, E_2, ..., E_n$ are said to be ___independent___ if, for every subset $E_{1'}, E_{2'}, ..., E_{r'}, r<=n$, of these events,
$$
\begin{eqnarray}
P(E_{1'}, E_{2'}, ..., E_{r'}) &=& P(E_{1'})P(E_{2'})...P(E_{r'}) \\
\end{eqnarray}
$$
__Proposition 2.3__

​	Conditional probabilities satisfy all of the properties of ordinary probabilities.
$$
0 <= P(E|F) <=1
$$
​	