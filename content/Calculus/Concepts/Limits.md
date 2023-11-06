# Description
Limits show what happens as a variable approaches a certain value. This is usually used in scenarios where the function is undefined at the value being checked for. ^63b984

# Formal Definition (Epsilon-Delta Definition)
<!---AP Calculus AB A, Unit 3, Lesson 2, Page 2--->
>Let $c$ and $L$ be real numbers. The function $f$ has limit $L$ as $x$ approaches $c$ if, given any positive number $\varepsilon$, there is a positive number $\delta$ such that $\left|f\left(x\right)-L\right|<\varepsilon$ whenever $\left|x-c\right|<\delta$ and $x \neq c$. This is just a mathematical way of saying that, as $x$ gets closer and closer to $c$ (i.e., $\delta$ gets smaller and smaller), $f\left(x\right)$ gets closer and closer to $L$ (e.g., $\varepsilon$ gets smaller and smaller). Under those conditions, the limit $\lim_{x \to c} f\left(x\right)=L$, regardless of whether $f\left(c\right)$ exists.
\- <u>AP Calculus AB A, Unit 3, Lesson 2, Page 2</u>

^9d3b21

# Tables
One way to find the limit of a function as a variable approaches a certain value is by using tables. ^056fc4

## Example
An example of finding the limit of a function using a table is the following.
What is the [[Derivative|derivative]] of $f(t)$?
$$f\left(t\right)=4.9t^2$$
$$\lim_{h \to 0} \frac{f(x+h)-f(x)}{h}$$
$$\lim_{h \to 0} \frac{(4.9(x+h)^2)-(4.9(x)^2)}{h}$$
$$\lim_{h \to 0} \frac{(4.9(x^2+2xh+h^2))-(4.9x^2)}{h}$$
$$\lim_{h \to 0} \frac{(4.9x^2+9.8xh+4.9h^2)-(4.9x^2)}{h}$$
$$\lim_{h \to 0} \frac{9.8xh+4.9h^2}{h}$$
$$\lim_{h \to 0} 9.8x+4.9h$$ ^a0b4db

| h        | 4.9h      |
| -------- | --------- |
| 1        | 4.9       |
| 0.1      | 0.49      |
| 0.01     | 0.049     |
| 0.001    | 0.0049    |
| 0.0001   | 0.00049   |
| 0.00001  | 0.000049  |
| -0.00001 | -0.000049 |
| -0.0001  | -0.00049  |
| -0.001   | -0.0049   |
| -0.01    | -0.049    |
| -0.1     | -0.49     |
| -1       | -4.9      |

As we can see, as $h$ approaches zero, $4.9h$ approaches zero. This means we can set $4.9h$ to zero.
$$\lim_{h \to 0} 9.8x+4.9h$$
$$9.8x+(0)$$
$$9.8x$$ ^b2a182

# Direct Substitution
Direct substitution is where the limit is found by directly substituting the variable into the function. While this is the easiest way to find the limit, it isn't always possible since often directly substituting the variable into the equation will cause it to be undefined.  ^f9b814

## Example of Direct Substitution
An example of finding the limit of a function via direct substitution is the following.
What is the [[Derivative|derivative]] of $f(t)$?
$$f\left(t\right)=4.9t^2$$
$$\lim_{h \to 0} \frac{f(x+h)-f(x)}{h}$$
$$\lim_{h \to 0} \frac{(4.9(x+h)^2)-(4.9(x)^2)}{h}$$
$$\lim_{h \to 0} \frac{(4.9(x^2+2xh+h^2))-(4.9x^2)}{h}$$
$$\lim_{h \to 0} \frac{(4.9x^2+9.8xh+4.9h^2)-(4.9x^2)}{h}$$
$$\lim_{h \to 0} \frac{9.8xh+4.9h^2}{h}$$
$$\lim_{h \to 0} 9.8x+4.9h$$
$$9.8x+4.9(0)$$
$$9.8x$$
$$f'(t)=9.8t$$ ^e6e02a

# Rearranging the Function for Direct Substitution
Sometimes, it is possible to re-arrange a function in a way to make direct substitution possible when it otherwise wouldn't. Take $\lim_{h \to 0} \frac{16(x+h)^2-16x^2}{h}$, for example. Directly substituting $h$ for 0 isn't possible. However, if we simplify the expression, we get $\lim_{h \to 0} {32x+16h}$. Substituting $h$ for 0 will no longer cause the expression to be undefined and thus, direct substitution is now a valid way to find the limit of the function as $h$ approaches 0. ^2a8c00

# Properties of Limits
## Sum Rule
<span style="text-align: center; display: block;">The limit of the sum of two functions is equal to the sum of the limits of those two functions.</span>
$$\lim_{x \to c}\left(f\left(x\right)+g\left(x\right)\right)=\lim_{x \to c}f\left(x\right)+\lim_{x \to c}g\left(x\right)=L+M$$

## Difference Rule
<span style="text-align: center; display: block;">The limit of the difference of two functions is equal to the difference of the limits of those two functions.}</span>
$$\lim_{x \to c}\left(f\left(x\right)-g\left(x\right)\right)=\lim_{x \to c}f\left(x\right)-\lim_{x \to c}g\left(x\right)=L-M$$

## Product Rule
<span style="text-align: center; display: block;">The limit of the product of two functions is equal to the product of the limits of those two functions.</span>
$$\lim_{x \to c}\left(f\left(x\right) \cdot g\left(x\right)\right)=\lim_{x \to c}f\left(x\right) \cdot \lim_{x \to c}g\left(x\right)=L \cdot M$$

