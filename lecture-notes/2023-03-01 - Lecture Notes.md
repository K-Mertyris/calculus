## Section 3.1 - Derivatives of Polynomial Functions
---

### The Power Rule
---

- Let $n$ be a positive integer. If $f(x) = x^n$, then $f'(x)=nx^{n-1}$, alternatively we may express this rule as $\dfrac{d}{dx}(x^n)=nx^{n-1}$
- Let $n\in N$ and $f(x)=x^n$
	- $f'(x)=\lim\limits_{h\to0}\dfrac{f(x+h)-f(x)}{h}$
	- $f(x+h)=(x+h)^n=(_0^n)x^n+(_1^n)x^{n-1}h+(_n^2)x^{n-2}h+...+(_{n-1}^n)x^1h^{n-1}+(_n^n)h^n$ 
	- $\implies f'(x)=\lim\limits_{h\to0}\dfrac{(_0^n)x^n+(_1^n)x^{n-1}h+(_n^2)x^{n-2}h+...+(_{n-1}^n)x^1h^{n-1}+(_n^n)h^n-x^n}{h}$
	- $\implies \lim\limits_{h\to0}\dfrac{\cancel{(_0^n)x^n}+(_1^n)x^{n-1}h+(_n^2)x^{n-2}h+...+(_{n-1}^n)x^1h^{n-1}+(_n^n)h^n-\cancel{x^n}}{h}$
	- $=\implies f'(x)=\lim\limits_{h\to0}\dfrac{(_1^n)x^{n-1}h+(_n^2)x^{n-2}h+...+(_{n-1}^n)x^1h^{n-1}+(_n^n)h^n}{h}$

![[lec-3-1-1.png]]

This means that when we look at the derivative of a function, we can do the following:
- We can take constants and make them a 0
- We can take a variable, bring down the power as a coefficient, subtract one from the power and rewrite

!Warning - We don't know how to compute the derivative of the product of functions ($\dfrac{d}{dx}f(x)\cdot g(x)$)

Find the derivative of $f(x)=x^2x^3$
- $f(x)=x^5$
- $f'(x)=5x^4$

!Warning - cannot use this trick in section 2.9. Only from 3.1 forward can we use the tricks taught in class. We haven't proved Theorem 3.1.3 (the Power Rule - for positive integer exponents only). 

We'll prove this one when we get to rational exponents, and we can use it for rational exponents.

Example: Find the derivative of each function:
- !EXAM - $g(x)=\dfrac{18x^3\sqrt[6]{x^5}-10x^2\sqrt[6]{x^5}-3(10x)^2x^{-1/6}+45x^{4/3}}{5(3x^{2/3})^2}$
	- $g(x)=\dfrac{18x^3\cdot x^{5/6}-10x^2\cdot x^{5/6}-300x^2\cdot x^{-1/6}+45x^{4/3}}{5\cdot 9x^{4/3}}$
	- $=\dfrac{18x^{23/6}-10x^{17/6}-300x^{11/12}+45x^{4/3}}{45x^{4/3}}$
	- $=\dfrac{2}{5}x^{15}{6}-\dfrac{2}{9}$ -- Finish writing this out
	- In calculus, leave rational exponents alone

![[lec-3-1-2.png]]

Example:
- $h(x)=x^{1/\pi}$
	- $h'(x)=\dfrac{1}{\pi}x^{1/\pi - 1}$
- $k(x)=\pi^e$
	- Since the base is a **constant** and not a variable, this means that the derivative is 0 because the derivative of a constant is 0
	- !TEST

The Power Rule only applies to algebraic functions of the form $y=x^n$.

