# 3.7: Optimization Problems
- Methods learned in this chapter are applicable to many areas of life
- The hardest part of these problems is often converting the word problem to a mathematical optimization problem by setting up the function to be maximized or minimized
> #### Steps in Solving Optimization Problems
> 1. **Understand the Problem**: first step is to clearly understand the problem. What is the unknown? What are the given quantities? What are the given conditions?
> 2. **Draw a Diagram**: In most problems, it is useful to draw a diagram and identify the given and required quantities on the diagram
> 3. **Introduce Notation**: Assign a symbol to the quantity that is to be maximized or minimized (can start with $Q$). Also, select symbols for other unknown quantities and label the diagram with these symbols. It can be helpful to use relevant initials, like $A$ for area, $h$ for height, etc.
> 4. Express $Q$ in terms of some of the other symbols (from step 3)
> 5. If Q has been expressed as a function of more than one variable in step four, use the given information to find relationships (equations) among these variables. Then use these equations to eliminate all but one of the variables in the expression for $Q$. Write the domain of this function in the given context
> 6. Use the methods in sections 3.1 and 3.3 to find the absolute maximum or minimum value of $f$. If the domain of $f$ is a closed interval, then the Closed Interval Method in section 3.1 can be used
- Example: Farmer has 2400ft of fencing and wants to fence off a rectangular field bordering a straight river. No fence along the river. What are the field dimensions that have the largest area?
  - Introduce notation: we wish to maximize area, so $A$.
    - We can use $x$ and $y$ for depth and width of the rectangle (field)
    - Then we express $A$ in terms of $x$ and $y$, so $A = xy$
  - We want to express $A$ as a function of one variable, so we can eliminate $y$
    - Using the given information (2400ft of fencing), we can say $2x + y = 2400$
      - Then we can do $y = 2400 - 2x$
    - Plugging in to original expression $A = xy = x(2400 - 2x) = 2400x - 2x^2$
  - $x$ cannot be negative and cannot be more than 1200, so we have $A(x) = 2400 - 2x^2; 0 \leq x \leq 1200$
  - Find the derivative, $A'(x) = 2400 - 4x$
    - To find critical numbers, we solve the equation $2400 - 4x = 0$
    - This gives us $x = 600$, which means the maximum value of $A$ must occur either at this critical number or at an endpoint of the interval
  - Find corresponding $y$ value, which is $y = 2400 - 2(600) = 1200$, so the field dimensions are 600ft deep and 1200ft wide
- Example: A cylindrical can is to be made to hold 1L of oil, we want to minimize the cost of the metal to manufacture the can
  - First draw a diagram where $r$ is the radius and $h$ is the height
  - We want to minimize total surface area, so we need to find the equation for the total surface area
    - $A = 2\pi r^2 + 2\pi rh$
      - $2\pi r^2$ because we need the top and bottom circles of the can
      - $2\pi rh$ because we need the circumference of the circle and the height to get the outer surface area of the can
  - We want to express $A$ in terms of one variable, $r$, so we eliminate $h$
    - Because we are given the volume of 1L ($1000\text{cm}^3$), $\pi r^2h = 1000$
    - This allows us to find $h = \frac{1000}{\pi r^2}$
    - Substitute back into expression for $A$
    - $A = 2\pi r^2 + 2\pi r(\frac{1000}{\pi r^2}) = 2\pi r^2 + \frac{2000}{r}$
  - We know that $r$ must be positive, so our function and domain are as follows
    - $A(r) = 2\pi r^2 + \frac{2000}{r}; r \gt 0$
  - Find critical numbers by differentiating
    - $A'(r) = 4\pi r - \frac{2000}{r^2} = \frac{4(\pi r^3 - 500)}{r^2}$
    - $A'(r) = 0$ when $\pi r^3 = 500$, so the only critical number is $r = \sqrt[3]{500/\pi}$
  - Value of $h$ corresponding to $r = \sqrt[3]{500/\pi}$ is $$h = \frac{1000}{\pi r^2} = \frac{1000}{\pi(500/\pi)^{2/3}} = 2\sqrt[3]{\frac{500}{\pi}} = 2r$$
> #### First Derivative Test for Absolute Extreme Values
> - Suppose that $c$ is a critical number of a continuous function $f$ defined on an interval
>   a. If $f'(x) \gt 0$ for all $x \lt c$ and $f'(x) \lt 0$ for all $x \gt c$, then $f(c)$ is the absolute maximum value of $f$
>   b. If $f'(x) \lt 0$ for all $x \lt c$ and $f'(x) \gt 0$ for all $x \gt c$, then $f(c)$ is the absolute minimum value of $f$

## Applications to Business and Economics