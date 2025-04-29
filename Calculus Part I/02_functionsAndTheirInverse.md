# Course #2: Functions and Its Inverse

# Platform: Edx

# Course Name: DelftX MMFEC1X: Calculus I: From Functions to Differential Equations

# Author: Caesar James LEE

## Unknown Keywords

| English           | Pronunciation     | Chinese Meaning            |
| :---------------: | :---------------: | :------------------------: |
| versatile         | ˈvɝsǝtḷ           | 多功能的；多才多藝的；易變的  |
| restrict          | rɪˈstrɪkt         | 限制；約束                  |
| propagate         | ˈprɑpǝˌɡеt        | 繁殖；傳播                  |
| cable             | ˈkеbḷ             | 纜；越洋電報；有線電視       |
| bedrock           | ˈbɛdˌrɑk          | 床岩；底部                  |

## functions

### definition

* a function $f: \mathbb {R} \rightarrow \mathbb{R}$ associates to each number `x` in its domain **exactly one** number `f(x)`
    * other names
        1. `output value f(x)`: `function value`
        2. `input value x`: `value of the variable`
* for $f(x) = x^2$, we can say `3 has image of 9` or `3 is mapped to 9`

### `domain`, `codomain` and `range`

* a function $f: A \rightarrow B$ is a rule that assigns to each element `x` in the set `A`, a **unique** element `f(x)` in the set `B`

#### `domain`
* set `A` of all possible input values

#### `codomain`
* set `B`

#### `range`
* range `R` of a function $f: A \rightarrow B$ is the set of all possible values of `f(x)` as `x` varies throughout the domain `A`
* $$R = \{f(x) \mid x \in A\}$$

#### `maximal domain`

* `maximal domain` of `f(x)` consists of all real numbers `x` for which the value `f(x)` is real number
* in other words, `maximal domain` is a domain that consists all possible input values

#### differences table
* for the function $f(x) = \frac {1} {x^2}$

| set               | values                                |
| :---------------: | :-----------------------------------: |
| `domain`          | $\{x \in \mathbb{R} \mid x \neq 0\}$  |
| `maximal domain`  | $\{x \in \mathbb{R} \mid x \neq 0\}$  |
| `codomain`        | $[0, \infty)$                         |
| `range`           | $(0, \infty)$                         |

## graphs

### definition

* the graph of a function $f: \mathbb{R} \rightarrow \mathbb{R}$ is the curve going through all the points `(x, f(x))` for `x` in the domain of `f`

## vertical line test

### theorem

* a curve in the plane is the graph of a function over a certain domain if every vertical line at `x-value`s in that domain intersects the curve **exactly once**
* in other words, **only one** point of the graph through every vertical line in the plane

## composition of functions

### product of functions

* given functions `f(x)` and `g(x)`, we can form their product `fg(x)`
$$fg(x) = f(x) \cdot g(x)$$
* example

| functions                     | domains       |
| :---------------------------: | :-----------: |
| $f(x) = \sqrt{x}$             | $[0, \infty)$ |
| $g(x) = x + 2$                | $\mathbb{R}$  |
| $fg(x) = (x + 2)\sqrt{x}$     | $[0, \infty)$ |
| $gf(x) = (x + 2)\sqrt{x}$     | $[0, \infty)$ |

###  composition of functions

* if `f(x)` and `g(x)` are two functions, the composition function $f \circ g$ is defined by
$$(f \circ g)(x) = f(g(x))$$
* example

| functions                                 | domains       |
| :---------------------------------------: | :-----------: |
| $f(x) = x^2 - x$                          | $\mathbb{R}$  |
| $g(x) = \sin(x)$                          | $\mathbb{R}$  |
| $(f \circ g)(x) = (\sin(x))^2 - \sin(x)$  | $\mathbb{R}$  |
| $(g \circ f)(x) = \sin(x^2 - x)$          | $\mathbb{R}$  |

## inverse functions

### definition

* suppose `f` is a function with domain `D` and range `R`, and function `g` is the inverse of `f`, then
$$f(x) = y \Longleftrightarrow x = g(y)$$

### notation of inverse functions

* $$f^{-1}$$
* $$f(f^{-1}(x)) = x \quad and \quad f^{-1}(f(x)) = x$$

