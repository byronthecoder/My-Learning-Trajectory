# The Summary of A First Course in Probability ()
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
0 \leq P(E) \leq 1
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
​	This tells how much more likely it is that the event $A$ occurs than it is that does not occur. If the odds are equal to $\alpha$, then it is common to say that the odds are "$\alpha$ to 1" in favor of the hypothesis.

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

​	(a)	$0 \leq P(E|F) \leq 1$

​	(b)	$P(S|F) = 1$

​	(c)	If $ E_i,\  i=1, 2, ...$, are mutually exclusive events, then
$$
P(\bigcup_1^\infty E_i|F) = \sum_1^\infty P(E_i|F)
$$
## 3. Random Variables

__Definition 3.1__

​	For a discrete random variable $X$, we define the ___probability mass function___ $p(a)$ of $X$ by
$$
p(a) = P(X=a)
$$
$X$ must take on one of the value $x_i$ for $i=1, 2, ...$, and we have
$$
\begin{eqnarray}
&p&(x_i) \geq 0 \quad \quad \ \ \ for \ i=1, 2, ...\\
&p&(x)=0 \qquad \quad for \ all \ other \ values \ of \ x \\
&\sum_{i=1}^\infty& p(x_i) = 1
\end{eqnarray}
$$
__Definition 3.2__

​	If $X$ is a discrete random variable having a probability mass function $p(x)$, then the ___expectation___, or the ___expected value___, of $X$, denoted by $E[X]$, is defined by
$$
E[X] = \sum_{x:p(x)>0}xp(x)
$$
$E[X]$ is also referred to as the ___mean___ or  ___the first moment___ of $X$. The quantity $E[Xn], n \geq 1$, is called  ___the nth moment ___ of X.

__Definition 3.3__

​	We say that $I$ is an ___indicator variable___ for the event $A$ if
$$
I=\begin {cases}
1, & if\ A\ occurs \\
0, & if\ A^c\ occurs
\end {cases}
$$
, and we have $E[I] = P(A)$

__Proposition 3.1__

​	If $X$ is a discrete random variable that takes on one of the values $x_i, i \geq 1$, with respective probabilities $p(x_i)$, then, for any real-valued function $g$,
$$
E[g(X)]=\sum_i g(x_i)p(x_i)
$$
__Corollary 3.1__

​	 If $a$ and $b$ are constants, then
$$
E[aX + b] = aE[X] + b
$$
__Definition 3.4__

​	If $X$ is a random variable with mean $\mu$, then the variance of $X$, denoted by $Var(X)$,
is defined by	
$$
Var(X) = E[(X − \mu)^2]
$$
An alternative formula for $Var(X)$ is derived as follows:
$$
Var(X) = E[X^2] − (E[X])^2
$$
__Corollary 3.2__

​	for any constants $a$ and $b$
$$
Var(aX + b) = a^2Var(X)
$$
__Definition 3.5__

​	The square root of the $Var(X)$ is called the ___standard deviation___ of $X$, and we denote it by $SD(X)$. That is, 
$$
SD(X) = \sqrt{Var(X)}
$$
__Remarks__

​	Analogous to the ___means___ being the center of gravity of a distribution of mass, the ___variance___ represents, in the terminology of mechanics, the moment of inertia.

__Definition 3.6__

​	Suppose now that $n$ independent trials, each of which results in a ___success___ with probability $p$ and in a ___failure___ with probability $1 − p$, are to be performed. If $X$ represents the number of successes that occur in the $n$ trials, then $X$ is said to be a  ___binomial random variable___ with parameters $(n, p)$, and its probability mass function is given by
$$
p(i) = \left(\begin{matrix} n\\i \end{matrix} \right)
p^i(1\ -\ p)^{n-i} \qquad i=0, 1, ..., n
$$


__Definition 3.7__

​	A random variable $X$ is said to be a ___Bernoulli random variable___ if its probability mass function is given by following equations for some $p \in (0, 1)$
$$
\begin{eqnarray}
&p(0)& = P{X = 0} = 1 − p \\
&p(1)& = P{X = 1} = p
\end{eqnarray}
$$
​	A Bernoulli random variable is just a binomial random variable with parameters $(1, p)$.	