Let $g(x)=\dfrac{18x^3\sqrt[6]{x^5}-10x^2\sqrt[6]{x^5}-3(10x)^2x^{-1/6}+45x^{4/3}}{5(3x^{2/3})^2}$
!TEST 
Find a point or points $a$ such that $f'(a)=0$
- From the previous example: $f'(x)=x^{3/2}-\frac{1}{3}x^{1/2}-\frac{10}{3}x^{-1/2}$
	- $=3x^{3/2}-x^{1/2}-10x^{-1/2}$
	- $=x^{-1/2}(3x^2-x-10)$
	- $=x^{-1/2}(3x+5)(x-2)$

Example:
!TEST
- Find a second-degree polynomial P such that P(2)=5, P'(2)=3, P''(2)=2
	- Let $P(x)=ax^2+bx+c$
		- $P(2)=5=ax^2+bx+c \implies c=3$
	- $P'(x)=2ax+b$
		- $P'(2)=3=4a+b \implies b=-1$
	- $P''(x)=2a$
		- $P''(2)=2=2a \implies a=1$

Example:
- The equation $y'' + y' - 2y = -2x^2+14x+8$ is called a differential equation, 
	- y''+y'-2y=-2x^2+14x+8 becomes
	- 2A+2Ax+B-2(Ax^2+Bx+C)=-2x^2+14x+8
		- Comparison of coefficients
		- -2Ax^2+(2A-2B)x+(2A+B-2C)=-2x^2+14x+8
|Term|LHS|RHS|System
|-|-|-|-|
|x^0|2A+B-2C|8|2A+B-2C=8=-2C=12 \implies
|x^1|2A-2B|14|
|x^2|-2A|-2|
^^ This is a system of equations

![[lec-3-1-3.png]]

!TEST
Find equations of both lines that are tangent to the curve $y=x^3-3x^2+3x-3$ and are parallel to the line $3x-y=15$
- Tangent lines mean that the slope of the tangent line must = 3, or $f'(x)=3$
- $y'=3x^2-6x+3$ -- When does this equal 3?
![[lec-3-1-4.png]]

Must also find the equations of the lines. To find the equation of a line, must have two things - the slope and a point.
- For both lines, the slope = 3
- The points are when $x=0, x=2$
	- One point is at $(0,-3)$
	- One point is at $(2,-1)$
- Now use point-slope form
	- $y-(-3)=3(x-0)\to y=3x-3$
	- $y-(-1)=3(x-2) \to y=3x-7$

Definition: Normal Line - the line perpendicular to the tangent line at a point $P$ is called the normal line to the curve at $P$

![[lec-3-1-5.png]]

Find the equation(s) of the normal line to the curve $y=x^3-3x^2+3x-3$ at $x=0, x=2$
- To find the equation of a line, we need a slope and a point
	- Normal line is **perpendicular** to the tangent line
	- If you have a perpendicular line, their slopes are negative reciprocals
		- If we have a tangent line with m=3, our perpendicular line will be $m=-\frac{1}{3}$

![[lec-3-1-6.png]]

Example: Where does the normal line to the parabola $y=x^2-1$ at the point $(-1,0)$ intersect the parabola a second time?
- $y=x^2-1$
- $y'=2x$
- $y'(-1)=-2$
- The normal line is **perpendicular**
	- Will be VERY helpful to find the equation of the normal line:
	- Slope = $1/2$ (negative reciprocal of the tangent line)
	- Point = (-1, 0)
	- Equation: $y-0=\frac{1}{2}(x+1)$
		- $y=\frac{1}{2}x+\frac{1}{2}$
	- ^^ This is the equation of the normal line
	- When does $\dfrac{1}{2}x+\dfrac{1}{2}=x^2-1$?
	- $x+1=2x^2-2$
	- $2x^2-x-3=0$
	- $(x+1)(2x-3)=0$
	- $x=-1, \dfrac{3}{2}$
	- We already have the -1 point, plug in $\dfrac{3}{2}$ to $x^2-1$
	- $\bigg(\dfrac{3}{2}\bigg)^2-1$
	- $\dfrac{9}{4}-\dfrac{4}{4}=\dfrac{5}{4}$
	- 