### invertibility

* a function `f` is invertible, meaning an inverse function exists, precisely if it is `one-to-one` meaning
$$f(x_1) \neq f(x_2) \quad whenever \quad x_1 \neq x_2$$
* example
    1. $f(x) = x^2$ is **not invertible**, cause it is not a `one-to-one` function, e.g. $f(x) = 1 \quad \rightarrow x = \pm 1$

### graph

* suppose `f` is a function with inverse $f^{-1}$, then you get the graph of $f^{-1}$ by reflecting the graph of `f` in the line `y = x`
* in other words, the graph of a function's inverse is the reflection of the function's graph across the line `y = x`

### horizontal line test

* a function is invertible if and only if all horizontal lines intersect the graph of the function in at most 1 place
* in other words, **only one** point of the graph through every horizontal line in the plane

### differences between `vertical line test` and `horizontal line test` table

| feature                   | `vertical line test`          | `horizontal line test`                        |
| :-----------------------: | :---------------------------: | :-------------------------------------------: |
| purpose                   | check if it is a function     | check if it is `one-to-one` (`invertible`)    |
| only one intersection     | it is a function              | it is `one-to-one` (`invertible`)             |
| multiple intersections    | not a function                | **not** `one-to-one` (`invertible`)           |
| key concept tested        | each `x` has exactly one `y`  | each `y` has exactly one `x`                  |
| summary                   | test if it's a function       | test if it's `one-to-one`                     |

### solving an inverse steps

1. write down the equation $f(x) = y$
2. solve that equation for `x` in terms of `y`
3. substitute `y` for `x` and `x` for `y` to obtain the formula $y = f^{-1}(x)$
* example $y = x^2 + 12x + 2 \quad on \quad D \geq -6$
    1. $$f(x) = x^2 + 12x + 2$$
    2. 
    $$
        y = (x + 6)^2 - 36 + 2\\
        y + 34 = (x + 6)^2\\
        x = \sqrt{y + 34} - 6
    $$
    3. $$f^{-1}(x) = \sqrt{x + 34} - 6 \quad on \quad D \geq -6$$

## inverses of trigonometric functions

### `arcsine`

* `sine` graph
![sine graph](photos/week%201/01-01.png)
* inverse of `sin(x)` exists on $[-\frac {\pi} {2}, \frac {\pi} {2}]$
* definition
    * inverse of $y = \sin(x)$ is the function $y = \arcsin(x)$
    * `domain`: [-1, 1]
    * `range`: $[-\frac {\pi} {2}, \frac {\pi} {2}]$
    * $$y = \arcsin(x) \quad \Longrightarrow \quad \sin(y) = x$$
* `arcsine` graph
![arcsine graph](photos/week%201/01-02.png)
* $\arcsin(x)$ is also denoted as $\sin^{-1}(x)$

### `arccosine`

* `cosine` graph
![cosine graph](photos/week%201/01-03.png)
* inverse of `cos(x)` exists on $[0, \pi]$
* definition
    * inverse of $y = \cos(x)$ is the function $y = \arccos(x)$
    * `domain`: [-1, 1]
    * `range`: $[0, \pi]$
    * $$y = \arccos(x) \quad \Longrightarrow \quad \cos(y) = x$$
* `arccosine` graph
![arccosine graph](photos/week%201/01-04.png)
* $\arccos(x)$ is also denoted as $\cos^{-1}(x)$

### `arctangent`

* `tangent` graph
![tangent graph](photos/week%201/01-05.png)
* inverse of `tan(x)` exists on $(-\frac {\pi} {2}, \frac {\pi} {2})$
* definition
    * inverse of $y = \tan(x)$ is the function $y = \arctan(x)$
    * `domain`: $\mathbb{R}$
    * `range`: $(-\frac {\pi} {2}, \frac {\pi} {2})$
    * $$y = \arctan(x) \quad \Longrightarrow \quad \tan(y) = x$$
* `arctangent` graph
![arctangent graph](photos/week%201/01-06.png)
* $\arctan(x)$ is also denoted as $\tan^{-1}(x)$

### common used `sin(x)`, `cos(x)`, `tan(x)` table

