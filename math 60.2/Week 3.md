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