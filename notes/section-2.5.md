# 2.5: The Chain Rule
- Using the example $F(x) = \sqrt{x^2 + 1}$, we see that $F$ is a composite function
  - We can break it into $f(u) = \sqrt{u}$ and $g(x) = x^2 + 1$, then we can write $f(g(x))$

## The Chain Rule
- The derivative of the composite function $f(g(x))$ is a product of the derivatives $f$ and $g$
  - This is one of the most important of the differentiation rules
#### The Chain Rule
- If $g$ is differentiable at $x$ and $f$ is differentiable at $g(x)$, then the composite function $F = f \circ g$ defined by $F(x) = f(g(x))$ is differentiable at $x$ and $F'$ is given by the product $$F'(x) = f'(g(x)) \cdot g'(x)$$
- Using Leibniz notation, if $y = f(u)$ and $u = g(x)$ are both differentiable functions, then $$\frac{dy}{dx} = \frac{dy}{du}\frac{du}{dx}$$
- Example: Find $F'(x)\text{ if }F(x) = \sqrt{x^2 + 1}$
  - $f(u) = \sqrt{u}$ and $g(x) = x^2 + 1$
  - $f'(u) = \frac{1}{2}u^{-\frac{1}{2}} = \frac{1}{2\sqrt{u}}$ (using the power rule)
  - $g'(x) = 2x$ (again using power rule, and derivative of a constant is 0)
  - We have $F'(x) = f'(g(x)) \cdot g'(x)$
    - $= \frac{1}{2\sqrt{x^2 + 1}} \cdot 2x = \frac{x}{\sqrt{x^2 + 1}}$
- Example: differentiate $y = \sin(x^2)$
  - $f(u) = \sin u$ and $g(x) = x^2$
  - $f'(u) = \cos u$
  - $g'(x) = 2x$
  - $F' = \cos(x^2) \cdot 2x = 2x\cos(x^2)$
- Example: differentiate $y = \sin^2x$
  - $f(u) = \sin^2(u) = (u)^2$ and $g(x) = \sin(x)$
  - $f'(u) = 2 \cdot \sin(u)$
  - $g'(x) = \cos x$
  - $F'(x) = 2 \cdot \sin(x) \cdot \cos x = 2\sin x \cos x$
#### Power Rule Combined with the Chain Rule
- If $n$ is any real number and $u = g(x)$ is differentiable, then $$\frac{d}{dx}(u^n) = nu^{n-1}\frac{du}{dx}$$
- Alternatively, $$\frac{d}{dx}[g(x)]^n = n[g(x)]^{n-1}\cdot g'(x)$$
- Example: differentiate $y = (x^3 - 1)^{100}$
  - Taking $u = g(x) = x^3 - 1$ and $n = 100$, we get $$\frac{dy}{dx} = \frac{d}{dx}(x^3 - 1)^{100} = 100(x^3 - 1)^{99}\frac{d}{dx}(x^3 - 1)$$
  - $$= 100(x^3 - 1)^{99} \cdot 3x^2 = 300x^2(x^3 - 1)^{99}$$
- Example: differentiate $f(x) = \frac{1}{\sqrt[3]{x^2 + x + 1}}$
  - First step is to rewrite $f(x) = (x^2 + x + 1)^{-\frac{1}{3}}$
  - Then $-\frac{1}{3}(x^2 + x + 1)^{-\frac{4}{3}}\frac{d}{dx}(x^2 + x + 1)$
  - $= -\frac{1}{3}(x^2 + x + 1)^{-\frac{4}{3}}(2x + 1)$
- Example: find derivative of $g(t) = (\frac{t - 2}{2t + 1})^9$
  - Here, we will combine the power rule, chain rule, and quotient rule
  - $g'(t) = 9(\frac{t - 2}{2t + 1})^8\frac{d}{dt}(\frac{t - 2}{2t + 1})$
  - $= 9(\frac{t - 2}{2t + 1})^8\frac{(2t + 1) \cdot 1 - 2(t - 2)}{(2t + 1)^2} = \frac{45(t - 2)^8}{(2t + 1)^{10}}$
- Example: differentiate $y = (2x + 1)^5(x^3 - x + 1)^4$
  - $\frac{dy}{dx} = (2x + 1)^5\frac{d}{dx}(x^3 - x + 1)^4 + (x^3 - x + 1)^4\frac{d}{dx}(2x + 1)^5$
  - $= (2x + 1)^5 \cdot 4(x^3 - x + 1)^3\frac{d}{dx}(x^3 - x + 1) + (x^3 - x + 1)^4 \cdot 5(2x + 1)^4\frac{d}{dx}(2x+1)$
  - $= 4(2x + 1)^5(x^3 - x + 1)^3(3x^2 - 1) + 5(x^3 - x + 1)^4(2x + 1)^4 \cdot 2$
  - $\frac{dy}{dx} = 2(2x + 1)^4(x^3 - x + 1)^3(17x^3 + 6x^2 - 9x + 3)$
#### Extending Chain Rule
- The chain rule can be extended by adding more links
- For example, $y = f(u)$, $u = g(x)$ and $x = h(t)$ where $f, g,\text{ and }h$ are differentiable
- To compute the derivative of $y$ with respect to $t$, you can use the chain rule twice: $$\frac{dy}{dt} = \frac{dy}{dx}\frac{dx}{dt} = \frac{dy}{du}\frac{du}{dx}\frac{dx}{dt}$$
- Example: $f(x) = \sin(\cos(\tan(x)))$
  - $f'(x) = \cos(\cos(\tan x))\frac{d}{dx}\cos(\tan x)$
  - $= \cos(\cos(\tan x))[-\sin(\tan x)\frac{d}{dx}(\tan x)$
  - $= -\cos(\cos(\tan x))\sin(\tan x)\sec^2 x$
- Example: differentiate $y = \sqrt{\sec x^3}$
  - Outer function is the square root function, middle function is secant function, inner function is cubing function
  - $\frac{dy}{dx} = \frac{1}{2\sqrt{\sec x^3}}\frac{d}{dx}(\sec x^3)$
  - $\frac{1}{2\sqrt{\sec x^3}}\sec x^3 \tan x^3\frac{d}{dx}(x^3)$
  - $\frac{3x^2\sec x^3 \tan x^3}{2\sqrt{\sec x^3}}$

## How to Prove the Chain Rule
- If $y = f(x)$ and $x$ changes from $a$ to $a + \Delta x$, the increment of $y$ is defined as $$\Delta y = f(x + \Delta x) - f(a)$$
- Following the definition of a derivative, we have $$\lim_{\Delta x \to 0}\frac{\Delta y}{\Delta x} = f'(a)$$
- If we denote the difference between $\Delta y / \Delta x$ and $f'(a)$ as $\epsilon$, then we get $$\lim_{\Delta x \to 0}\epsilon = \lim_{\Delta x \to 0}(\frac{\Delta y}{\Delta x} - f'(a)) = f'(a) - f'(a) = 0$$
- But $$\epsilon = \frac{\Delta y}{\Delta x} - f'(a) \to \Delta y = f'(a)\Delta x + \epsilon\Delta x$$
- If we define $\epsilon$ to be 0 when $\Delta x = 0$, then $\epsilon$ becomes a continuous function of $\Delta x$, so we can write $$\Delta y = f'(a)\Delta x + \epsilon\Delta x\text{ where }\epsilon \to 0\text{ as }\Delta x \to 0$$
