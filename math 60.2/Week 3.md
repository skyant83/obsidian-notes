- [Day 1](#Day%201)
	- [Sample Population](#Sample%20Population)
	- [Probabilistic/Random Sampling](#Probabilistic/Random%20Sampling)
		- [Simple Random Sampling](#Simple%20Random%20Sampling)
		- [Stratified Random Sampling](#Stratified%20Random%20Sampling)
		- [Cluster Sampling](#Cluster%20Sampling)
		- [1-in-k Systematic Random Sample](#1-in-k%20Systematic%20Random%20Sample)
	- [Non-Probabilistic Sampling](#Non-Probabilistic%20Sampling)
	- [Observational Study](#Observational%20Study)
	- [Potential issues](#Potential%20issues)
	- [Observed vs. Random Variable](#Observed%20vs.%20Random%20Variable)
	- [Sampling Distribution of a Statistic](#Sampling%20Distribution%20of%20a%20Statistic)
		- [Sample Mean $\overline{x}$](#Sample%20Mean%20$%5Coverline%7Bx%7D$)
			- [Example.](#Example.)
		- [Central Limit Theorem](#Central%20Limit%20Theorem)
			- [Example](#Example)
		- [Sampling Distribution of the Sample Mean](#Sampling%20Distribution%20of%20the%20Sample%20Mean)
			- [Standard Errors](#Standard%20Errors)
			- [Probabilities for the Sample Mean $\overline{X}$](#Probabilities%20for%20the%20Sample%20Mean%20$%5Coverline%7BX%7D$)
				- [Example](#Example)
## Day 1
### Sample Population
- The use of a **~={blue}subset=~** of a population to <u>represent</u> the whole population. 
- ~={blue}Sampling plans=~ or ~={blue}experimental designs=~ are the ways observations are selected from a population to be used as samples

### Probabilistic/Random Sampling
#### Simple Random Sampling
- Every sample of size $n$ has the same chance of being selected.
- A sample following these indicators is called a **~={blue}simple random sample=~**

#### Stratified Random Sampling
- Consists of two or more subpopulations (**~={blue}strata=~**)
- Involves a <u>simple random sample</u> from each of a given number of subpopulations.
- Ensures that each subpopulation is represented in the sample is called a **~={blue}stratified random sample=~**

#### Cluster Sampling
- Selecting a <u>simple random sample</u> of clusters from the available clusters of a population.
- If a clusters is selected, then **all members of that cluster will be included** in the overall sample
- Some clusters will not have representation

#### 1-in-k Systematic Random Sample
- Involves the random selection of one of the first $k$ elements in an ordered population

### Non-Probabilistic Sampling 
- Cannot be used for making statistical inferences about the populations they came from.
- **Convenience Sampling:** subjects are selected because of their convenient accessibility or proximity to the researcher/s
- **Judgement Sampling:** allows the researcher to decide who will be included in the sample based on the researchers judgement
- **Quota Sampling:** the makeup of the sample must reflect the makeup of the population based on some preselected characteristic

### Observational Study
- Often administered through a survey.
- The data already existed before the researcher's decision to observe or describe it.

### Potential issues
- **Nonresponse:** Only a portion of the carefully selected random sample responded.
- **Under Coverage:** Sample systematically excludes certain segments.
- **Wording Bias:** Questionnaire may have questions that are too complicated or confusing for the reader. May also be too sensitive in topic.

### Observed vs. Random Variable
- ~={blue}Random variable=~ is **capital**, ~={blue}Observed variable=~ is **lowercase**.
- Given a random variable $X$, the measurements of $n$ random variables $X_1,\; X_2,\;\cdots\;,\; X_n$ with the same distribution as $X$

### Sampling Distribution of a Statistic
- Probability distribution of a statistic that arises when a random sample of size $n$ are repeatedly drawn from the population
- Three ways to find the sampling distribution
	1. Derive the distribution mathematically using the laws of probability.
	2. Use a simulation to approximate the distribution. That is, draw a large number of samples of size $n$, calculating the value of the statistic for each sample.
	3. Use statistical theorems to derive exact or approximate sampling distributions

#### Sample Mean $\overline{x}$
$$
\overline{x} = \dfrac{\displaystyle\sum^{n}_{i=1}x_i}{n}
$$
##### Example.
> A population consists of $N=5$ numbers: $3,\; 6,\; 9,\; 12,\; 15$. If a random sample of size $n=3$ is selected without replacement, find the sampling distributions of the sample mean and the sample median

Sample Mean

|  Sample   | $\overline{x}$ |
| :-------: | :------------: |
|  3, 6, 9  |       6        |
| 3, 6, 12  |       7        |
| 3, 6, 15  |       8        |
| 3, 9, 12  |       8        |
| 3, 9, 15  |       9        |
| 3, 12, 15 |       10       |
| 6, 9, 12  |       9        |
| 6, 9, 15  |       10       |
| 6, 12, 15 |       11       |
| 9, 12, 15 |       12       |

Sampling distribution of the sample mean $\overline{X}$

|  k  | $p_\overline{X}(k)$ |
| :-: | :-----------------: |
|  6  |   $\frac{1}{10}$    |
|  7  |   $\frac{1}{10}$    |
|  8  |   $\frac{2}{10}$    |
|  9  |   $\frac{2}{10}$    |
| 10  |   $\frac{2}{10}$    |
| 11  |   $\frac{1}{10}$    |
| 12  |   $\frac{1}{10}$    |
Sample Median

|  Sample   | $m$ |
| :-------: | :-: |
|  3, 6, 9  |  6  |
| 3, 6, 12  |  6  |
| 3, 6, 15  |  6  |
| 3, 9, 12  |  9  |
| 3, 9, 15  |  9  |
| 3, 12, 15 | 12  |
| 6, 9, 12  |  9  |
| 6, 9, 15  |  9  |
| 6, 12, 15 | 12  |
| 9, 12, 15 | 12  |
Sampling distribution of the median

| ${} k {}$ | ${} p_M(k) {}$ |
| :-------: | :------------: |
|     6     | $\frac{3}{10}$ |
|     9     | $\frac{4}{10}$ |
|    12     | $\frac{3}{10}$ |

#### Central Limit Theorem
- If random samples of $n$ observations are drawn from a non-normal population with finite mean $\mu$ and standard deviation $\sigma$, then when $n$ is large, the sampling distribution of the sample mean is approximately normal with mean $\mu$ and standard deviation $\dfrac{\sigma}{\sqrt{n}}$. Accuracy ↑ as $n$ ↑
- If the population is normally distributed, then the sampling distribution of $\overline{X}$ is also normal regardless of the sample size.
- If the population distribution is symmetrical (non-normal), then the sampling distribution of $\overline{X}$ already becomes approximately normal for relatively small sample sizes.
- If the population distribution is skewed, the sampling distribution of $\overline{X}$ is approximately normal for sample sizes of at least 30.
##### Example
> Suppose you toss two fair dice and you record the average of the two numbers in the two upper faces. Note that there are $6(6)=36$ possible outcomes. When all the 36 possible averages are consolidated in a table, the result is the sampling distribution of $\overline{X}$


|         $k$         |       1        |      1.5       |       2        |      2.5       |       3        |      3.5       |       4        |      4.5       |       5        |      5.5       |       6        |     |     |     |     |     |     |     |     |     |     |
| :-----------------: | :------------: | :------------: | :------------: | :------------: | :------------: | :------------: | :------------: | :------------: | :------------: | :------------: | :------------: | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| $p_\overline{X}(k)$ | $\frac{1}{36}$ | $\frac{2}{36}$ | $\frac{3}{36}$ | $\frac{4}{36}$ | $\frac{5}{36}$ | $\frac{6}{36}$ | $\frac{5}{36}$ | $\frac{4}{36}$ | $\frac{3}{36}$ | $\frac{2}{36}$ | $\frac{1}{36}$ |     |     |     |     |     |     |     |     |     |     |

```graph
bounds: [-1,0.2,7,-0.03]
defaultAxes: {
	y: {
		ticks: {
			insertTicks: false,
			ticksDistance: 0.05,
		}
	}
}
elements: [
	{
		type: chart, 
		def: [
			[
				1,1.5,2,2.5,3,3.5,4,4.5,5,5.5,6
			],
			[
				0.028, 0.055, 0.083, 0.11, 0.138, 0.166, 0.138, 0.11, 0.083, 0.055, 0.028,
			],
		],
		att: {
			chartStyle: 'bar',
			width: 0.4,
			colors: [
				'#FBD79D',
				'#FBD79D',
				'#FBD79D',
				'#FBD79D',
				'#FBD79D',
				'#FBD79D',
				'#FBD79D',
				'#FBD79D',
				'#FBD79D',
				'#FBD79D',
				'#FBD79D',
			],
			opacity: 1,
			withLines: true,
			strokeColor: '#00000',
			strokeWidth:10,
			strokeOpacity: 0
		}
	}
]
```

If we try increasing the number of dice, we will see that the sampling distribution will look more and more like the normal distribution.

#### Sampling Distribution of the Sample Mean
- According to the **~={blue}CLT=~**, the sampling distribution of the sample mean is **approximately normal** for a **large sample size**
$$
\begin{gather}
	\text{Estimators:}
	\\
	\overline{X}\dot{\sim}N (\mu, \frac{\sigma}{\sqrt{n}})
\end{gather}
$$

##### Standard Errors
- The standard deviation of a statistic used as an estimator of a population is called the **~={blue}standard error (SE)=~** of the estimator because it refers to the precision of the estimator
- SE of $\overline{X}$ is $\dfrac{\sigma}{\sqrt{n}}$
##### Probabilities for the Sample Mean $\overline{X}$
- If the sampling distribution of $\overline{X}$ is normal or approximately normal
	1. Find $\mu$ and calculate the SE of $\overline{X}$, which is $\frac{\sigma}{\sqrt{n}}$
	2. Compute the desired possibility via Excel or calculator.
###### Example
> The duration of Alzheimer's disease from the onset of symptoms until death ranges from 3 to 20 years; the average is 8 years with a standard deviation of 4 years. The administrator of a large medical center randomly selects the medical records of 36 deceased Alzheimer's patients from the medical center's database and records the average duration. Find the approximate probabilities for these events:

1. The average duration is less than 7 years.
2. The average duration exceeds 7 years.
3. The average duration lies within 1.2 years of the population with mean $\mu = 8$.

Since the range is from 3 to 20 years and the average is 8, the data is concentrated on the lower values (skewed to the right). Since the sample size is 36 (>30), by the CLT, the sampling distribution of $\overline{X}$ is approximately normal. The mean and standard deviation of $\overline{X}$ are $\mu = 8$ and $\frac{\sigma}{\sqrt{n}} = \frac{4}{\sqrt{36}} = \frac{2}{3}$, respectively. Thus, $\overline{X} \dot{\sim} N\left(8, \frac{2}{3}\right)$.

1. $P(\overline{X} < 7) = \texttt{NORM.DIST(7, 8, 2/3, TRUE)} \approx 0.0668$
2. $P(\overline{X} > 7) = 1 - \texttt{NORM.DIST(7, 8, 2/3, TRUE)} \approx 0.9332$
3. $\begin{align*} P(8 - 1.2 < \overline{X} < 8 + 1.2) &= P(6.8 < \overline{X} < 9.2) \\ &= \texttt{NORM.DIST(9.2, 8, 2/3, TRUE)} - \texttt{NORM.DIST(6.8, 8, 2/3, TRUE)} \\ &\approx 0.9281 \end{align*}$

> A paper manufacturer requires a minimum strength of 20 pounds per square inch. To check the quality of the paper, a random sample of 16 pieces of paper is selected and a strength measurement is recorded for each. Assume that the strength measurements are normally distributed with standard deviation 2 pounds per square inch.
1. If the mean of the population of strength measurements is 21 pounds per square inch, what is the approximate probability that, for a random sample of 16 test pieces of paper, $\overline{X} < 20$?
2. What value would you select for the mean paper strength \mu so that $P(\overline{X} < 20) = 0.001$?

Since we are given that the measurements are normally distributed, the sample mean $\overline{X}$ is also normally distributed.

1. The mean and standard deviation of $\overline{X}$ are $\mu = 21$ and $\frac{\sigma}{\sqrt{n}} = \frac{2}{\sqrt{16}} = \frac{1}{2}$, respectively. Thus, $\overline{X} \dot{\sim} N\left(21, \frac{1}{2}\right)$.  
$$
P(\overline{X} < 20) = \texttt{NORM.DIST(20, 21, 1/2, TRUE)} \approx 0.0228
$$
2. For this item, $\mu$ is unknown, but the standard deviation is still $\frac{1}{2}$. To find $\mu$, we will have to standardize $\overline{X}$:  
$$
P(\overline{X} < 20) = P\left(\frac{\overline{X} - \mu}{\dfrac{1}{2}} < \frac{20 - \mu}{\dfrac{1}{2}}\right) = P(Z < 40 - 2\mu) = 0.001  
$$
To get the z-value with probability 0.001, we use the **NORM.S.INV** function in Excel:  

$$
40 - 2\mu = \texttt{NORM.S.INV(0.001)} \approx -3.0902 
$$

Solving for ${} \mu$ in the equation ${} 40 - 2\mu = -3.0902$ yields $\mu = 21.5451$.