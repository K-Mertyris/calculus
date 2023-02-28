## Section 2.9
---

If we have a couple functions, $f(x)=g(x)+c$, then $f'(x)=g'(x)$
- Remember, the $+c$ in this case is just a y-shift
- If this is true, then is f(x)=(x+c) the same?
- As long as a function is off by a constant, their derivatives are the same

### Notations for the Derivative
---

- Lagrange's Notation
	- $f'(x)$ - this is the notation that most people are aware of
- Leibniz's Notation
	- $\dfrac{dy}{dx}$ -- the derivative of y with respect to x
- Euler's Notation
	- $D$ -- called a differential operator, used almost exclusively in differential equations
- Newton's Notation
	- $y$ (y-dot)
- These notations are the same as arithmetic notations, they mean the same thing / are equivalent
- Will be using Lagrange's and Leibniz's notations the most

### Graphing a Derivative
---

Three ways to tell that a function is _not_ differentiable at a point $x=a$ given the graph of $f$
1. The graph has a cusp or corner at $x=a$
2. The graph is not continuous at $x=a$
3. The graph has a vertical tangent line at $x=a$

Graph $|x+3|$ 
- Limit at $x=-3$ DNE because to the left of -3, the slope is -1. To the right of -3 the slope is +1
	- $y'(-3)$ DNE
- Functions with a cusp are functions where a quick change in the slope happens, those also don't have a derivative at that point; the derivative DNE.

Think in terms of roller coasters, if there is a kink/cusp/hard turn in the coaster, there is no derivative.

If there is a discontinuity in the function, there is no slope of the line at that discontinuity

If there is a vertical tangent line, the derivative doesn't exist because we'll be dividing by zero (slope of the tangent line = rise/run). A vertical line is some rise over a zero run.

Method for graphing the derivative:
- Given a graph of a function and asked to graph its derivative:
	- Look for where the function has horizontal tangent lines
		- Label these values or intervals
	- Place open circles where derivatives don't exist
	- If any linear "parts" exist, approximate their slopes
	- For the rest of the graph, estimate the slopes of the tangent lines
	- Use the slopes as y-values to graph f'.

Some function example:
- (-4,3) m=0 and -3 is an open circle
- (-1,0) m=0 and -1 and 0 are open circles
- (-3,-1) m=3/2
- (0, 4) m=changes over time

![[lec-2-9-1.png]]

Graph the derivative $f(x)=\ln|x|$
- Recommendation, use the same Cartesian coordinates for the derivative of the function we're going to graph

Graph the derivative of $f(x)=\sin(x)$
- Look for horizontal tangent lines - where m=0
- No open circles
- Approximate slopes, looks like slopes don't go any greater than 1, or any less than -1

![[lec-2-9-2.png]]

![[lec-2-9-3.png]]

![[lec-2-9-4.png]]

To prove that it's not differentiable at the points identified.
- we know that a function is differentiable except where
	- There are vertical tangent lines
	- There is a discontinuity
	- There is a cusp
- $f'(2)=\lim\limits_{h\to 0}\dfrac{f(2+h)-f(2)}{h}$
- $\lim\limits_{h\to0^+}\dfrac{f(2+h)-f(2)}{h}$
- $|x^2-4|=\begin{cases}x^2-4 & \text{if } x^2-4\ge0 \\ -(x^2-4) & \text{if } x^2-4<0 \end{cases}$
- ![[lec-2-9-5.png]]

![[lec-2-9-6.png]]
This implies that the limit as h goes to 0 f'(2) DNE

!Exam - will be asked to graph the derivative of a function given a graph of a function

## Derivatives and Continuity
---

Differentiability implies continuity
- Let $f(x)$ be a function and $a$ be in its domain. If $f(x)$ is differentiable at $a$, then $f$ is continuous at $a$.
- The converse of this theorem is not true - just because we have a continuous function, does not mean that it's differentiable
![[lec-2-9-7.png]]

## Higher-Order Derivatives
---

Most common derivative we'll use in this class is Legrange's notation, watch the YouTube video


Use the limit definition of the