## Section 2.8 - Defining the Derivative
---

Can't define derivatives until we can define limits.

- Start discussion with Tangent Lines and Secant lines
	- Anchor point $(a, f(a))$
	- Secondary point $(a+h, f(a+h))$
	- Connecting these two points gets us the secant line
	- Dragging those points closer together gets us the tangent line (as $h\to 0$)
- Difference Quotient
	- Let $f$ be a function defined on an interval $I$ containing $a$. If $x\not= a$ is in $I$ then we have our tangent or secant function $f(x)=\dfrac{f(x)-f(a)}{x-a}$ Also can use $\dfrac{f(a+h)-f(a)}{h} = \dfrac{f(a+h)-f(h)}{a+h-a}$
	- Remember - anchor point stays, the $h$ moves closer and closer to 0 which means that the other input moves closer and closer to $a$
- Tangent Line
	- The main difference between the formulas for the secant line and the tangent line is that the **tangent line has a limit**. 
		- $m_{tan}=\lim\limits_{x\to a}\dfrac{f(x)-f(a)}{x-a}$
		- See?
		- We can also use $m_{tan}=\lim\limits_{x\to a}\dfrac{f(x+h)-f(x)}{h}$
		- Can also think about it as a change in y over a change in x
- What do we need to find the equation of a line?
	- Need a point and a slope
	- Specifically we need a line **tangent** to the point
	- First start with the point that they've given us. Usually said as "as $x=\text{ something}$"
- Example
	- Find slope of the tangent line of $f(x)=x-x^3$
	- Version 1:
		- $m_{tan}=\lim\limits_{x\to a}\dfrac{f(x)-f(a)}{x-a}$ at $x=1$ <--- we know from this that our $a$ **will** equal 1, so rewriting it
		- $=\lim\limits_{x\to 1}\dfrac{f(x)-f(1)}{x-1}$
		- $=\lim\limits_{x\to 1}\dfrac{x-x^3 - (0)}{x-1}$
		- $=\lim\limits_{x\to1}\dfrac{x(1-x^2)}{x-1}$
		- $=\lim\limits_{x\to 1}\dfrac{-x(x+1)(x-1)}{x-1}$
		- $=\lim\limits_{x\to1}-x(x+1)$
		- $=-2$ via D.S.
		- ^^ this is the slope of the tangent line, now we can use the point-slope form to find the equation of the tangent line
		- $y-y_1=m(x-x_1)$
		- $y-0=-2(x-1)$
		- $y=-2x+2$
	- Version 2:
		- $m_{tan}=\lim\limits_{h\to 0}\dfrac{f(1+h)-f(1)}{h}$ -- because in this case our $x=1$
		- $=\lim\limits_{h\to 0}\dfrac{(1+h)-(1+h)^3-0}{h}$
		- $=\lim\limits_{h\to0}\dfrac{(1+h)[1-(1+h)^2]}{h}$
		- =$\lim\limits_{h\to0}\dfrac{(1+h)(1-(1+h))(1+(1+h))}{h}$
		- $=\lim\limits_{h\to 0}\dfrac{(1+h)(-h)(2+h)}{h}$ -- this looks like factoring, but it's algebra, dropping the parenthesis
		- $=\lim\limits_{h\to0}-(1+h)(2+h)$
		- $=-2$ via direct substitution. Carry out the point-slope form above and we'll get the same equation
	- Derivative functions are denoted by $f'(a)$ also called "f-prime of a"
	- The limit **has** to exist, the derivative is a limit itself. If the function doesn't exist at that point, then there's no derivative to find because the limit at that point doesn't exist.
- Example 2
	- $f(t)=\dfrac{3t-1}{5t+3}$ find $f'(-1)$
	- $f'(-1)=\lim\limits_{h\to0}\dfrac{f(-1+h)-f(-1)}{h}$
	- $=\lim\limits_{h\to0}\dfrac{\frac{3(-1+h)-1}{5(-1+h)+3}-(-2)}{h}$
	- $=\lim\limits_{h\to0}\dfrac{\frac{3h-4}{5h-2}-2}{h}$
	- $=\lim\limits_{h\to0}\dfrac{(3h-4)-2(5h-2)}{h(5h-2)}$
	- $=\lim\limits_{h\to0}\dfrac{3h-4-10h+4}{h(5h-2)}$
	- $=\lim\limits_{h\to0}\dfrac{-7h}{h(5h-2)}$
	- $=\lim\limits_{h\to0}\dfrac{-7}{5h-2}$
	- $=\dfrac{-7}{-2}=\dfrac{7}{2}$
	- ^^ this is the slope of the tangent line at $(-1, f(-1))$
