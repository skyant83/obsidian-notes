- [Day 2](#Day%202)
	- [Counting Techniques](#Counting%20Techniques)
	- [Permutation](#Permutation)
		- [Distinct Permutation](#Distinct%20Permutation)
		- [Repeating Permutation](#Repeating%20Permutation)
			- [Example](#Example)
		- [Circular Permutation](#Circular%20Permutation)
			- [Example](#Example)
	- [Combination](#Combination)
			- [Example](#Example)
	- [Probability](#Probability)
		- [Uniform Probability Model](#Uniform%20Probability%20Model)
	- [Conditional Probability](#Conditional%20Probability)
		- [Dependent Events](#Dependent%20Events)
		- [Independent Events](#Independent%20Events)
- [Day 3](#Day%203)
	- [Probability Distribution](#Probability%20Distribution)
		- [Example](#Example)
		- [~={blue}Probability Distribution Function (pdf) $p_X(k)$=~](#~=%7Bblue%7DProbability%20Distribution%20Function%20(pdf)%20$p_X(k)$=~)
		- [~={blue}Probability Distribution Table=~](#~=%7Bblue%7DProbability%20Distribution%20Table=~)
		- [Cumulative Distribution $F_X(k)$](#Cumulative%20Distribution%20$F_X(k)$)
		- [Mean or Expected Value](#Mean%20or%20Expected%20Value)
		- [Standard Deviation and Variance](#Standard%20Deviation%20and%20Variance)
	- [Binomial Distribution](#Binomial%20Distribution)
		- [Example](#Example)
		- [~={blue}Probability Distribution Function=~](#~=%7Bblue%7DProbability%20Distribution%20Function=~)
		- [Mean, Variance, Standard Deviation](#Mean,%20Variance,%20Standard%20Deviation)
		- [~={green}Excel=~](#~=%7Bgreen%7DExcel=~)
	- [Probability Distribution Continuous Variable](#Probability%20Distribution%20Continuous%20Variable)
		- [~={blue}Probability Density Function $f_X(x)$=~](#~=%7Bblue%7DProbability%20Density%20Function%20$f_X(x)$=~)
		- [~={blue}Cumulative Distribution Function $F_X(x)$=~](#~=%7Bblue%7DCumulative%20Distribution%20Function%20$F_X(x)$=~)
	- [Normal Distribution](#Normal%20Distribution)
		- [~={blue}Gaussian Curve=~](#~=%7Bblue%7DGaussian%20Curve=~)
		- [Standardization](#Standardization)
<div class="page-break" style="page-break-before: always;"></div>

## Day 2
### Counting Techniques
(The $mn$ Rule [Fundamental Counting Principle])
- First stage = $m$ & Second stage = $n$
- $mn$ ways to accomplish an experiment

(Extended $mn$ Rule)
- $k$ stages with $n_1$ ways for the first stage, $n_2$ ways for the second stage, and $n_k$ ways to for the $k^{th}$ stage
- $\prod^{k}_{x=1} n_x$

### Permutation
#### Distinct Permutation
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

#### Repeating Permutation
- Permutation of $n$ objects with $k$ types
$$
	\frac{n!}{n_1!n_2!\cdots n_k!}
$$
##### Example
>How many ways can 9 beads (3 red, 2 yellow, 4 blue) lined up

$$
	\frac{9!}{3!2!4!} = 1260
$$
#### Circular Permutation
- Permutation in a circle with one fixed object is $(n-1)!$	

##### Example
> 6 different colored beads (~={red}**r**=~ ~={blue}**b**=~ ~={yellow}**y**=~ ~={purple}**p**=~ **bl** ~={green}**g**=~) into a bracelet if ~={red}**red**=~, ~={blue}**blue**=~, ~={yellow}**yellow**=~ are together, and ~={purple}**purple**=~, **black** must not be adjacent
$$
	\begin{align}
		3!(4-1)! = 36 &\qquad \text{rby together}\\
		3!2!(3-1)! = 24 &\qquad \text{rby together and pbl together}\\
		36-24 = 12 &\qquad \text{rby together, pbl not}
	\end{align}
$$
### Combination
- Counting without arrangement
$$
	C(n,r) = \frac{n!}{r!(n-r)!}
$$
##### Example
>Possible combinations in 7 balls drawn from a set of 42 numbered balls

$$
	\begin{align}
		C(42,7) &= \binom{42}{7} \\
			   &= \frac{42!}{7!(42-7)!} \\
			   &= 26\,978\,328
	\end{align}
$$
### Probability
#### Uniform Probability Model
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
#### Dependent Events
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

#### Independent Events
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

#### Example
	Toss two fair coins and let $X$ be the number of heads observed. Find the probability distribution for $X$.

| **Simple Event** | **Coin 1** | **Coin 2** | Probability of Simple Event<br><br>$P(E_i)$ | **Number of Heads Observed**<br><br>$X$ |
| :--------------: | :--------: | :--------: | :-----------------------------------------: | :-------------------------------------: |
|      $E_1$       |     H      |     H      |                $\frac{1}{4}$                |                    2                    |
|      $E_2$       |     H      |     T      |                $\frac{1}{4}$                |                    1                    |
|      $E_3$       |     T      |     H      |                $\frac{1}{4}$                |                    1                    |
|      $E_4$       |     T      |     T      |                $\frac{1}{4}$                |                    0                    |

#### ~={blue}Probability Distribution Function (pdf) $p_X(k)$=~
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

#### Cumulative Distribution $F_X(k)$
- formula, table or graph that gives all the possible values $k$ and $F_X(k) = P(X\le k)$, the probability that $X$ is at most $k$

| $k$ | $F_X(k)$                                                     |
|:---:|:------------------------------------------------------------ |
|  0  | $p_X(0)=\frac{1}{4}$                                         |
|  1  | $p_X(0)+p_X(1)=\frac{1}{4}+\frac{1}{2}=\frac{3}{4}$          |
|  2  | $p_X(0)+p_X(1)+p_X(2)=\frac{1}{4}+\frac{1}{2}+\frac{1}{4}=1$ |

#### Mean or Expected Value
- The average value of $X$ in the population
$$
	\mu = E(X) = \sum_{\textrm{all }k} k\cdot p_X(k)
$$

#### Standard Deviation and Variance
- Standard Deviation
	- Measures the spread or variability of the random variable
$$
	\begin{align}
		\sigma &= \sqrt{E((X-\mu)^2)} \\
			   &= \sqrt{\sum_{\textrm{all }k}(k-\mu)^2\cdot p_X(k)}
	\end{align}
$$

- Variance
$$
	\begin{align}
		\sigma^2 &= E((X-\mu)^2) \\
			     &= \sum_{\textrm{all }k}(k-\mu)^2\cdot p_X(k)
	\end{align}
$$

### Binomial Distribution
- Experiment consists of $n$ identical trials
- Each trial results in one of two outcomes
- The probability of success on a single trial is equal to $p$ and remains from trial to trial. Failure, $q=1-p$
- Trials are independent
- Each trial is called a ~={blue}Bernoulli Trial=~

#### Example
	33 distinguishable biased coins --> 0.60 heads.

| Coin 1 | Coin 2 | Coin 3 | Number of Heads | Probability |
| ------ | ------ | ------ | :-------------: | :---------: |
| H      | H      | H      |        3        |   $0.216$   |
| H      | H      | T      |        2        |   $0.144$   |
| H      | T      | H      |        2        |   $0.144$   |
| H      | T      | T      |        1        |   $0.096$   |
| T      | H      | H      |        2        |   $0.144$   |
| T      | H      | T      |        1        |   $0.096$   |
| T      | T      | H      |        1        |   $0.096$   |
| T      | T      | T      |        0        |   $0.064$   |
#### ~={blue}Probability Distribution Function=~
- If $p$ is the probability of success in $n$ Bernoulli Trials, then the probability of $k$ successes:
$$
	\begin{align}
		&p_X(k) = P(X=k) = nCp\cdot p^k\cdot (1-p)^{n-k}\\\\
		&\textrm{for }k=0,1,\cdots,n \\
		&\textrm{aka. } X \sim B(n,p)
	\end{align}
$$
#### Mean, Variance, Standard Deviation
$$
	\begin{align}
		\mu &= np \\\\
		\sigma^2 &= np(1-p) \\\\
		\sigma &= \sqrt{np(1-p)} 
	\end{align}
$$

#### ~={green}Excel=~
- Probability Dist Func
```js
=BINOM.DIST(X,N,p,FALSE)
```

- Cumulative Dist Func
```js
=BINOM.DIST(X,N,p,TRUE)
```

### Probability Distribution Continuous Variable
#### ~={blue}Probability Density Function $f_X(x)$=~
- For all values $x$ of $X$
	- $f_X(x) \ge 0$
	- $\displaystyle\int^{\infty}_{-\infty} f_X(x)\;dx = 1 \quad \textnormal{(the total area under the curve)}$
- Integration is actually done over all values $x$ that $X$ can assume
$$
	\displaystyle P(a\le X\le b) = \int^{b}_{a} f_X(x)\;dx
$$
- Rule Satisfaction
	- $P(X=a)=0$
	- ${} P(X\ge a) = P(X>a) {}$
	- $P(X\le a) = P(X<a)$
	- $P(X>a) = 1-F_X(a)$
	- $\displaystyle\lim_{x\to\infty} F_X(x)=1$
	- $\displaystyle\lim_{x\to-\infty} F_X(x)=0$

#### ~={blue}Cumulative Distribution Function $F_X(x)$=~
$$
	\begin{align}
		F_X(x) &= P(X\le x) = \int^{x}_{-\infty}f_X(t)\;dt \\\\
		
		\mu &= E(X) = \int^{\infty}_{-\infty}x\cdot f_X(x)\;dx \\
		
		\sigma &= \sqrt{E((X-\mu)^2)} = \sqrt{\int^{\infty}_{-\infty}(x-\mu)^2\cdot f_X(x)\;dx} \\
		
		\sigma^2 &= \text{Var}(X) = E((X-\mu)^2) = \int^{\infty}_{-\infty}(x-\mu)^2\cdot f_X(x)\;dx
	\end{align}
$$

### Normal Distribution
```graph
bounds: [-1,.29,1,-.2]
axis: false
defaultAxes: {
	x: {
		ticks: {
			visible: false
		}
	},
	y: {
		ticks: {
			visible: false
		}
	}
}
elements: [
	{type: slider, def: [[0.12,-0.075],[0.7,-0.075],[1.4,2,50]], att: {name: "σ"}},
	{type: functiongraph, def: ["f:(1 / (2 * Math.sqrt(2 * Math.PI))) * Math.exp(-(Math.pow(x - 0, 2)*50) / (2 * Math.pow(2, 2)))"]},
	{type: segment, def: [[-0.96,0.25],[-0.96,0]], att: {firstArrow: {type: 5}, strokeColor: '#ffff'}},
	{type: segment, def: [[-0.96,0],[1,0]], att: {lastArrow: {type: 5}, strokeColor: '#ffff'}},
	{type: segment, def: [[0,"f:(1 / (2 * Math.sqrt(2 * Math.PI))) * Math.exp(-(Math.pow(0, 2)*50) / (2 * Math.pow(2, 2)))"],[0,0]]},
	{type: point, def: [0,0], att: {name: "μ"}},
	{type: segment, def: [["f:0-(e0/10)","f:(1 / (2 * Math.sqrt(2 * Math.PI))) * Math.exp(-(Math.pow(-(e0/10), 2)*50) / (2 * Math.pow(2, 2)))"],["f:0-(e0/10)",0]]},
	{type: point, def: ["f:-(e0/10)",0], att: {name: "μ-σ"}},
	{type: segment, def: [["f:(e0/10)","f:(1 / (2 * Math.sqrt(2 * Math.PI))) * Math.exp(-(Math.pow(((e0/10)), 2)*50) / (2 * Math.pow(2, 2)))"],["f:(e0/10)",0]]},
	{type: point, def: ["f:(e0/10)",0], att: {name: "μ+σ"}},
]
```
$$
	f_X(x) = \dfrac{1}{\sigma\sqrt{2\pi}}\cdot e^{\dfrac{-(x - \mu)^2}{2\sigma^2}}, \: -\infty < x < \infty
$$
- Large values of $\sigma$ reduce the height of the curve and increase the spread
- $X \sim N\;(\mu,\sigma)$

#### ~={blue}Gaussian Curve=~
$$
	\begin{gather}
		X\sim N\;(0,1)\\\\
		or\\\\
		f_X(x)=\frac{1}{\sqrt{2\pi}}e^{\dfrac{-x^2}{2}},\quad -\infty<x<\infty
	\end{gather}
$$
- ${} P(\mu - \sigma \le X \le \mu + \sigma) \approx 0.6827 {}$
- $P(\mu - 2\sigma \le X \le \mu + 2\sigma) \approx 0.9545$
- $P(\mu - 3\sigma \le X \le \mu + 3\sigma) \approx 0.9973$

#### Standardization
- Expressing a normal random variable $X\sim N\; (\mu, \sigma)$ as the number of standard deviations it lies to the left or the right of its mean
$$
	Z = \frac{X-\mu}{\sigma}\sim N\; (0,1)
$$