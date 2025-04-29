# Course #3: Differentiation

# Platform: Edx

# Course Name: DelftX MMFEC1X: Calculus I: From Functions to Differential Equations

# Author: Caesar James LEE

## Unknown Keywords

| English           | Pronunciation     | Chinese Meaning            |
| :---------------: | :---------------: | :------------------------: |
| decompression     | ˌdikǝmˈprɛʃǝn     | 減壓                       |
| instantaneous     | ˌɪnstǝnˈtеnɪǝs    | 瞬間的；猝發的；瞬時的       |
| kink              | kɪŋk              | 扭結；抽筋                  |
| scenario          | sɪˈnɛrɪˌo         | 方案；情況                  |
| implicit          | ɪmˈplɪsɪt         | 含蓄的；內含的；隱式的       |
| explicit          | ɪkˈsplɪsɪt        | 詳盡的；直率的；顯式的       |
| neat              | nit               | 整潔的；熟練的；光滑的       |
| differential      | ˌdɪfǝˈrɛnʃǝl      | 差別的；獨特的；微分的       |

## derivatives

### concept definitions

#### rate of change

* rate of change of the function $y = f(x)$ over the interval $[a, b]$ is given by
$$\frac {\Delta y} {\Delta x} = \frac {f(b) - f(a)} {b - a}$$

#### instantaneous rate of change

* let the width $\Delta x$ of the interval $[a, b]$ approach 0, the rate of change of the function $f(x)$ will approach the derivative f'(a) at the point a
$$
f'(a) = \lim_{\Delta x \rightarrow 0} \frac {\Delta y} {\Delta x}\\
= \lim_{b \rightarrow a} \frac {f(b) - f(a)} {b - a}
$$

#### tangent line

* given a function $f(x)$ the tangent line to the graph of $f$ at the point $a$ in the domain is given by the equation
$$y = f(a) + f'(a)(x - a)$$
* photo
![tangent line graph](photos/week%202/02-01.png)

#### derivatives at a point

* the slope of the tangent line to the function $f$ at the point $a$ is denoted by $f'(x)$ or $\frac {df} {dx}$ and called the derivative of $f$ at $a$

#### differentiable

* given a function $f: D \rightarrow \mathbb{R}$ that is differentiable at each point $a$ in $D$ we define the derivative $f': D \rightarrow \mathbb{R}$ as the function that associates the derivative of $f$ at $a$ to each point $a$ in the domain $D$
* not differentiable examples
    1. `jump`

        ![jump example](photos/week%202/02-02.png)
    2. `kink`

        ![kink example](photos/week%202/02-03.png)

#### notations

1. first derivative: $f'(x)$ or $\frac {df} {dx}$
2. second derivative: $f''(x)$ or $\frac {d^2f} {dx^2}$
3. third derivative: $f^{(3)}(x)$ or $\frac {d^3f} {dx^3}$
4. n-th derivative: $f^{(n)}$ or $\frac {d^nf} {dx^n}$

#### computation rules

1. standard derivatives

| Standard Function                     | Derivative                                    |
| :-----------------------------------: | :-------------------------------------------: |
| ***BASIC***                           | ***BASIC***                                   |
| $a$                                   | $0$                                           |
| $x^a$                                 | $ax^{a - 1}$                                  |
| ***TRIGONOMETRIC***                   | ***TRIGONOMETRIC***                           |
| $\sin(x)$                             | $\cos(x)$                                     |
| $\cos(x)$                             | $-\sin(x)$                                    |
| $\arcsin(x)$                          | $\frac {1} {\sqrt {1 - x^2}}$                 |
| $\arccos(x)$                          | $-\frac {1} {\sqrt {1 - x^2}}$                |
| $\arctan(x)$                          | $\frac {1} {1 + x^2}$                         |
| ***LOGARITHM & EXPONENTIAL***         | ***LOGARITHM & EXPONENTIAL***                 |
| $\log_a(x)$                           | $\frac {1} {x\ln(a)}$                         |
| $\ln(x)$                              | $\frac {1} {x}$                               |
| $a^x, \quad a > 0$                    | $a^x\ln(a)$                                   |
| $e^x$                                 | $e^x$                                         |

2. scalar multiplication rule
$$(c \cdot f(x))' = c \cdot f'(x) \quad \text {for c } \in \mathbb{R}$$
3. sum and difference rule
$$(f(x) \pm g(x))' = f'(x) \pm g'(x)$$
4. product rule
$$(f(x) \cdot g(x))' = f'(x) \cdot g(x) + f(x) \cdot g'(x)$$
5. quotient rule
$$(\frac {f(x)} {g(x)})' = \frac {f'(x) \cdot g(x) -  f(x) \cdot g'(x)} {(g(x))^2}$$
6. chain rule
$$f(g(x))' = f'(g(x)) \cdot g'(x)$$

### implicit differentiation

#### implicit vs explicit

* `explicit function` is a function that you can directly solve for `y`
    * example
        1. $y = x^3$
        2. $y = \sqrt{x - 12}$
        3. $y = \sin(x) + \cos^2(x)$
* `implicit function` is a function where variables are mixed, and you cannot directly solve for `y`
    * example
        1. $x^2 + y^2 = 12$
        2. $x^2 + xy + y^2 = 3$
        3. $e^{xy} + x^2y^2 = 7$

#### solve derivative of an implicit function steps

1. differentiate $F_x$, and treat all $y$ as a constant number
2. differentiate $F_y$, and treat all $x$ as a constant number
2. solve for $\frac {dy} {dx} = -\frac {F_x} {F_y}$
* example: $x^2 + y^2 = 12$
    1. $$F_x = 2x + 0 - 0$$
    $$F_x = 2x$$
    2. $$F_y = 0 + 2y - 0$$
    $$F_y = 2y$$
    3. $$\frac {dy} {dx} = -\frac {2x} {2y}$$
    $$\frac {dy} {dx} = -\frac {x} {y}$$
* example: $x^3 + y^3 = 6xy$
    1. $$F_x = 3x^2 - 6y$$
    2. $$F_y = 3y^2 - 6x$$
    3. $$\frac {dy} {dx} = -\frac {3x^2 - 6y} {3y^2 - 6x}$$
    $$\frac {dy} {dx} = \frac {6y - 3x^2} {3y^2 - 6x}$$

#### solve tangent line of an implicit function formula

$$y = \left. \frac {dy} {dx} \right|_{(x_0, y_0)} (x - x_0) + y_0$$

#### general formula to find the derivative of an inverse function

$$\frac {d} {dx} f^{-1}(x) = \frac {1} {f'(f^{-1}(x))}$$

* explanation
1. using inverse definition
$$f(f^{-1}(x)) = x$$
2. differentiate each term
$$\frac {d} {dx} f(f^{-1}(x)) = \frac {d} {dx} x$$
$$f'(f^{-1}(x)) \cdot \frac {d} {dx} f^{-1}(x) = 1$$
$$\frac {d} {dx} f^{-1}(x) = \frac {1} {f'(f^{-1}(x))}$$
* example: $f: \quad e^x \quad f^{-1}: \quad \ln(x)$
$$\frac {d} {dx} e^x = \frac {1} {e^{\ln(x)}}$$
$$= \frac {1} {x}$$