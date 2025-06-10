## Notations
In finding the partial derivative with respect to $x$, we use the following notation
$$
f_X, \quad \frac{\partial f}{\partial x}, \quad D_xf, \quad f_1
$$

In finding the partial derivative with respect to $y$, we use the following notation
$$
f_X, \quad \frac{\partial f}{\partial x}, \quad D_xf, \quad f_1
$$
---
## Limit Definition
#### Partial Derivative of $f$ with respect to $x$.

$$
f_x(x,y)=\lim_{h\to 0} \frac{f(x+h,y)-f(x,y)}{h}
$$
#### Partial Derivative of $f$ with respect to $y$.
$$
f_x(x,y)=\lim_{h\to 0} \frac{f(x+h,y)-f(x,y)}{h}
$$
---
## Clairaut's Theorem
If the functions $f_{xy} \text{ and } f_{yx}$ are both continuous on the disk, then $f_{xy}(a,b) = f_{yx}(a,b)$

---
## General Chain Rules
$$
\frac{\partial u}{\partial t_i}= \frac{\partial u}{\partial x_1}\frac{\partial x_1}{\partial t_i}+\frac{\partial u}{\partial x_2}\frac{\partial x_2}{\partial t_i}+...+\frac{\partial u}{\partial x_n}\frac{\partial x_n}{\partial t_i}
$$