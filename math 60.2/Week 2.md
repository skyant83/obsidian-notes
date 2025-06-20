## Day 2

### Counting Techniques
(The $mn$ Rule [Fundamental Counting Principle])
- First stage = $m$ & Second stage = $n$
- $mn$ ways to accomplish an experiment

(Extended $mn$ Rule)
- $k$ stages with $n_1$ ways for the first stage, $n_2$ ways for the second stage, and $n_k$ ways to for the $k^{th}$ stage
- $\prod^{k}_{x=1} n_x$

### Permutation
Arrangement of Objects

(Distinct Permutation)
- Permutation of $n$ objects is $n!$
- Permutation of $n$ objects $r$ at a time
$$
	\begin{align}
		P(n,r) &= \frac{n!}{(n-1)!} \\
			   &= nPr \\
			   &= P^n_r
	\end{align}
$$
- Note that $P(n,n) = n!$

(Repeating Permutation)
- Permutation of $n$ objects with $k$ types
$$
	\frac{n!}{n_1!n_2!\cdots n_k!}
$$

(Circular Permutation)
- Permutation in a circle with one fixed object is $(n-1)!$

### Combination
- Counting without arrangement
$$
	C(n,r) = \frac{n!}{r!(n-r)!}
$$

### Probability
(Uniform Probability Model)
$$
	\begin{align}
		P(A) &= \frac{\textrm{no. of simple events in  }A}{\textrm{no. of simple events in } S} \\
			 &= \frac{|A|}{|S|}
	\end{align}
$$
- In cases where out comes are <u>not equally likely to occur</u>:
$$
	P(A) = P(A_1) + P(A_2) + \cdots + P(A_n)
$$
- Note that:
	1. $0 \le P(A) \le 1$
	2. $P(\varnothing) = 0$
	3. $P(S) = 1$
- Union and Intersection
$$
	\begin{align}
	P(A\cup B) &= \frac{|A\cup B|}{|S|} \\ 
			   &= P(A) + P(B) \\\\

	P(A\cap B) &= \frac{|A\cap B|}{|S|}
	\end{align}
$$
- Note the **Addition Rule**
$$
	P(A\cup B) = P(A) + P(B) - P(A\cap B)
$$
- Compliment --> $P(A^C) = 1 - P(A)$

### Conditional Probability
(Dependent Events)
- An event occurring affects the probability of the following event
- Probability of $A$ given event $B$ has occurred
$$
	P(A|B) = \frac{P(A\cap B)}{P(B)}
$$
- Note the Multiplication Rule
$$
	\begin{align}
		P(A\cap B) &= P(A|B)\cdot P(B) \\
				   &= P(B|A)\cdot P(A)
	\end{align}
$$

(Independent Events)
- Probability of one does not affect the other
- Independent if
$$
	\begin{align}
	P(A|B) &= P(A) \\
	\textrm{ or } \\
	P(B|A) &= P(B) \\\\
	\textrm{ or } \\
	P(A\cap B) &= P(A)\cdot P(B)
	\end{align}
$$