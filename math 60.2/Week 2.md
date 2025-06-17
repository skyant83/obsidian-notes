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
- Note that:
	1. $0 \le P(A) \le 1$
	2. $P(\varnothing) = 0$
	3. $P(S) = 1$