| $x$                   | $\sin(x)$                 | $\cos(x)$                 | $\tan(x)$                 |
| :-------------------: | :-----------------------: | :-----------------------: |:------------------------: |
| $0$                   | $0$                       | $1$                       | $0$                       |
| $\frac {\pi} {6}$     | $\frac {1} {2}$           | $\frac {\sqrt {3}} {2}$   | $\frac {\sqrt {3}} {3}$   |
| $\frac {\pi} {4}$     | $\frac {\sqrt {2}} {2}$   | $\frac {\sqrt {2}} {2}$   | $1$                       |
| $\frac {\pi} {3}$     | $\frac {\sqrt {3}} {2}$   | $\frac {1} {2}$           | $\sqrt {3}$               |
| $\frac {\pi} {2}$     | $1$                       | $0$                       | undefined                 |
| $\frac {2\pi} {3}$    | $\frac {\sqrt {3}} {2}$   | $-\frac {1} {2}$          | $-\sqrt {3}$              |
| $\frac {3\pi} {4}$    | $\frac {\sqrt {2}} {2}$   | $-\frac {\sqrt {2}} {2}$  | $-1$                      |
| $\frac {5\pi} {6}$    | $\frac {1} {2}$           | $-\frac {\sqrt {3}} {2}$  | $-\frac {\sqrt {3}} {3}$  |
| $\pi$                 | $0$                       | $-1$                      | $0$                       |
| $\frac {7\pi} {6}$    | $-\frac {1} {2}$          | $-\frac {\sqrt {3}} {2}$  | $\frac {\sqrt {3}} {3}$   |
| $\frac {5\pi} {4}$    | $-\frac {\sqrt {2}} {2}$  | $-\frac {\sqrt {2}} {2}$  | $1$                       |
| $\frac {4\pi} {3}$    | $-\frac {\sqrt {3}} {2}$  | $-\frac {1} {2}$          | $\sqrt {3}$               |
| $\frac {3\pi} {2}$    | $-1$                      | $0$                       | undefined                 |
| $\frac {5\pi} {3}$    | $-\frac {\sqrt {3}} {2}$  | $\frac {1} {2}$           | $-\sqrt {3}$              |
| $\frac {7\pi} {4}$    | $-\frac {\sqrt {2}} {2}$  | $\frac {\sqrt {2}} {2}$   | $-1$                      |
| $\frac {11\pi} {6}$   | $-\frac {1} {2}$          | $\frac {\sqrt {3}} {2}$   | $-\frac {\sqrt {3}} {3}$  |
| $2\pi$                | $0$                       | $1$                       | $0$                       |

### calculation rules

1. reverse
    1. $$\arcsin(\sin(x)) = \sin(\arcsin(x)) = x$$
    2. $$\arccos(\cos(x)) = \cos(\arccos(x)) = x$$
    3. $$\arctan(\tan(x)) = \tan(\arctan(x)) = x$$
2. using $\sin^2(x) + \cos^2(x) = 1$
    * example $\sin(\arccos(x))$
    $$
        \sin^2(\arccos(x)) + \cos^2(\arccos(x)) = 1\\
        \sin^2(\arccos(x)) = 1 - x^2\\
        \sin(\arccos(x)) = \pm \sqrt {1 - x^2}\\
        \sin(\arccos(x)) = \sqrt {1 - x^2}
    $$
3. substitute
    * example $\cos(\arctan(x))$
    $$
    x = \tan(\theta) \quad \longrightarrow \quad \text {substitute x}\\
    = \frac {opposite} {adjacent} \quad \longrightarrow \quad \text {definition of tangent}\\
    = \frac {x} {1} \quad \longrightarrow \quad \text {x = } \frac {x} {1}\\
    hypotenuse = \sqrt {x^2 + 1} \quad \longrightarrow \quad \text {use Pythagoras' theorem}\\
    \cos(\arctan(x)) = \cos(\theta) \quad \longrightarrow \quad \text {substitute } \theta = \arctan(x)\\
    = \frac {adjacent} {hypotenuse} \quad \longrightarrow \quad \text {definition of cosine}\\
    = \frac {1} {\sqrt {x^2 + 1}}
    $$