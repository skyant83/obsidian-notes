Find the number $b$ such that the line $y = b$ divides the region bounded by the curves $y = x^2$ and $y = 4$ into two regions with equal area

We are given the region bounded by the curves
$$
y=x^2 \text{ and } y = 4 
$$
These curves intersect when $x^2=4$, i.e.,

$$
x = -2 \quad \text{and} \quad x = 2
$$

Thus, the region is the set of all points $(x,y)$ satisfying

$$x^2 \le y \le 4 \quad \text{with} \quad -2 \le x \le 2$$

### Step 1. Compute the Total Area of the Region

The total area $A_{\text{total}}$ is given by

$$A_{\text{total}} = \int_{x=-2}^{2} \Bigl[4 - x^2\Bigr]\,dx$$

Since the integrand is even, we can write:

$$
A_{\text{total}} = 2\int_{0}^{2} (4 - x^2)\,dx.
$$

Compute the integral:

$$\int_{0}^{2} (4 - x^2)\,dx = \left[4x - \frac{x^3}{3}\right]_0^2 = \left(4(2) - \frac{2^3}{3}\right) - 0 = 8 - \frac{8}{3} = \frac{24-8}{3} = \frac{16}{3}.$$

Thus,

$$
A_{\text{total}} = 2 \cdot \frac{16}{3} = \frac{32}{3}.
$$
### Step 2. Determine the Area that Must Be Equal

We want the horizontal line $y = b$ to divide the region into two parts of equal area. Therefore, each part must have area

$$
\frac{1}{2}A_{\text{total}} = \frac{1}{2}\left(\frac{32}{3}\right) = \frac{16}{3}.
$$
### Step 3. Express the Area of the Lower Region

The lower part of the region is bounded by the parabola $y=x^2$ below and the line $y = b$ above. For a given $y$ between 0 and $b$, the horizontal cross-section of the region runs from

$$x = -\sqrt{y} \quad \text{to} \quad x = \sqrt{y},
$$
so its length is $2\sqrt{y}$.

Thus, the area $A_{\text{lower}}$ of the lower region is

$$
A_{\text{lower}} = \int_{y=0}^{b} 2\sqrt{y}\,dy.
$$
Evaluate the integral:

$$
\int 2\sqrt{y}\,dy = 2\int y^{1/2}\,dy = 2\cdot\frac{2}{3}y^{3/2} = \frac{4}{3}y^{3/2}.
$$
So,

$$
A_{\text{lower}} = \left.\frac{4}{3}y^{3/2}\right|_0^b = \frac{4}{3}b^{3/2}.
$$
### Step 4. Set Up the Equation and Solve for bb

We want the lower region's area to equal $\frac{16}{3}$:

$$
\frac{4}{3}b^{3/2} = \frac{16}{3}.
$$

Multiply both sides by 3 to eliminate the denominator:

$$4b^{3/2} = 16.$$

Divide both sides by 4:

$$b^{3/2} = 4.$$

Now, raise both sides to the power $\frac{2}{3}$ to solve for $b$:

$$b = 4^{2/3}$$

Noticing that $4 = 2^2$, we can also write:

$$b = (2^2)^{2/3} = 2^{4/3}.$$

Alternatively, since $(2^{4/3})^3 = 2^4 = 16$, we can express the answer as

$$b = \sqrt[3]{16}.$$

### Final Answer

The number $b$ such that the line $y = b$ divides the region into two regions of equal area is:

$$
\boxed{2^{4/3}} \quad \text{or equivalently} \quad \boxed{\sqrt[3]{16}}.
$$
---


Suppose $f(x) = x^{c−1}$ and $g(x) = \frac{x^c}{c}$ for some $c > 1$. Then the area under the curve $y = f(x)$ on the interval $[0, 2]$ is given by $g(0) − g(2)$.

For any continuous function $f(x)$ with an antiderivative $g(x)$, the Fundamental Theorem of Calculus tells us that

$$\int_a^b f(x)\,dx = g(b) - g(a)$$.

Here, we have

$$f(x) = x^{c-1} \quad \text{and} \quad g(x) = \frac{x^c}{c},$$

with $c > 1$.

To find the area under $f(x)$ on the interval $[0,2]$, we calculate

$$\int_0^2 x^{c-1}\,dx = g(2) - g(0).$$

Now, evaluate g at the endpoints:

$$g(2) = \frac{2^c}{c}, \quad \text{and} \quad g(0) = \frac{0^c}{c} = 0.$$

