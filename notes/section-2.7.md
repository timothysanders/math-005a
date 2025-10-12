# 2.7: Rates of Change in the Natural and Social Sciences
- If we have $y = f(x)$, then the derivative $dy/dx$ can be interpreted as "the rate of change of $y$ with respect to $x$"
- If $x$ changes from $x_1\text{ to }x_2$, then the change in $x$ is $\Delta x = x_2 - x_1$
- The corresponding change in $y$ is $\Delta y = f(x_2) - f(x_1)$
- The difference quotient, $\frac{\Delta y}{\Delta x} = \frac{f(x_2) - f(x_1)}{x_2 - x_1}$, is the **average rate of change of $y$ with respect to $x$** and can be interpreted as the slope of the secant line
  - The units for $\frac{dy}{dx}$ are the units for $y$ divided by the units for $x$
  - Using Leibniz notation, this is written as $$\frac{dy}{dx} = \lim_{\Delta x \to 0}\frac{\Delta y}{\Delta x}$$

## Physics
- If $s = f(t)$ is the position function of a particle moving in a straight line, then $\Delta s/\Delta t$ represents the average velocity over a time period $\Delta t$, and $v = ds/dt$ represents the **instantaneous velocity** (rate of change of displacement with respect to time)
- The instantaneous rate of change of velocity with respect to time is **acceleration**: $a(t) = v'(t) = s''(t)$
- Example: position of a particle is given by $s = f(t) = t^3 - 6t^2 + 9t$
  - $t$ is measured in seconds and $s$ in meters
  - Velocity function is the derivative of the position function
    - $v(t) = \frac{ds}{dt} = 3t^2 - 12t + 9$ (using power rule)
  - Velocity after 2 seconds means instantaneous velocity when $t = 2$
    - $$v(2) = \frac{ds}{dt}|_{t=2} = 3(2)^2 - 12(2) + 9 = -3m/s$$
    - $$v(4) = \frac{ds}{dt}|_{t=4} = 3(4)^2 - 12(4) + 9 = 9m/s$$
  - Particle is at rest when $v(t)$ = 0
    - $$3t^2 - 12 + 9 = 3(t^2 - 4t + 3) = 3(t-1)(t-3) = 0$$
    - Which means it is at rest when $t = 1$ or $t = 3$
- Velocity, density, and current are not the only rates of change that are important in physics. Others include power(rate at which work is done), rate of heat flow, temperature gradient (rate of change of temperature with respect to position), and rate of decay of a radioactive substance

## Chemistry
- Rate of reaction = $\frac{d[C]}{dt} = -\frac{d[A]}{dt} = -\frac{d[B]}{dt}$
- Isothermal compressibility = $\beta = -\frac{1}{V}\frac{dV}{dP}$
  - Volume = V; Pressure = P

## Biology
- Example: $n = f(t)$ represents the number of individuals in a population at time t
  - Average rate of growth = $\frac{\Delta n}{\Delta t} = \frac{f(t_2) - f(t_1)}{t_2 - t1}$
  - Instantaneous rate of growth is obtained from this average rate of growth
  - Growth rate = $\lim_{\Delta t \to 0}\frac{\Delta n}{\Delta t} = \frac{dn}{dt}$

## Economics
- Example: $C(x)$ is the total cost a company incurs to produce $x$ units of a commodity, this function $C$ is called a **cost function**
  - If additional units are produced (going from $x_1$ to $x_2$), then the additional cost is $\Delta C = C(x_2) - C(x_1)$
  - Average rate of change would be $\frac{\Delta C}{\Delta x} = \frac{C(x_2) - C(x_1)}{x_2 - x_1} = C(x_1 + \Delta x) - C(x_1)}{\Delta X}$
  - Instantaneous rate of change of cost with respect to the number of items produced is called the marginal cost by economists
    - Marginal cost = $\lim_{\Delta x \to 0}\frac{\Delta C}{\Delta x} = \frac{dC}{dx}$
  - A concrete example, $C(x) = 10000 + 5x + 0.01x^2$
    - Marginal cost function: $C'(x) = 5 + 0.02x$