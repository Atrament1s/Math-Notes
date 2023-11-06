# What is a Function?
A function is an expression which relates two variables to each other. One of these variables is dependent and the other independent. Generally, the dependent variable is denoted with $y$ and the independent variable with $x$. ^663901
>"In the set of real numbers $\mathbb{R}$, the mathematical definition of a function is as follows:
>A **function** from a set *D* to a set *R* is a rule that assigns to every element in *D*, one and only one element in *R*."
>
\-AP Calculus AB A, Unit 2, Lesson 2, Page 2
>>Set *D* is the domain.
>>Set *R* is the range.
^1b9f92
# Vertical Line Test
Since a function is only allowed 1 output per input, we can use a vertical line to test if a function is a graph. If the line touches the graph at more than one point at any time, the graph is NOT a function. ^b51974

# Domain and Range
The domain of a function is the values of the independent variable. This means that the domain of a function represents every x-coordinate of that function.
The range of a function represents the values of the dependent variable. Likewise, the range of a function is the set of all y-coordinates of that function. ^edaa74

# Even and Odd Functions
A function is an even function if $f(-x) = f(x)$.
A function is an odd function if $f(-x) = -f(x)$. ^c6c70e

## Symmetry
The graph of an **even** function has y-axis symmetry.
The graph of an **odd** function has origin symmetry. ^7f21c4

### Example
$$y = \sqrt{x^2 + 2}$$
$$ \\ $$
$$f(x) = \sqrt{x^2 + 2}$$
$$f(-x) = \sqrt{(-x)^2 + 2} = \sqrt{x^2 + 2}$$
$$-f(x) = -\sqrt{x^2 + 2}$$
$$ \\ $$
$$f(-x) = f(x)$$
$$f(-x) \neq -f(x)$$
$$ \\ $$
$$\text{The given function is even.}$$ ^4386eb

# Piecewise Functions
A piecewise function is a function that is defined differently over different parts of its domain. ^19accd

## Example 1
$$
f(x) =
\begin{cases}
3 - x, & x \leq 1 \\
2x, & 1 < x
\end{cases}
$$

^fcd62a

```tikz
\usepackage{pgfplots}
\begin{document}
\begin{tikzpicture}[
  declare function={
    func(\x)= (\x <= 1) * (3 - \x) + (\x > 1) * (2 * \x);
  }
]
\begin{axis}[
  axis x line=middle, axis y line=middle,
  ymin=-5, ymax=5, ytick={-5,...,5}, ylabel=$y$,
  xmin=-5, xmax=5, xtick={-5,...,5}, xlabel=$x$,
  samples=101
]

\addplot [blue,thick] {func(x)};
\end{axis}
\end{tikzpicture} 
\end{document}
```

^cec2bf

