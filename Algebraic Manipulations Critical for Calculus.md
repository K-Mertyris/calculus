>[!Learning Objectives]
>- State the Mathematical Mantra
>- Briefly review the following topics from Algebra:
>	- Nontrivial factoring techniques
>	- Understand when to distribute and when not to distribute
>	- Simplifying compound fractions
>	- Rationalizing numerators and denominators
>	- Using the piecewise definition of absolute value

## The Mathematical Mantra

> As a rule of thumb, perform mathematics in the order you learned mathematics. That is, perform Arithmetic before Algebra, Algebra before Trigonometry, and Trigonometry before Calculus.

## Nontrivial Factoring Techniques

### Sums and Differences of Cubes

>[! Theorem 1.1.1]
>Sums and Differences of Cubes
>$F^3 \pm L^3 = (F \pm L)(F^2 \mp FL + L^2)$

### Factoring the GCF Out of Expressions Involving Negative Rational Exponents

When all terms of an algebraic expression share a common factor, but the common factor has different powers in each term, factor out the _smallest-powered_ version of the shared factor.

### Knowing When to Distribute

If you have an expression that is already factored, then distributing things out is _almost_ always a bad idea.

In cases where we have to multiply the numerator and denominator of a given expression by a fraction equivalent to 1, a good rule of thumb to follow is:

>[! Rule of Thumb]
>When there is no choice but to multiply the numerator and denominator of a rational expression by either:
>
>a. A conjugate (to clear radicals)
>b. A LCD (to clear a compound fraction)
>
>Only perform distribution on the part (numerator or denominator) that caused the need for such an operation.

### Simplifying Compound Fractions

With compound fractions, the LCD of _all_ fractions in the numerator and denominator must be found. If the numerator and denominator of the compound fraction by the LCD, the compound fraction will unravel.

- Example:
	- $\dfrac{(1+x+h)^{-1} - (1+x)^{-1}}{h}$
	- $\dfrac{\dfrac{1}{1+x+h} - \dfrac{1}{1+x}}{h} \cdot \dfrac{(1+x+h)(1+x)}{(1+x+h)(1+x)}$
	- $\dfrac{\dfrac{(1+x+h)(1+x)}{1+x+h} - \dfrac{(1+x+h)(1+x)}{1+x}}{h(1+x+h)(1+x)}$
	- $\dfrac{\dfrac{\not{(1+x+h)}(1+x)}{\not{(1+x+h)}} - \dfrac{(1+x+h)\not{(1+x)}}{\not{(1+x)}}}{h(1+x+h)(1+x)}$
	- $\dfrac{(1+x)-(1+x+h)}{h(1+x+h)(1+x)}$
	- $\dfrac{1+x-1-x-h}{h(1+x+h)(1+x)}$
	- $\dfrac{-h}{h(1+x+h)(1+x)}$
	- $\dfrac{-\not h}{\not h(1+x+h)(1+x)}$
	- $\dfrac{-1}{(1+x+h)(1+x)}$

Note that the 'offending' fraction was in the numerator, we did not distribute the denominator, but kept it in its factored form.

### Rationalizing Numerators and Denominators

The same rule of thumb applies when rationalizing compound fractions to avoid division by zero or when trying to remove a variable from the denominator.

- Example:
	- $-\dfrac{\dfrac{1}{\sqrt{x}}-\dfrac{1}{\sqrt{x+h}}}{h}$
	- $-\dfrac{\bigg(\dfrac{1}{\sqrt{x}}-\dfrac{1}{\sqrt{x+h}}\bigg)}{h} \cdot \dfrac{\sqrt{x} \sqrt{x+h}}{\sqrt{x}\sqrt{x+h}}$
	- $-\dfrac{\sqrt{x+h} - \sqrt{x}}{h \sqrt{x}\sqrt{x+h}}$
	- $\dfrac{-\sqrt{x+h} + \sqrt{x}}{h\sqrt{x}\sqrt{x+h}}$
	- $\dfrac{\sqrt{x} - \sqrt{x+h}}{h\sqrt{x}\sqrt{x+h}}$
	- Remove the $h$ from the denominator
	- $\dfrac{(\sqrt{x}-\sqrt{x+h})}{h\sqrt{x}\sqrt{x+h}} \cdot \dfrac{(\sqrt{x}+\sqrt{x+h})}{(\sqrt{x}+\sqrt{x+h})}$
	- $\dfrac{x-(x+h)}{(h\sqrt{x}\sqrt{x+h})(\sqrt{x}+\sqrt{x+h})}$
	- $\dfrac{-\not h}{\not h \sqrt{x}\sqrt{x+h}(\sqrt{x}+\sqrt{x+h})}$
	- $\dfrac{-1}{\sqrt{x}\sqrt{x+h}(\sqrt{x}+\sqrt{x+h})}$

### Using the Piecewise Definition of the Absolute Value

$|a| = a$ if $a \ge 0$
$|a| = -a$ if $a < 0$

The absolute value of an expression with a variable (unknown) in it has two possible outcomes:

1. If $a$ is already non-negative, there is no need for absolute values
2. If $a$ is negative, the absolute value symbol will force it to become positive by returning the _opposite_ of $a$

Remember that absolute value is **_measuring the distance from the variable to zero_**. Distance is not 'negative', therefore we have to express the term in the 'positive' case.

- Example:
	- $\dfrac{x^2 + x + 6}{|x-2|}$
	- $\dfrac{(x+3)(x-2)}{|x-2|}$
	- We **_cannot_** cancel $(x-2)$ because we need to understand first if $|x-2|$ is positive or negative
		- In this case, we're saying that $|x-2| < 0$ so $|x-2| = -(x-2)$
		- Now substitute
	- $\dfrac{(x+3)(x-2)}{-(x-2)}$
	- $\dfrac{(x+3)}{-1}$
	- $-(x+3)$
