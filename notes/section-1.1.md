## 1.1: Four Ways to Represent a Function
## Functions
- Functions arise when one quantity depends on another (independent variable $\to$ dependent variable))
  - The area of a circle ($A$), which is dependent on the radius ($r$). This is given by the equation $A = \pi r^2$
  - The population of the world ($P$), which is dependent on a particular time ($t$). So, "$P$ is a function of $t$"
  - Other examples include the cost of mailing an envelope depends on its weight, the vertical acceleration of the ground during an earthquake is a function of the elapsed time
- When given a number, another number is assigned, so the second number "is a function of" the first number. This can be represented in **functional notation**, $A = f(r)$
- A **function** is a rule to assign each element $x$ in set $D$ to exactly one element, $f(x)$ in set $E$
  - The set $D$ is called the **domain** of the function, $f(x)$ is the value of $f$ at $x$ and is said "f of x"
  - The **range** of $f$ is all possible values of $f(x)$ as x varies through the domain
  - An arbitrary number in the *domain* of the function is called the **independent variable**
    - This is the **input** of the function, so the domain is the set of all possible inputs
  - A number in the *range* of the function is called the **dependent variable**
    - This is the **output** of the function, so the range is the set of all possible outputs
  - You can visualize a function through its graph, where you have ordered pairs of $(x, f(x))$ where $y = f(x)$
- In calculus, the most common method of defining a function is by an algebraic equation, such as $f(x) = 2x - 1$

#### Appended Notes
- A function is formally defined as a relation that assigns to each element in the domain exactly one element in the range.
- The independent variable is the input value from the domain, and the dependent variable is the output value from the range.
- The domain and range can be represented on graphs, where the horizontal axis typically shows the domain (input values) and the vertical axis shows the range (output values).
- Functions can also be visualized using machine diagrams, where inputs go into a "machine" that produces outputs, or arrow diagrams that map elements of the domain to elements of the range.
- Interval notation is commonly used to describe the domain and range, for example, $[0, \infty)$ for all non-negative real numbers.
- Examples of functions include:
  - (A) Area of a circle: $A = \pi r^2$, where $r$ is the radius (independent variable) and $A$ is the area (dependent variable).
  - (B) World population $P$ as a function of time $t$.
  - (C) Cost of mailing an envelope as a function of its weight.
  - (D) Vertical acceleration during an earthquake as a function of elapsed time.
- Common graph examples include:
  - Linear function: $f(x) = 2x - 1$, which produces a straight line.
  - Quadratic function: $g(x) = x^2$, which produces a parabola.
- The difference quotient, given by $\frac{f(x+h) - f(x)}{h}$, represents the average rate of change of the function over the interval from $x$ to $x+h$.

## Representations of Functions
- Four different ways to represent a function, sometimes going from one representation to another can help gain additional insight
  - Verbally: by description in words
  - Numerically: by a table of values
    - This can also be called a *tabular* function
  - Visually: by a graph
  - Algebraically: by an explicit formula
- **Domain function**: when a function is given by a formula and the domain is not stated explicitly, we use the set of all inputs for which the formula makes sense and gives a real-number output for the domain

#### Appended Notes
- Circle area function: The algebraic representation is $A(r) = \pi r^2$, with domain $(0,\infty)$ since radius must be positive, and range $(0,\infty)$ as area is always positive. The graph looks like half a parabola opening upwards.
- World population example: The function describing world population $P$ as a function of time $t$ can be described verbally, represented numerically by a table of values, and visualized with a scatter plot of data points. A common mathematical model approximation is $P(t) \approx (1.43653 \times 10^9)(1.01395)^t$, showing how functions can model real-world data.
- Mailing cost function: The cost of mailing an envelope as a function of its weight can be described verbally and represented with a stepwise table of values, reflecting price increments for weight brackets. This can be graphed as a step function, introducing the term "tabular function" for such numerical representations.
- Seismograph function: The vertical acceleration of the ground during an earthquake is most naturally represented by a graph of acceleration versus time, which shows patterns and fluctuations more clearly than formulas or tables.
- Example 4: Hot water faucet function—The temperature of water rises from room temperature, levels off at a certain temperature, then decreases when the hot water tank drains. This can be described verbally and sketched as a rough graph illustrating the behavior.
- Example 5: Storage container cost function—The cost $C$ as a function of weight $w$ is modeled algebraically by $C(w) = 20w^2 + \frac{180}{w}, \, w>0$. This example is used in applied modeling to solve maximum or minimum cost problems.
- Domain convention: If the domain is not explicitly stated, it is assumed to be all inputs for which the formula makes sense and yields real outputs.
  - Example: For $f(x) = \sqrt{x+2}$, the domain is $[-2,\infty)$ because the expression under the square root must be non-negative.
  - Example: For $g(x) = \tfrac{1}{x^2 - x}$, the domain excludes values where the denominator is zero, i.e., $x=0$ and $x=1$, so the domain is $(-\infty,0) \cup (0,1) \cup (1,\infty)$.

## Which Rules Define Functions?
- Not every equation defines a function, a function must have only one value of $y$ for each value of $x$ (remember the vertical line test). In the same manner, not every table defines a function
- **Vertical Line Test**: A curve on the xy-plane is a graph of a function $x$ if and only if no vertical line intersects the curve more than once
#### Appended Notes
- Not every equation defines a function. Example: $y = x^2$ defines $y$ as a function of $x$, but $x = y^2 - 2$ does not define $y$ as a function of $x$ since one $x$ value can correspond to two $y$ values.
- Tables: A valid function must map each input to exactly one output. Example: mailing cost table is valid, but a table where $x=5$ gives $y=7$ and $y=8$ is not a function.
- Vertical Line Test: A curve in the $xy$-plane is the graph of a function of $x$ if and only if no vertical line intersects it more than once. This ensures one output per input.
- Example with parabola: The equation $x = y^2 - 2$ fails the vertical line test if graphed as $y$ vs $x$, but can be expressed as two separate functions $y = \pm\sqrt{x+2}$. Reversing roles of $x$ and $y$, it can define $x$ as a function of $y$.