Thus, the area is

$$g(2) - g(0) = \frac{2^c}{c} - 0 = \frac{2^c}{c}.$$

The statement in the problem claims the area is $g(0) - g(2)$, but that would give

$$g(0) - g(2) = 0 - \frac{2^c}{c} = -\frac{2^c}{c},$$

which is negative and does not represent an area (since area is nonnegative).

### Conclusion

The correct expression for the area under the curve $y = f(x)$ on $[0,2]$ is

$$\boxed{\frac{2^c}{c}},$$

which comes from $g(2) - g(0)$, not $g(0) - g(2)$.

--- 

Let $f$ and $g$ be continuous functions on the interval $[0, 5]$. If $f > g$ on $[0, 3]$ and $f < g$ on $[3, 5]$, then the area bounded by the two curves on the interval $[2, 4]$ is $\int^{3}_{2}(g-f)\, dx + \int^{4}_{3}(f-g)\, dx$

**FALSE**

On any interval, the area between two curves is given by the integral of the absolute difference:

$$\text{Area} = \int |f(x) - g(x)|\,dx.$$

In this problem:

- On $[2, 3]$, since $f(x) > g(x)$, the difference $f(x) - g(x)$ is positive. Thus, the area on this interval is $\int_2^3 [f(x) - g(x)]\,dx.$
- On $[3, 4]$, since $f(x) < g(x)$, the difference $g(x) - f(x)$ is positive. Thus, the area on this interval is $\int_3^4 [g(x) - f(x)]\,dx.$

So the total area bounded by the curves on the interval $[2, 4]$ is

$$\int_2^3 [f(x) - g(x)]\,dx + \int_3^4 [g(x) - f(x)]\,dx.$$

However, the statement given in the problem is

$$\int_2^3 [g(x) - f(x)]\,dx + \int_3^4 [f(x) - g(x)]\,dx,$$

which reverses the differences on both intervals. This would result in negative values for each integral, rather than the correct positive area.

Thus, the correct expression for the area is:

$$\boxed{\int_2^3 (f(x)-g(x))\,dx + \int_3^4 (g(x)-f(x))\,dx.}$$

The expression given in the problem is incorrect because it reverses the order of the functions in the integrals.

--- 


Since $\int \frac{1}{x-5}\, dx = \ln |x − 5| + C$ for $C \in R$, it directly follows that $\int^{8}_{4}\frac{1}{x-5}\, dx=\ln 3-\ln 1=\ln 3$.

**FALSE**

The antiderivative of

$\frac{1}{x-5}$

is indeed

$\ln |x-5| + C.$

However, notice that the integrand has a vertical asymptote (a discontinuity) at $x=5$. Since the interval $[4,8]$ contains $x=5$, we must treat the integral as an improper integral.

### Why the Direct Evaluation is Problematic

If we naïvely apply the Fundamental Theorem of Calculus, we might write

$$\int_{4}^{8} \frac{1}{x-5}\,dx = \ln |8-5| - \ln |4-5| = \ln 3 - \ln 1 = \ln 3.$$

But this method ignores the fact that the integrand is not defined at x=5.

### Proper Treatment as an Improper Integral

We must split the integral at the point of discontinuity and take limits:

$$\int_{4}^{8} \frac{1}{x-5}\,dx = \lim_{a\to 5^-} \int_{4}^{a} \frac{1}{x-5}\,dx + \lim_{b\to 5^+} \int_{b}^{8} \frac{1}{x-5}\,dx.$$

1. **For x from 4 to 5:**
    
    $$\int_{4}^{a} \frac{1}{x-5}\,dx = \ln|a-5| - \ln|4-5| = \ln|a-5| - \ln 1 = \ln|a-5|.$$
    
    As $a\to 5^-$, $|a-5|\to 0$, so
    
    $$\lim_{a\to 5^-} \ln|a-5| = -\infty.$$
2. **For x from 5 to 8:**
    
    $$\int_{b}^{8} \frac{1}{x-5}\,dx = \ln|8-5| - \ln|b-5| = \ln 3 - \ln|b-5|.$$
    
    As $b\to 5^+$, $|b-5|\to 0$, so
    
    $$\lim_{b\to 5^+} \ln|b-5| = -\infty,$$
    
    and hence
    
    $$\lim_{b\to 5^+} \left(\ln 3 - \ln|b-5|\right) = \infty.$$

