Kalani Mertyris
6. Given that $\cosh(x)=\dfrac{e^x+e^{-x}}{2}$, write a proof that $f(x)=\cosh(x)$ is an even function.
	1. Definition of an even function: $f(x) = f(-x)$
	2. Definition of $\cosh(x)=\dfrac{e^x+e^{-x}}{2}$
	3. Plug in $-x$ into $f(x)$ and we get: $\cosh(-x)=\dfrac{e^{(-x)}+e^{-(-x)}}{2}$
	4. Substitute: $f(x)=f(-x)$
		1. $\dfrac{e^x+e^{-x}}{2}=\dfrac{e^{(-x)}+e^{-(-x)}}{2}$
		2. $\dfrac{e^x+e^{-x}}{2}=\dfrac{e^{-x}+\dfrac{1}{e^{-x}}}{2}$
		3. $\dfrac{e^x+e^{-x}}{2}=\dfrac{e^{-x}+e^x}{2}$
		4. Commutative property of addition: $\dfrac{e^x+e^{-x}}{2}=\dfrac{e^x+e^{-x}}{2}$
	5. Since $f(x)=f(-x)$, $\cosh(x)$ is an even function

Kalani Mertyris
7. Prove the identity: $\cosh(x+y)=\cosh(x)\cosh(y)+\sinh(x)\sinh(y)$
	1. Flipping the equation, taking the (now) left hand side of the equation and substituting:
		1. $\bigg(\dfrac{e^x+e^{-x}}{2}\bigg)\bigg(\dfrac{e^y+e^{-y}}{2}\bigg)+\bigg(\dfrac{e^x-e^{-x}}{2}\bigg)\bigg(\dfrac{e^y-e^{-y}}{2}\bigg) = \cosh(x+y)$
	2. Multiplying
		1. $\dfrac{e^{x+y}+e^{x-y}+e^{-x+y}+e^{-x-y}}{4}+\dfrac{e^{x+y}-e^{x-y}-e^{-x+y}+e^{-x-y}}{4}=\cosh(x+y)$
	3. Combining (same denominator)
		1. $\dfrac{e^{x+y}+e^{x-y}+e^{-x+y}+e^{-x-y}+e^{x+y}-e^{x-y}-e^{-x+y}+e^{-x-y}}{4}=\cosh(x+y)$
	4. Simplifying
		1. $\dfrac{2e^{x+y}+2e^{-x-y}}{4}=\cosh(x+y)$
	5. Factoring and simplifying
		1. $\dfrac{2(e^{x+y}+e^{-x-y})}{4}=\cosh(x+y)$
		2. $\dfrac{e^{x+y}+e^{-(x+y)}}{2}=\cosh(x+y)$
	6. Substituting $t$ to show the base form of the equation:
		1. $\cosh(t)=\dfrac{e^t+e^{-t}}{2}$

Kalani Mertyris
8. Prove the identity: $\sinh(x-y)=\sinh(x)\cosh(y)-\cosh(x)\sinh(y)$
	1. Flipping the equation, taking the (now) left hand side of the equation and substituting:
		1. $\bigg(\dfrac{e^x-e^{-x}}{2}\bigg)\bigg(\dfrac{e^y+e^{-y}}{2}\bigg)-\bigg(\dfrac{e^x+e^{-x}}{2}\bigg)\bigg(\dfrac{e^y-e^{-y}}{2}\bigg)=\sinh(x-y)$
	2. Multiplying
		1. $\dfrac{e^{x+y}+e^{x-y}-e^{-x+y}-e^{-x-y}}{4}-\dfrac{e^{x+y}-e^{x-y}+e^{-x+y}-e^{-x-y}}{4}=\sinh(x-y)$
	3. Combining (same denominator) and simplifying
		1. $\dfrac{2e^{x-y}-2e^{-x+y}}{4}=\sinh(x-y)$
	4. Factoring and simplifying
		1. $\dfrac{2(e^{x-y}-e^{-x+y})}{4}=\sinh(x-y)$
		2. $\dfrac{e^{x-y}-e^{-(x-y)}}{2}=\sinh(x-y)$
	5. Substituting to show the base form of the equation
		1. $\dfrac{e^t-e^{-t}}{2}=\sinh(t)$

