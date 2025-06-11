---
~
---
## Day 1
### Permutation 
(Distinct Objects)
- refers to an arrangement of these objects
- $P(n,r)$, $nPr$, $P_r^n$
- $P(n,r) = \frac{n!}{(n-r)!}$

(Repeating Objects)
- applies when all objects are not distinct
- $P(n,r) = \frac{n!}{n_1!n_2!\cdots n_k!}$

(Circular Permutation)
- arrangement in a circular manner, the number of arrangements are less
- $P(n,r) = (n-1)!$

### Combination
- used when order or arrangement is not important
- $C(n,r)$, $nCr$, $C_r^n$, $\binom{n}{r}$
- $C(n,r) = \frac{n!}{r!(n-r)!}$
---

## Day 2
### Probability 
- A simple event is the outcome observed on a single repetition of an experiment
	- Set of all simple events -> <mark class="hltr-pink">**sample space**</mark> '$S$'
- Collection of simple events -> **<mark class="hltr-pink">event</mark>**
- Two events are **mutually exclusive if one event occurs the other cannot**

(Uniform Probability Model)
- When measuring the belief the **event** $A$ will occur when each simple event is <u>equally likely to occur</u>

> Consider an experiment with a finite simple space $S$ in which each simple event is likely to occur. 
> 
> The **<mark class="hltr-yellow">probability</mark>** event $A$ is the ratio:

$$
P(A) = \frac{\textrm{no. of simple events in in } A}{\textrm{no. of simple events in } S} = \frac{|A|}{|S|}
$$

In cases where the outcomes are **<u>not equally likely to occur</u>**, we attribute $P(A)$ to be the following:

$$
P(A) = P(A_1) + P(A_2) + \cdots + P(A_n) 
$$

(Complements of Events)
- All events in the sample space <mark class="hltr-red">**except**</mark> the sample event

(Rules of Calculating Probability)
- Union
$$
	\begin{gather}
		P(A \cup B) = \frac{|A \cup B|}{|S|} 
		\\ \textrm{ or } \\
		P(A \cup B) =  P(A) + P(B) - P(A \cap B) 
	\end{gather}
$$
- Intersection
$$
	P(A \cap B) = \frac{|A \cap B|}{|S|} 
$$
- Complement