## Constant Multiple Rule
<span style="text-align: center; display: block;">The limit of the product of a constant and a function is equal to the product of the limits of the constant and the function.</span>
$$\lim_{x \to c}\left(k \cdot f\left(x\right)\right)=\lim_{x \to c}k \cdot \lim_{x \to c}f\left(x\right)=k \cdot L$$

## Quotient Rule
<span style="text-align: center; display: block;">The limit of the quotient of two functions is equal to the quotient of the limits of those two function, assuming that the denominator of the quotient is not equal to zero.</span>
$$\lim_{x \to c}\frac{f\left(x\right)}{g\left(x\right)}=\frac{\lim\limits_{x \to c}f\left(x\right)}{\lim\limits_{x \to c}g\left(x\right)}=\frac{L}{M},M \neq 0$$

## Power Rule
<span style="text-align: center; display: block;">"The limit of a rational power of a function is that power of the limit of the function, provided the latter is a real number and $L>0$ if $s$ is even. If $r$ and $s$ are integers, $s \neq 0$, then</span>
$$\lim_{x \to c}\left(f\left(x\right)^{\frac{r}{s}}\right)=\left(\lim_{x \to c}f\left(x\right)\right)^{\frac{r}{s}}=L^{(\frac{r}{s})}, \text{provided that } L^{\frac{r}{s}} \text{ is a real number and } L > 0 \text{ if } s \text{ is even.}$$

# One- and Two-Sided Limits
## One-Sided Limit
A one-sided limit is a limit where the value being approached is approached from one side. The two types of one-sided limits are left- and right-hand limits.

### Left- and Right-Hand Limits
#### Right-Hand Limit
A right-hand limit is a limit where the value being approached is approached from the right-hand side, rather than the left-hand side.

The standard notation for the right-hand limit is the following.
$$\lim_{x \to c^{+}}f\left(x\right)$$

#### Left-Hand Limit
A left-hand limit is a limit where the value being approached is approached from the left-hand side, rather than the right-hand side.

The standard notation for the left-hand limit is the following.
$$\lim_{x \to c^{-}}f\left(x\right)$$

## Two-Sided Limit
The two-sided limit exists if, and only if, the right-hand limit is equal to the left-hand limit. This can be written as the following (where $\iff$ means "if, and only if").
$$\lim_{x \to c}f\left(x\right)=L \iff \lim_{x \to c^{+}}f\left(x\right)=L \text{ and } \lim_{x \to c^{-}}f\left(x\right)=L$$

# The Squeeze Theorem
The Squeeze Theorem is useful for finding the limits of functions where the limit might be able to be determined directly.

## Example 1
For example, in the limit $\lim_{x \to 0}\left[x^{2}\cos\left(\frac{1}{x}\right)\right]$, we can find the limit by using the squeeze theorem. We can take off the $x^{2}$ part to get $\cos\left(\frac{1}{x}\right)$. Since we know that the range of $\cos\left(\frac{1}{x}\right)$ is $-1 \leq x \leq 1$, we can write $-1 \leq \cos\left(\frac{1}{x}\right) \leq 1$. We can then multiply by $x^{2}$ to get $-x^{2} \leq x^{2}\cos\left(\frac{1}{x}\right) \leq x^{2}$. We can then directly substitute the number we are approaching, 0 into the first and third parts of the inequality to get $0 \leq x^{2}\cos\left(\frac{1}{x}\right) \leq 0$. There is only one solution for $x^{2}\cos\left(\frac{1}{x}\right)$ when written as $0 \leq x^{2}\cos\left(\frac{1}{x}\right) \leq 0$, $0$. Thus, $\lim_{x \to 0}\left[x^{2}\cos\left(\frac{1}{x}\right)\right] = 0$.

## Example 2
The [[Limits#Example 1|previous example's]] limit could have been solved by directly substituting the value without having to go through the hassle of using the squeeze theorem. This example will show a limit where that isn't possible.
$$\text{Given:} \quad \lim_{x \to -\infty}\frac{5x^{2}-\cos\left(5x\right)}{3x^{2}-2}$$
$$\text{Create an inequality:} \quad -1 \leq \cos\left(5x\right) \leq 1$$
$$\text{Multiply by } -1 \text{:} \quad 1 \geq -\cos\left(5x\right) \geq -1$$
$$\text{Rewrite the inequality so that the lower number is on the left:} \quad -1 \leq -\cos\left(5x\right) \leq 1$$
$$\text{Add } 5x^{2} \text{:} \quad 5x^{2}-1 \leq 5x^{2}-\cos\left(5x\right) \leq 5x^{2}+1$$
$$\text{Divide by } 3x^{2} - 2 \text{:} \quad \frac{5x^{2}-1}{3x^{2}-2} \leq \frac{5x^{2}-\cos\left(5x\right)}{3x^{2}-2} \leq \frac{5x^{2}+1}{3x^{2}-2}$$
$$\text{Find the limit of the inequality as } x \text{ approaches } -\infty \text{:} \quad \lim_{x \to -\infty}\frac{5x^{2}-1}{3x^{2}-2} \leq \lim_{x \to -\infty}\frac{5x^{2}-\cos\left(5x\right)}{3x^{2}-2} \leq \lim_{x \to -\infty}\frac{5x^{2}+1}{3x^{2}-2}$$
$$\text{Find the horizontal asymptote of } \frac{5x^{2} \pm 1}{3x^{2}-2} \text{ to resolve the limit:} \quad \frac{5}{3} \leq \lim_{x \to -\infty}\frac{5x^{2}-\cos\left(5x\right)}{3x^{2}-2} \leq \frac{5}{3}$$
$$\therefore \lim_{x \to -\infty}\frac{5x^{2}-\cos\left(5x\right)}{3x^{2}-2} = \frac{5}{3}$$ ^SqThEx1

# Infinite Limits
Infinite limits are limits where the value approaches either infinity or negative infinity.