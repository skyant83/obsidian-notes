```insta-toc
---
title:
  name: Table of Contents
  level: 1
  center: false
exclude: ""
style:
  listType: dash
omit: []
levels:
  min: 1
  max: 6
---

# Table of Contents

- Day 2
    - Counting Techniques
    - Permutation
    - Combination
    - Probability
    - Conditional Probability
- Day 3
    - Probability Distribution
        - ~={blue}Probability Distribution **Function** (pdf)=~
        - ~={blue}Probability Distribution Table=~
    - Cumulative Distribution
    - Mean or Expected Value
    - Standard Deviation and Variance
    - Binomial Distribution
```
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
- Note the **Multiplication Rule**
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

- Mutual Independence
	- Events $A_1$$,A_2,\cdots ,A_n$ are mutually independent if each pair of events $A_i$ and $A_j$ are independent.
$$
	P(A_1 \cap A_2 \cap\cdots\cap A_n) = P(A_1)\cdot P(A_2)\cdot\,\cdots\,\cdot P(A_n)
$$

---
## Day 3
### Probability Distribution
- A formula, table, or graph that gives all the possible values $k$ of the discrete random variable $X$, and the probability $p_X(k)=P(X=k)$ associated with each value
- $p_X(k) \ge 0$
- $\displaystyle\sum_{\textrm{all }k} p_x(k)=1$

(Example)
	Toss two fair coins and let $X$ be the number of heads observed. Find the probability distribution for $X$.

| **Simple Event** | **Coin 1** | **Coin 2** | Probability of Simple Event<br>$P(E_i)$ | **Number of Heads Observed**<br>$X$ |
|:----------------:|:----------:|:----------:|:---------------------------------------:|:-----------------------------------:|
|      $E_1$       |     H      |     H      |              $\frac{1}{4}$              |                  2                  |
|      $E_2$       |     H      |     T      |              $\frac{1}{4}$              |                  1                  |
|      $E_3$       |     T      |     H      |              $\frac{1}{4}$              |                  1                  |
|      $E_4$       |     T      |     T      |              $\frac{1}{4}$              |                  0                  |

#### ~={blue}Probability Distribution **Function** (pdf)=~
$$
	p_X(k)=
	\begin{cases}
		\frac{1}{4} \textrm{ if } k=0 \\
		\frac{1}{2} \textrm{ if } k=1 \\
		\frac{1}{4} \textrm{ if } k=2
	\end{cases}
$$
#### ~={blue}Probability Distribution Table=~

| $k$ |   $p_X(k)$    |
| :-: | :-----------: |
|  0  | $\frac{1}{4}$ |
|  1  | $\frac{1}{2}$ |
|  2  | $\frac{1}{4}$ |

### Cumulative Distribution
- formula, table or graph that gives all the possible values $k$ and $F_X(k) = P(X\le k)$, the probability that $X$ is at most $k$

| $k$ | $F_X(k)$                                                     |
|:---:|:------------------------------------------------------------ |
|  0  | $p_X(0)=\frac{1}{4}$                                         |
|  1  | $p_X(0)+p_X(1)=\frac{1}{4}+\frac{1}{2}=\frac{3}{4}$          |
|  2  | $p_X(0)+p_X(1)+p_X(2)=\frac{1}{4}+\frac{1}{2}+\frac{1}{4}=1$ |

### Mean or Expected Value
- The average value of $X$ in the population
$$
	\mu = E(X) = \sum_{\textrm{all }k} k\cdot p_X(k)
$$

### Standard Deviation and Variance
(Standard Deviation)
- Measures the spread or variability of the random variable
$$
	\begin{align}
		\sigma &= \sqrt{E((X-\mu)^2)} \\
			   &= \sqrt{\sum_{\textrm{all }k}(k-\mu)^2\cdot p_X(k)}
	\end{align}
$$

(Variance)
$$
	\begin{align}
		\sigma^2 &= E((X-\mu)^2) \\
			     &= \sum_{\textrm{all }k}(k-\mu)^2\cdot p_X(k)
	\end{align}
$$

### Binomial Distribution