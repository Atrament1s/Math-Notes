# What are Linear and Quadratic Systems?
Linear and quadratic systems are a type of [[Systems of Equations and Inequalities|systems of equations]] where one of the equations is linear and the other in quadratic. An example of this would be the following.

$$2y=x^2+5$$
$$0=3x-2-y$$^intro-example-system

$$ \\ $$
# Solving Linear and Quadratic Systems
Linear and quadratic systems can be solved via substitution. The first step in doing so is to isolate the same variable in both equations. If we wanted to solve the [[Linear and Quadratic Systems of Equations#^intro-example-system|example system]], we can do this through the following operations.
$$2y=x^2+5$$
$$0=3x-2-y$$
$$ \\ $$
$$y=\frac{x^2+5}{2}$$
$$y=3x-2$$
$$ \\ $$
Now that we isolated the same variable in both equations, in this case, y, we can write the system as a singular equation. We can do this because both equations equal y, and thus, equal each other.
$$y=\frac{x^2}{2}$$
$$y=3x-2$$

$$3x-2=\frac{x^2}{2}$$^substituted-intro-example-system

$$ \\ $$
Now that the two equations are combined, we can solve for x. We can do this in two ways, either by factoring or using the quadratic formula.

## Solving by Using [[The Quadratic Formula]]
To use the Quadratic Formula, we first have to more everything to one side so that the other side is equal to zero.
$$3x-2=\frac{x^2}{2}$$
$$0=\frac{x^2}{2}-(3x-2)$$
$$0=\frac{x^2}{2}-3x+2$$
$$\frac{x^2}{2}-3x+2=0$$
$$ \\ $$
Now that everything is on one side we can apply the quadratic formula.
$$x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}$$
$$ \\ $$
$$\frac{x^2}{2}-3x+2=0$$
$$a=0.5$$
$$b=-3$$
$$c=2$$
$$ \\ $$
$$x=\frac{-(-3)\pm\sqrt{(-3)^2-4(0.5)(2)}}{2(0.5)}$$
$$x=\frac{3\pm\sqrt{9-4}}{1}$$
$$x=\frac{3\pm\sqrt{5}}{1}$$
$$x=3\pm\sqrt{5}$$
$$ \\ $$

To find the y values, we can substitute the x values into one of our given equations.
$$0=3x-2-y$$
$$y=3x-2$$
$$y=3(3\pm\sqrt{5})-2$$
$$y=9\pm3\sqrt{5}-2$$^finding-y-using-x

$$ \\ $$
## Solving by [[Factoring]]
To solve by factoring, we can take our [[Linear and Quadratic Systems of Equations#^substituted-intro-example-system|substituted system]] and factor it. (Since this problem is difficult to factor due to $x^2$'s coefficient, I used wolfram alpha)
$$3x-2=\frac{x^2}{2}$$
$$0=0.5x^2-3x+2$$
$$0=0.5(x-5.23607)(x-0.763932)$$
$$ \\ $$
Next, we can solve for each of the x values.
$$0=0.5(x-5.23607)(x-0.763932)$$
$$\frac{0}{0.5}=(x-5.23607)(x-0.763932)$$
$$\frac{0}{x-0.763932}=x-5.23607$$
$$0+5.23607=x$$
$$x\approx5.23607$$
$$ \\ $$
$$0=0.5(x-5.23607)(x-0.763932)$$
$$\frac{0}{0.5}=(x-5.23607)(x-0.763932)$$
$$\frac{0}{x-5.23607}=x-0.763932$$
$$0+0.763932=x$$
$$x\approx0.763932$$
$$ \\ $$
$$x\approx[5.23607, 0.763932]$$
$$ \\ $$
To find the y values, we can follow the same steps used in the [[Linear and Quadratic Systems of Equations#^finding-y-using-x|solving by using the quadratic formula section]].

## Potential Method to Quickly Solve
When given one equation and the solutions, finding the second equation from a list of answers can be done by substituting the given answer values into the given equation and every equation that is a potential answer as seen below.
Given:
$$y=\frac{1}{2}x^2-6$$
$$(2,-4), (-4,2)$$
$$ \\ $$
Answer Choices:
$$\text{A) }x-y=6$$
$$\text{B) }y-x=6$$
$$\text{C) }x-y=-2$$
$$\text{D) }y+x=-2$$
$$ \\ $$
I find substituting the value that is squared easier than the one that isn't squared because with the latter option, you will have to take the square root, something which does not have to be done with the former method. Additionally, since both the x- and y-coordinates are given, we do not need to substitute one of the variables for one of the given values. However, for completeness this was done anyway below.
$$\text{Given) }y=\frac{1}{2}x^2-6$$
$$ \\ $$
$$y=\frac{1}{2}(2)^2-6$$
$$y=\frac{1}{2}4-6$$
$$y=-4$$
$$ \\ $$
$$y=\frac{1}{2}(-4)^2-6$$
$$y=\frac{1}{2}16-6$$
$$y=2$$
$$ \\ $$
$$y=[-4,2]$$
$$ \\ $$
$$\text{A) }x-y=6$$
$$-y=6-x$$
$$y=x-6$$
$$ \\ $$
$$y=2-6$$
$$y=-4$$
$$ \\ $$
$$y=-4-6$$
$$y=-10$$
$$ \\ $$
$$y=[-4,-10]$$
$$ \\ $$
$$\text{B) }y-x=6$$
$$y=6-x$$
$$ \\ $$
$$y=6-2$$
$$y=4$$
$$ \\ $$
$$y=6-(-4)$$
$$y=10$$
$$ \\ $$
$$y=[4,10]$$
$$ \\ $$
$$\text{C) }x-y=-2$$
$$-y=-2-x$$
$$y=x+2$$
$$ \\ $$
$$y=2+2$$
$$y=4$$
$$ \\ $$
$$y=-4+2$$
$$y=-2$$
$$ \\ $$
$$y=[4,-2]$$
$$ \\ $$
$$\text{D) }y+x=-2$$
$$y=-x-2$$
$$ \\ $$
$$y=-2-2$$
$$y=-4$$
$$ \\ $$
$$y=-(-4)-2$$
$$y=2$$
$$ \\ $$
$$y=[-4,2]$$
$$ \\ $$
$$\text{Given) }y=[-4,2]$$
$$\text{A) }y=[-4,-10]$$
$$\text{B) }y=[4,10]$$
$$\text{C) }y=[4,-2]$$
$$\text{D) }y=[-4,2]$$
$$ \\ $$
Since the given coordinates match with answer choice D, D is the correct answer.