## Piecewise Defined Functions
- A **piecewise defined function** is a function with different formulas in different parts of their domains
- When graphing piecewise defined functions, remember that a solid dot indicates the point is included on the graph, an open dot indicates the point is excluded from the graph
- We also have **absolute value functions** and **step functions**
#### Appended Notes
- A piecewise defined function uses **different formulas for different parts of its domain**, but it is still considered a single function.
- **Example 7**:  
  $$
  f(x) =
  \begin{cases}
  1 - x & \text{if } x \leq -1 \\
  x^2 & \text{if } x > -1
  \end{cases}
  $$
  - Even though two formulas are used, this defines one function.  
  - When graphing, solid dots indicate included endpoints and open dots indicate excluded endpoints.
- **Absolute Value Function**:  
  - Defined as the distance from a number to 0 on the real number line, so $|a| \geq 0$.  
  - Piecewise definition:  
    $$
    |x| =
    \begin{cases}
    x & \text{if } x \geq 0 \\
    -x & \text{if } x < 0
    \end{cases}
    $$
  - Graph is a "V" shape, coinciding with $y=x$ for $x \geq 0$ and $y=-x$ for $x<0$.
- **Example 9**: Constructing a function from a graph.  
  - If the graph passes through $(0,0)$ to $(1,1)$, then $(1,1)$ to $(2,0)$, and then continues along the $x$-axis for $x>2$, the function is:
    $$
    f(x) =
    \begin{cases}
    x & 0 \leq x \leq 1 \\
    2 - x & 1 < x \leq 2 \\
    0 & x > 2
    \end{cases}
    $$
- **Step Functions**:  
  - Defined as piecewise constant functions that jump between values.  
  - Example: Mailing cost function  
    $$
    C(w) =
    \begin{cases}
    1.00 & 0 < w \leq 1 \\
    1.15 & 1 < w \leq 2 \\
    1.30 & 2 < w \leq 3 \\
    1.45 & 3 < w \leq 4 \\
    \vdots
    \end{cases}
    $$  
  - These graphs look like "steps" (hence the name).

## Even and Odd Functions
- If a function $f$ satisfies $f(-x) = f(x)$ for every number $x$ in its domain, then it is called an **even function**
  - An example of this is $f(x) = x^2$
  - The graphs of these functions are symmetric with respect to the y-axis
- If a function $f$ satisfies $f(-x) = -f(x)$ for every number $x$ in its domain, then it is called an **odd function**
  - An example of this is $f(-x) = (-x)^3 = -x^3 = -f(x)$
  - The graph of an odd function is symmetric about the origin, meaning you can obtain the entire graph by plotting $f(x); x \geq 0$ and rotating this portion about the origin
#### Appended Notes
- An **even function** satisfies $f(-x) = f(x)$ for every $x$ in its domain.  
  - Example: $f(x) = x^2$, since $f(-x) = (-x)^2 = x^2 = f(x)$.  
  - Graphs of even functions are symmetric about the $y$-axis.  
  - To graph an even function, it suffices to plot for $x \geq 0$ and reflect about the $y$-axis.
- An **odd function** satisfies $f(-x) = -f(x)$ for every $x$ in its domain.  
  - Example: $f(x) = x^3$, since $f(-x) = (-x)^3 = -x^3 = -f(x)$.  
  - Graphs of odd functions are symmetric about the origin.  
  - To graph an odd function, it suffices to plot for $x \geq 0$ and rotate the portion $180^\circ$ about the origin.
- Not all functions are even or odd. Some functions are **neither**.  
  - Example functions:  
    - $f(x) = x^5 + x$ is odd.  
    - $g(x) = 1 - x^4$ is even.  
    - $h(x) = 2x - x^2$ is neither, since $h(-x) \neq h(x)$ and $h(-x) \neq -h(x)$.  
  - Graphs of "neither" functions do not have symmetry about the $y$-axis or the origin.

## Increasing and Decreasing Functions
- A function is called **increasing** on an interval $I$ if $f(x_1) \lt f(x_2)$ whenever $x_1 \lt x_2$ in $I$
  - In the definition of an increasing function, the inequality $f(x_1) \lt f(x_2)$ must be satisfied for *every* pair of numbers $x_1$ and $x_2$ in $I$ with $x_1 \lt x_2$
- A function is called **decreasing** on an interval $I$ if $f(x_1) \gt f(x_2)$ whenever $x_1 \lt x_2$ in $I$
#### Appended Notes
- A function is called **increasing** on an interval $I$ if $f(x_1) < f(x_2)$ whenever $x_1 < x_2$ in $I$.  
  - The inequality must hold for **every pair of numbers** $x_1$ and $x_2$ in $I$ with $x_1 < x_2$.
- A function is called **decreasing** on an interval $I$ if $f(x_1) > f(x_2)$ whenever $x_1 < x_2$ in $I$.
- Example: For $f(x) = x^2$,  
  - $f$ is decreasing on $(-\infty, 0]$.  
  - $f$ is increasing on $[0, \infty)$.  
  - This matches the symmetry of the parabola, which decreases until its vertex and increases thereafter.
- More generally, a graph can alternate between intervals of increase and decrease.  
  - Example: In a graph with intervals $[a,b]$, $[b,c]$, $[c,d]$, the function could be increasing on $[a,b]$, decreasing on $[b,c]$, and increasing again on $[c,d]$.