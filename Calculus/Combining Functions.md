Taking the basics of functions, we can combine them using basic mathematical operations to create new functions. There are two ways to combine functions covered here - combining using mathematical operations and combining using function composition.

## Combining Functions with Mathematical Operators

To combine functions using mathematical operators, write the functions with the operator and simplify. Examples below using two functions $f$ and $g$:
1. Sum: $(f + g)(x) = f(x) + g(x)$
2. Difference: $(f-g)(x) = f(x) - g(x)$
3. Product: $(f \cdot g)(x) = f(x)g(x)$
4. Quotient: $\bigg(\dfrac{f}{g} \bigg)(x) = \dfrac{f(x)}{g(x)}$ for $g(x) \not = 0$

## Function Composition

Function composition means to take an input $x$, plug it into a function $f(x)$, then have the output of that function be the input to another function $g(x)$.
- $g(f(x))$ OR $(g \circ f)(x)$ OR $g \circ f$
- $f(x) = x^2$
- $g(x) = x^3$
- $g(f(x)) = (x^2)^3 = x^6$

>[!Definition]
>Function $f$ with domain **_A_** and range **_B_**, function $g$ with domain **_D_** and range **_E_**. If **_B_** is a subset of **_D_**, then the **composite function** $(g \circ f)(x)$ is the function with domain **_A_** such that:
>$(g \circ f)(x) = g(f(x))$