- Example 3
	- We may get questions like "What does the following limit represent?"
		- $\lim\limits_{h\to0}\dfrac{(3+h)^{-1}-3^{-1}}{h}$
		- The above function follows the form of: $\lim\limits_{h\to0}\dfrac{f(3+h)-f(3)}{h}$ which is the derivative function
		- This **looks** like a derivative where the original function would be $f(x)=\frac{1}{x}$ or $x^{-1}$ at $x=3$
		- What does the following limit represent?
			- The slope of the tangent line (because remember that the function gives us the slope of the tangent line) for the function $f(x)=x^{-1}$. That's it

## Velocities and Rates of Change
---

$s(t)$ is used throughout calculus to represent the position of a particle.

- Average velocity = change in position / change in time
	- $\dfrac{s(t)-s(a)}{t-a}$
	- This is the same as the secant line
- Instantaneous velocity = change in position / change in time at a specific point
	- $\lim\limits_{t\to a}\dfrac{s(t)-s(a)}{t-a}$
	- The instantaneous velocity at $t=a$ is the derivative of position at $t=a$
	- This is the same as the tangent line
- Example:
	- Rock is thrown upward with a velocity of 10 m/s, height in meters after $t$ seconds is given by $H=10t-1.86t^2$
	- Find instantaneous velocity of the rock at 1 second
		- $H'(1)=\lim\limits_{t\to1}\dfrac{H(t)-H(1)}{t-1}$
		- $=\lim\limits_{t\to1}\dfrac{10t-1.86t^2-8.14}{t-1}$
		- $=\lim\limits_{t\to1}\dfrac{-1.86t^2+10t-8.14}{t-1}$
			- Remainder and Factor Theorems
				- If $P(c)=0$ then $(x-c)$ must be a factor of $P$
				- By this, we know that $t-1$ is a factor
			- Synthetic Division
			- 1 | -1.86 | 10 | -8.14 |
			- 1 |          |      |          |
			- ----------------------
			-    | -1.86|8.14|0| < ------- number we get after we factor out (t-1)
		- $=\lim\limits_{t\to1}\dfrac{(t-1)(-1.86t+8.14)}{t-1}$
		- $=-1.86+8.14=6.28$
		- Velocity of the rock at 1 second = 6.28 m/s
	- Find the velocity of the rock when $t=a$
		- $H'(a)=\lim\limits_{h\to 0}\dfrac{H(a+h)-H(a)}{t-a}$
		- $=\lim\limits_{h\to 0}\dfrac{(10(a+h)-1.86(a+h)^2)-(10a-1.86a^2)}{h}$
		- $=\lim\limits_{h\to 0}\dfrac{10a+10h-1.86(a^2+2ah+h^2)-10a+1.86a^2}{h}$
		- $=\lim\limits_{h\to 0}\dfrac{10h-3.72ah-1.86h^2}{h}$
		- $=\lim\limits_{h\to 0}10-3.72a-1.86h$
		- =$10-3.72a$
	- What will the velocity and speed of the rock be when it hits the ground?
		- $H(t)=0$
		- $10t-1.86t^2=0$
		- $t(10-1.86t)=0$
		- $t=0, \dfrac{10}{1.86}$
		- $10-3.72\cdot(\frac{10}{1.86})$
		- $=10-20=-10$
		- Velocity as the rock hits the ground is -10 m/s. Rock hits the ground at $\dfrac{10}{1.86}$ seconds
		- Speed = | Velocity |, therefore the speed of the rock as it hits the ground is 10 m/s
- Example 2:
	- Given a function $B(t)$ is the cost of producing a single bitcoin $t$ years after 2011.
		- What is the meaning of the derivative $B'(t)$?
			- State what the original function **is**
				- B(t) is in dollars
				- t is in years
				- $B'(t)=\lim\limits_{h\to 0}\dfrac{B(t+h)-B(t)}{h} = \dfrac{\Delta \$}{\Delta \text{ Years}}$
				- $B'(t)$ is the change in cost for producing a single bitcoin per year
		- What are its units?
			- Change in dollars per year
			- Change in **cost to produce a bitcoin that year**
		- What does the statement $B'(8)=4758$ mean?
			- This means that in 2019, it cost $4758 dollars to produce a single bitcoin
			- The **rate of change** of the cost to produce was increasing at $4758 annually in 2019
		- Do you think the values of $B'(t)$ increased or decreased in the first year of bitcoin's release?
			- Increased
		- What do you think is the long-term behavior of $B'(t)$?
			- 