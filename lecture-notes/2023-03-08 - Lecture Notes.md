## 3.4 - The Chain Rule
---

Example:
- $k(x)=3\cos^2(sin(x))$
	- $3[\cos(\sin(x))]^2$
	- $k'(x)=6[\cos(\sin(x))]\cdot(-\sin(\sin(x)))\cdot(\cos(x))$
	- $=-6[\cos(\sin(x))]\cdot(\sin(\sin(x)))\cdot\cos(x)$

#exam 
- Example
	- Suppose $y=f(x)$ is a curve that always lies above the x-axis and never has a horizontal tangent, wher $f$ is differentiable everywhere. For what value of $y$ is the rate of change of $y^5$ with respect to $x$ eighty times the rate of change of $y$ with respect to $x$?
		- $f(x)>0$, $f'(x)\not=0$, $f'$ exists
		- $\dfrac{dy^5}{dx}=80\dfrac{dy}{dx}$
		- $\implies 5y^4 \dfrac{dy}{dx} = 80\dfrac{dy}{dx}$
			- Because $\dfrac{dy}{dx} \not= 0$, we can divide both sides by $\dfrac{dy}{dx}$
		- $\implies 5y^4=80$
		- $\implies y^4=16$
		- $\implies y=\pm 2$
			- Remember that our function is always positive, so...
		- $\implies y=2$
	- $\dfrac{dx^5}{dx}=5x^4\cdot\dfrac{dx}{dx}=5x^4$
	- $\dfrac{d\sin(x)}{dx}=\cos(x)\cdot\dfrac{dx}{dx}=\cos(x)$
	- $\dfrac{dy^5}{dx}=5(y)^4\cdot\dfrac{dy}{dx}= 5y^4\dfrac{dy}{dx}$
		- Since we don't know what $\dfrac{dy}{dx}$ is, we have to leave it like this.

## 3.5 - Derivatives of Exponential and Hyperbolic Functions
---

### Discovering $e$
---

>[!Note] Definition of $e$
>
>The limit
>$$\lim\limits_{k\to\infty} \bigg(1+\dfrac{1}{k}\bigg)=\lim\limits_{n\to0}(1+n)^{1/n}=e$$ is defined to be the irrational number $e$
>
>We need this to be able to take derivatives of exponential functions

### Derivative of the Exponential Function
---

In previous courses, the values of exponential functions were defined - beginning with the definition of $b^n$, where $n\in \N$ - as the product of $b$ multiplied by itself $n$ times.

Later, we defined $b^0=1, b^{-n}=\dfrac{1}{b^n}$

>[!Example] Theorem: Exponential Functions are Continuous Everywhere
>
>$B(x)=b^x$, where $b>0$ and $b\not= 1$ is continuous for all real numbers
>
>**Proof**
>Let $B(x)=b^x$ and let $a$ be arbitrary.
>- Want $\lim\limits_{x\to a}b^x=b^a$
>- $\lim\limits_{x\to a}b^x=\lim\limits_{h\to 0}b^{a+h}$
>- $=\lim\limits{h\to0}b^a\cdot b^h$
>- $=b^a \cdot \lim\limits{h\to0}b^h$
>- $=b^a \cdot b^0$
>	- The proof of $\lim\limits_{h\to 0}b^h=b^0$ is in the textbook
>- $=b^a$

>[Example] Theorem: Derivative of $e^x$
>
>$$\dfrac{d}{dx}(e^x)=e^x$$
>- $\dfrac{d}{dx}(e^x)=\lim\limits_{h\to0}\dfrac{e^{x+h}-e^x}{h}$
>	- Let $n=e^h-1$ as $h\to0$
>	- $n\to1-1=0$
>	- 
>- $=\lim\limits_{h\to0}\dfrac{e^x\cdot e^h-e^x}{h}$
>- 

![[lec-3-5-1.png]]

>[!Example] Corollary: Derivative of $b^x$
>
>$$\dfrac{d}{dx}(b^x)=b^x\ln(b)$$
>
>**Proof**
>- $\dfrac{d}{dx}b^x$
>- $=\dfrac{d}{dx}[e^{\ln(b^x)}]$
>- $=e^{\ln(b^x)}\cdot\dfrac{d}{dx}\ln(b^x)$
>- $=e^{\ln(b^x)}\cdot\dfrac{d}{dx}[x\ln(b)]$
>- $=e^{\ln(b^x)}\cdot\ln(b)$
>- $=b^x\ln(b)$


Examples:
- Find the derivative of $f(x)=2^{\sec(\pi x)}$ #exam 
	- $2^{\sec(\pi x)}$
	- $f'(x)=2^{\sec(\pi x)}\cdot \ln(2) \cdot \sec(\pi x)\tan(\pi x)\cdot \pi$
- Suppose that $f$ is differentiable on $\R$. Let $F(x)=f(e^x)$ and $G(x)=e^{f(x)}$. Find expressions for $F'(x), G'(x)$
	- $F'(x)=f'(e^x)\cdot e^x$
	- $G'(x)=e^{f(x)}\cdot f'(x)$
- Show that the function $y=Ae^{-x}+Bxe^{-x}$ satisfies the differential equation $y''+2y'+y=0$
- $y'=-Ae^{-x}+B(1e^{-x}+xe^{-x})$
	- $=-Ae^{-x}+Be^{-x}-Bxe^{-x}$
	- $=e^{-x}(-A+B-Bx)$
- $y''=-e^{-x}(-A+B-Bx)+e^{-x}(-B)$
	- $=e^{-x}(A-B+Bx-B)$
	- $=e^{-x}(A-2B+Bx)$
- $-e^{-x}(A-2B+Bx)+e^{-x}(-2A+2B-2Bx)+Ae^{-x}+Bxe^{-x}$

![[lec-3-5-2.png]]


### Derivatives of the Hyperbolic Function
---

![[lec-3-5-3.png]]
![[lec-3-5-4.png]]
For the normal trig functions, whenever we take the derivative of the "co", it's negative. 