# Absolute Value Function
The absolute value function, $f(x) = |x|$ is a [[Functions#Piecewise Functions|piecewise function]] where $f(x) = -x$ over $x < 0$ and $f(x) = x$ over $x \geq 0$. When written as a piecewise function this would be $f(x) = \begin{cases} -x, & x < 0 \\ x, & x \geq 0 \end{cases}$. ^5f6a97

# Composite Functions
A composite function (e. g. $(f \circ g)\left(\frac{2}{3}\right)$) is a function where a function is used as the input of another function.  ^44fe7e

## Example
For example, in the following composite function, $f$'s input is $g$ and $g$'s input is 5.
$$f(x) = 3x + 2$$
$$g(x) = x^2 + 4$$
$$(f \circ g)(5)$$
$$ \\ $$
$$(f \circ g)(5) = f(g(5)) = 3\left(5^2 + 4\right) + 2 = 89$$ ^1119e6

# Exponential Functions
## Exponential Growth
<!---AP Calculus AB A, Unit 2, Lesson 3, Page 2--->
<q>Exponential growth can be modeled by the function $y = k*a^x$, $k>0$ and $a>1$.</q> Where $k$ is the initial amount, $a$ is the rate of growth, and $x$ is the amount of time intervals. ^b75e4f

## Exponential Decay
<!---AP Calculus AB A, Unit 2, Lesson 3, Page 3--->
<q>Exponential decay can be modeled by the function $y = k*a^x$, $k>0$ and $0<a<1$.</q> ^390a9a

<!---AP Calculus AB A, Unit 2, Lesson 3, Page 3--->
<q>Radioactive decay can be modeled by the function $A\left(t\right)=A_0 \left(\frac{1}{2}\right)^{\frac{t}{H}}$. In this function, $A_0$ is the initial amount of substance, $H$ is the half-life, and $t$ is (time) measured in years.</q> ^2c4fc2

# One-to-One Function
A one-to-one function is a function where for every output there is only one input. This can be written as $f(x_1)\neq f(x_2)$ where $x_1\neq x_2$. This is not to be confused with every input only having one output, which is a given when talking about functions as they are a requirement to be called a function in the first place. To test whether a function has more that one input for every output the horizontal line test can be used. ^69744c

## The Horizontal Line Test
The horizontal line test is where  horizontal line is drawn across every point of a function, if the line intercepts more than 1 part of the function at a time, we know that there is more than one input for every output, making the function **not** one-to-one. ^13b335
```desmos-graph
bottom=-5; top=5;
left=-5; right=5;
---
f(x)=0.2964x^3-2x|#c74440
y=1.3|#2d70b3
(-2.175,1.3)|cross|#388c46
(-0.701,1.3)|cross|#388c46
(2.876,1.3)|cross|#388c46
(0,3.5)|hidden|label:The function is NOT one-to-one|#c74440
```

^d5bcfc

# Inverse Functions
An inverse function is a function where the x- and y-coordinates are swapped. This means that for every $(a,b)$ in the original function there is a $(b,a)$ in the inverse function. The notation for showing that a function is an inverse function is $f^{-1}(x)$. Since an inverse function is simply the reverse of a function, $f^{-1}(f(a))=a$. Note that there there might be exceptions to the properties in scenarios where the function's domain or range needs to be restricted. The reason a function or inverse function's domain or range may need to be restricted is when the original function fails the vertical line test or horizontal line test. If a function is [[Functions#One-to-One Function|one-to-one]], this is not a concern.
The process to finding the inverse of a function is to change $f(x)$ to $y$, swapping $x$ and $y$, solving for $y$, and changing $y$ to $f^{-1}(x)$. ^d0747b

# Logarithms
![[Logarithms#^70a85d]]
![[Logarithms#^417023]]

## Domain and Range
![[Logarithms#^cf893d]]
![[Logarithms#^66a117]]
![[Logarithms#^ea424c]]

## Common and Natural Logarithms
![[Logarithms#^850334]]

## Properties of Logarithms
### Inverse Property
![[Logarithms#^986198]]
![[Logarithms#^d92b1f]]

### Product Rule
![[Logarithms#^6ec43b]]

### Quotient Rule
![[Logarithms#^53b0e7]]

### Power Rule
![[Logarithms#^eabacd]]

### Change of Base
![[Logarithms#^cbe223]]

# Trigonometric Functions
## Basic Trigonometric Functions
### Sine
![[Trigonometric Functions#^2f3df6]]

### Cosine
![[Trigonometric Functions#^695efc]]

### Tangent
![[Trigonometric Functions#^982b2a]]

### Cosecant
![[Trigonometric Functions#^f85b9b]]

### Secant
![[Trigonometric Functions#^e04cb3]]

### Cotangent
![[Trigonometric Functions#^6d275f]]

## Inverse Trigonometric Functions
### Inverse Sine
![[Trigonometric Functions#^aeda2f]]

### Inverse Cosine
![[Trigonometric Functions#^5fdf40]]

### Inverse Tangent
![[Trigonometric Functions#^2a2be5]]

### Inverse Cosecant
![[Trigonometric Functions#^2e3119]]

### Inverse Secant
![[Trigonometric Functions#^a81a38]]

### Inverse Cotangent
![[Trigonometric Functions#^35f281]]

# Transformations of Functions
The general form for transforming a function is $y=af\left(b\left(x+c\right)\right)+d$, where $a$ is a vertical stretch or shrink and can reflect about the x-axis, $b$ is a horizontal stretch or shrink and can reflect about the y-axis, $c$ is the horizontal shift, $d$ is the vertical shift, and $f(x)$ is the function being transformed. ^0528ba