Since one limit goes to $-\infty$ and the other to $+\inft$y, the overall integral

$$\int_{4}^{8} \frac{1}{x-5}\,dx$$

**diverges**.

### The Cauchy Principal Value

It is worth noting that if one considers the Cauchy principal value, one defines

$$\text{p.v.} \int_{4}^{8} \frac{1}{x-5}\,dx = \lim_{\epsilon\to 0^+}\left[\int_{4}^{5-\epsilon} \frac{1}{x-5}\,dx + \int_{5+\epsilon}^{8} \frac{1}{x-5}\,dx\right].$$

In this symmetric approach,

$$\int_{4}^{5-\epsilon} \frac{1}{x-5}\,dx = \ln|5-\epsilon-5| - \ln|4-5| = \ln \epsilon - \ln 1 = \ln \epsilon,
$$
and

$$\int_{5+\epsilon}^{8} \frac{1}{x-5}\,dx = \ln|8-5| - \ln|5+\epsilon-5| = \ln 3 - \ln \epsilon.$$

Thus,

$$\text{p.v.} \int_{4}^{8} \frac{1}{x-5}\,dx = \lim_{\epsilon\to 0^+} \left(\ln \epsilon + \ln 3 - \ln \epsilon\right) = \ln 3.$$

While the principal value is $\ln 3$, **this does not mean the original improper integral converges**. The actual integrals on $[4,5)$ and $(5,8]$ diverge.

### Conclusion

The statement

$\int_{4}^{8} \frac{1}{x-5}\,dx = \ln 3$

is misleading if interpreted in the usual sense of an improper integral. The correct interpretation is that the integral diverges, even though its Cauchy principal value is $\ln 3$.

--- 

Let $f$ and $f'$ be continuous on $[a,b]$. Show that

$$
\int^{b}_{a}f(x)f'(x)\, dx=\frac{[f(b)]^2-[f(a)]^2}{2}
$$

We start by observing that the derivative of $[f(x)]^2$ is given by

$$\frac{d}{dx}[f(x)]^2 = 2f(x)f'(x)$$

Thus, we can write
$$f(x)f'(x) = \frac{1}{2}\frac{d}{dx}[f(x)]^2.$$

Now, integrate both sides from aa to bb:

$$\int_a^b f(x)f'(x)\,dx = \int_a^b \frac{1}{2}\frac{d}{dx}[f(x)]^2\,dx = \frac{1}{2}\int_a^b \frac{d}{dx}[f(x)]^2\,dx.$$

By the Fundamental Theorem of Calculus, we have:

$$\int_a^b \frac{d}{dx}[f(x)]^2\,dx = [f(b)]^2 - [f(a)]^2.
$$
Thus,

$$\int_a^b f(x)f'(x)\,dx = \frac{1}{2}\Bigl([f(b)]^2 - [f(a)]^2\Bigr).$$

This completes the proof:

$$\boxed{\int_a^b f(x)f'(x)\,dx = \frac{[f(b)]^2 - [f(a)]^2}{2}}$$
--- 

Let $f(x) = x^2 − c^2$ and $g(x) = c^2 − x^2$ . 
	(a) Sketch the region A bounded by the graphs of $f(x)$ and $g(x)$ for any $c \in R$. 
	(b) Set-up the integral representing the area of region $A$. 
	(c) Solve for value(s) of $c$ for which the area of region $A$ is $576$.

We are given the functions

$$f(x)=x^2-c^2\quad\text{and}\quad g(x)=c^2-x^2,$$

and we wish to study the region A bounded by these curves.

---

### (a) Sketching the Region

1. **Graphs of $f$ and $g$:**
    
    - The graph of$ f(x)=x^2-c^2$ is an upward opening parabola with vertex at $(0,-c^2)$.
    - The graph of $g(x)=c^2-x^2$ is a downward opening parabola with vertex at $(0,c^2)$.
2. **Intersection Points:** To find the intersections, set $f(x)=g(x)$:
    
    $$x^2-c^2 = c^2-x^2.$$
    
    Adding $x^2+c^2$ to both sides gives:
    
    $$2x^2 = 2c^2 \quad\Longrightarrow\quad x^2=c^2,$$
    
    so
    
    $$x=\pm c$$.
    
    At $x=\pm c$, we have
    
    $$f(\pm c)= (\pm c)^2-c^2 = c^2-c^2=0$$,
    
    and similarly $g(\pm c)=0$.
    
3. **The Region $A$:**
    
    - For $x$ between $-c$ and $c$ (assuming $c>0$ for clarity), note that: $f(x)=x^2-c^2\le 0\quad\text{and}\quad g(x)=c^2-x^2\ge 0$.
    - Thus, $g(x)$ lies above $f(x)$ on the interval $[-c,c]$.
    - The region $A$ is the set of points between these curves for $x$ from $-c $to$ c$.

A sketch would show two parabolas symmetric about the $y$-axis: one opening upward with its vertex below the $x$-axis and the other opening downward with its vertex above the$ x$-axis, meeting at the points $(-c,0)$ and $(c,0)$.

---

### (b) Setting Up the Integral for the Area

Since $g(x)\ge f(x)$ for $x\in[-c,c]$, the vertical distance between the curves is

$$g(x)-f(x)=\Bigl[c^2-x^2\Bigr]-\Bigl[x^2-c^2\Bigr]=2c^2-2x^2.$$

Thus, the area $A$ is given by

$$\text{Area} = \int_{-c}^{c} \Bigl(g(x)-f(x)\Bigr)\,dx = \int_{-c}^{c}\Bigl(2c^2-2x^2\Bigr)\,dx.$$

It is often convenient to factor out the constant:

$$\text{Area} = 2\int_{-c}^{c} \Bigl(c^2-x^2\Bigr)\,dx.$$

---

### (c) Solving for $c$ When the Area is $576$

1. **Evaluate the Integral:**
    
    The function $c^2-x^2$ is even, so we can use symmetry:
    
    $$\int_{-c}^{c}(c^2-x^2)\,dx = 2\int_{0}^{c}(c^2-x^2)\,dx.$$
    
    Compute the integral on $[0,c]$:
    
    $$\int_{0}^{c}(c^2-x^2)\,dx = \left[ c^2x - \frac{x^3}{3}\right]_{0}^{c} = c^2\cdot c - \frac{c^3}{3} = c^3-\frac{c^3}{3} = \frac{2c^3}{3}.
    $$
    Then,
    
    $$\int_{-c}^{c}(c^2-x^2)\,dx = 2\cdot \frac{2c^3}{3} = \frac{4c^3}{3}.$$
2. **Multiply by the Constant Factor:**
    
    Recall that
    
    $$\text{Area} = 2\int_{-c}^{c}(c^2-x^2)\,dx = 2\cdot \frac{4c^3}{3} = \frac{8c^3}{3}.$$
    
1. **Set Equal to $$576$$ and Solve:**
    
    We set
    
    $$\frac{8c^3}{3} = 576.$$
    
    Multiply both sides by $3$:
    
    $$8c^3 = 576 \cdot 3 = 1728.$$
    
    Now divide by $:
    
    $c^3 = \frac{1728}{8} = 216.$
    
    Taking the cube root:
    
    $c = \sqrt[3]{216} = 6.$
    
    **Note:** Although the functions are defined for any real $c$, the geometry of the region (with intersection points at $x=\pm c$) is most natural when $c>0$. If one were to allow $c<0$, the area would depend on $|c|$. In that case, the condition becomes $|c|=6$, so $c=6$ or $c=-6$. However, by convention we take $c=6$.
    

---

### Final Answers

- **(a)** The region A is bounded by the parabolas
    
    $$f(x)=x^2-c^2 \quad\text{(opening upward with vertex at }(0,-c^2)\text{)}$$
    
    and
    
    $$g(x)=c^2-x^2 \quad\text{(opening downward with vertex at }(0,c^2)\text{)},$$
    
    which intersect at $(x,y)=(-c,0)$ and $(c,0)$. The region is the set of points between these curves for $x\in[-c,c]$.
    
- **(b)** The area of region A is given by
    
    $$\text{Area} = \int_{-c}^{c}\Bigl[g(x)-f(x)\Bigr]dx = \int_{-c}^{c} \Bigl(2c^2-2x^2\Bigr)dx = 2\int_{-c}^{c}(c^2-x^2)\,dx.$$
- **(c)** Evaluating the integral, we found
    
    $$\text{Area} = \frac{8c^3}{3}$$
    
    Setting this equal to $576$ gives
    
$$\frac{8c^3}{3}=576 \quad\Longrightarrow\quad c^3=216 \quad\Longrightarrow\quad c=6.
$$
Thus, the value of $c$ for which the area of region $A$ is $576$ is

$$\boxed{6}$$