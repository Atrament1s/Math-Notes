# Objectives
- Use properties of limits to calculate limits
- Find right- and left-hand limits
- Use the Squeeze Theorem or algebraic manipulation to find a limit

# Key Words
- floor function (or greatest integer function)
- left-hand limit
- [[Limits|limit of a function]]
- right-hand limit
- Squeeze Theorem
- two-sided limit

# Definition of a Limit
## Formal Definition (Epsilon-Delta Definition)
![[Limits#^9d3b21]]

# Properties of Limits
## Sum Rule
><span style="text-align: center; display: block;">The limit of the sum of two functions is equal to the sum of the limits of those two functions.</span>
>$$\lim_{x \to c}\left(f\left(x\right)+g\left(x\right)\right)=\lim_{x \to c}f\left(x\right)+\lim_{x \to c}g\left(x\right)=L+M$$
>
>[[Limits#Sum Rule\|Link to original]]

## Difference Rule
><span style="text-align: center; display: block;">The limit of the difference of two functions is equal to the difference of the limits of those two functions.</span>
>$$\lim_{x \to c}\left(f\left(x\right)-g\left(x\right)\right)=\lim_{x \to c}f\left(x\right)-\lim_{x \to c}g\left(x\right)=L-M$$
>
>[[Limits#Difference Rule\|Link to original]]

## Product Rule
><span style="text-align: center; display: block;">The limit of the product of two functions is equal to the product of the limits of those two functions.</span>
>$$\lim_{x \to c}\left(f\left(x\right) \cdot g\left(x\right)\right)=\lim_{x \to c}f\left(x\right) \cdot \lim_{x \to c}g\left(x\right)=L \cdot M$$
>
>[[Limits#Product Rule\|Link to original]]

## Constant Multiple Rule
><span style="text-align: center; display: block;">The limit of the product of a constant and a function is equal to the product of the limits of the constant and the function.</span>
>$$\lim_{x \to c}\left(k \cdot f\left(x\right)\right)=\lim_{x \to c}k \cdot \lim_{x \to c}f\left(x\right)=k \cdot L$$
>
>[[Limits#Constant Multiple Rule\|Link to original]]

## Quotient Rule
><span style="text-align: center; display: block;">The limit of the quotient of two functions is equal to the quotient of the limits of those two function, assuming that the denominator of the quotient is not equal to zero.</span>
>$$\lim_{x \to c}\frac{f\left(x\right)}{g\left(x\right)}=\frac{\lim\limits_{x \to c}f\left(x\right)}{\lim\limits_{x \to c}g\left(x\right)}=\frac{L}{M},M \neq 0$$
>
>[[Limits#Quotient Rule\|Link to original]]

## Power Rule
><span style="text-align: center; display: block;">"The limit of a rational power of a function is that power of the limit of the function, provided the latter is a real number and $L>0$ if $s$ is even. If $r$ and $s$ are integers, $s \neq 0$, then</span>
>$$\lim_{x \to c}\left(f\left(x\right)^{\frac{r}{s}}\right)=\left(\lim_{x \to c}f\left(x\right)\right)^{\frac{r}{s}}=L^{(\frac{r}{s})}, \text{provided that } L^{\frac{r}{s}} \text{ is a real number and } L > 0 \text{ if } s \text{ is even.}$$
>
>[[Limits#Power Rule\|Link to original]]

# One- and Two-Sided Limits
## One-Sided Limit
>A one-sided limit is a limit where the value being approached is approached from one side. The two types of one-sided limits are left- and right-hand limits.
>
>[[Limits#One-Sided Limit\|Link to original]]

### Left- and Right-Hand Limits
#### Right-Hand Limit
>A right-hand limit is a limit where the value being approached is approached from the right-hand side, rather than the left-hand side.
>
>The standard notation for the right-hand limit is the following.
$$\lim_{x \to c^{+}}f\left(x\right)$$
>
>[[Limits#Right-Hand Limit\|Link to original]]

#### Left-Hand Limit
>A left-hand limit is a limit where the value being approached is approached from the left-hand side, rather than the right-hand side.
>
>The standard notation for the left-hand limit is the following.
>$$\lim_{x \to c^{-}}f\left(x\right)$$
>
>[[Limits#Left-Hand Limit\|Link to original]]

## Two-Sided Limit
>The two-sided limit exists if, and only if, the right-hand limit is equal to the left-hand limit. This can be written as the following (where $\iff$ means "if, and only if").
>$$\lim_{x \to c}f\left(x\right)=L \iff \lim_{x \to c^{+}}f\left(x\right)=L \text{ and } \lim_{x \to c^{-}}f\left(x\right)=L$$
>
>[[Limits#Two-Sided Limit\|Link to original]]

# The Squeeze Theorem
>The Squeeze Theorem is useful for finding the limits of functions where the limit might be able to be determined directly.
>
>[[Limits#The Squeeze Theorem\|Link to original]]

## Example 1
>For example, in the limit $\lim_{x \to 0}\left[x^{2}\cos\left(\frac{1}{x}\right)\right]$, we can find the limit by using the squeeze theorem. We can take off the $x^{2}$ part to get $\cos\left(\frac{1}{x}\right)$. Since we know that the range of $\cos\left(\frac{1}{x}\right)$ is $-1 \leq x \leq 1$, we can write $-1 \leq \cos\left(\frac{1}{x}\right) \leq 1$. We can then multiply by $x^{2}$ to get $-x^{2} \leq x^{2}\cos\left(\frac{1}{x}\right) \leq x^{2}$. We can then directly substitute the number we are approaching, 0 into the first and third parts of the inequality to get $0 \leq x^{2}\cos\left(\frac{1}{x}\right) \leq 0$. There is only one solution for $x^{2}\cos\left(\frac{1}{x}\right)$ when written as $0 \leq x^{2}\cos\left(\frac{1}{x}\right) \leq 0$, $0$. Thus, $\lim_{x \to 0}\left[x^{2}\cos\left(\frac{1}{x}\right)\right] = 0$.
>
>[[Limits#Example 1\|Link to original]]

## Example 2
>The [[U3L2 Using Properties of Limits#Example 1|previous example's]] limit could have been solved by directly substituting the value without having to go through the hassle of using the squeeze theorem. This example will show a limit where that isn't possible.
>$$\text{Given:} \quad \lim_{x \to -\infty}\frac{5x^{2}-\cos\left(5x\right)}{3x^{2}-2}$$
>$$\text{Create an inequality:} \quad -1 \leq \cos\left(5x\right) \leq 1$$
>$$\text{Multiply by } -1 \text{:} \quad 1 \geq -\cos\left(5x\right) \geq -1$$
>$$\text{Rewrite the inequality so that the lower number is on the left:} \quad -1 \leq -\cos\left(5x\right) \leq 1$$
>$$\text{Add } 5x^{2} \text{:} \quad 5x^{2}-1 \leq 5x^{2}-\cos\left(5x\right) \leq 5x^{2}+1$$
>$$\text{Divide by } 3x^{2} - 2 \text{:} \quad \frac{5x^{2}-1}{3x^{2}-2} \leq \frac{5x^{2}-\cos\left(5x\right)}{3x^{2}-2} \leq \frac{5x^{2}+1}{3x^{2}-2}$$
>$$\text{Find the limit of the inequality as } x \text{ approaches } -\infty \text{:} \quad \lim_{x \to -\infty}\frac{5x^{2}-1}{3x^{2}-2} \leq \lim_{x \to -\infty}\frac{5x^{2}-\cos\left(5x\right)}{3x^{2}-2} \leq \lim_{x \to -\infty}\frac{5x^{2}+1}{3x^{2}-2}$$
>$$\text{Find the horizontal asymptote of } \frac{5x^{2} \pm 1}{3x^{2}-2} \text{ to resolve the limit:} \quad \frac{5}{3} \leq \lim_{x \to -\infty}\frac{5x^{2}-\cos\left(5x\right)}{3x^{2}-2} \leq \frac{5}{3}$$
>$$\therefore \lim_{x \to -\infty}\frac{5x^{2}-\cos\left(5x\right)}{3x^{2}-2} = \frac{5}{3}$$
>
>[[Limits#Example 2\|Link to original]]