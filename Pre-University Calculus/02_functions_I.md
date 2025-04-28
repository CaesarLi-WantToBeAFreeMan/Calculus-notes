# Course #1: Functions Part I

# Platform: Edx

# Course Name: DelftX Calc001x: Pre-University Calculus

# Author: Caesar James LEE

## Unknown Keywords:

| English       | Pronunciation   | Chinese Meaning |
| :-----------: | :-------------: | :-------------: |
| domain        | doˈmеn          | 定義域           |
| codomain      | ˈkəʊdomеn       | 對應域           |
| continuity    | ˌkɑntǝˈnjuǝtɪ   | 連續性           |
| polynomial    | ˌpɑlɪˈnomɪǝl    | 多項式的         |
| friction      | ˈfrɪkʃǝn        | 摩擦力           |
| trigonometric | ˌtrɪɡǝnǝˈmɛtrɪk | 三角學的         |
| piecewise     | pis waɪz        | 分段            |
| partitioned   | pɑrˈtɪʃǝn       | 分割            |
| asymptotically| еˌsɪmptɑˈtɪkḷɪ  | 漸進            |
| equivalent    | ɪˈkwɪvǝlǝnt     | 等價            |
| slope         | slop            | 斜率            |
| intercept     | ˌɪntɚˈsɛpt      | 截取            |
| factorized    | ˈfæktəˌraɪzd    | 因數的          |
| quadratic     | kwɑdˈrætɪk      | 二次的          |
| vertex        | ˈvɝtɛks         | 頂點            |
| interpret     | ɪnˈtɝprɪt       | 解釋            |
| plot          | plɑt            | 測定（點線）位置 |
| arbitrary     | ˈɑrbǝˌtrɛrɪ     | 隨心所欲的       |
| rational      | ˈræʃǝnḷ         | 有理的          |
| numerator     | ˈnjumǝˌrеtɚ     | 分子            |
| denominator   | dɪˈnɑmǝˌnеtɚ    | 分母            |
| asymptote     | ˈæsɪmˌtot       | 漸近線          |
| oblique       | ǝbˈlik          | 斜的            |
| restriction   | rɪˈstrɪkʃən     | 限制            |
| attain        | əˈten           | 達到            |
| rope          | rop             | 繩              |
| delimit       | diˈlɪmɪt        | 限定            |
| continuity    | ˌkɑntǝˈnjuǝtɪ   | 連續性          |
| intermediate  | ˌɪntɚˈmidɪǝt    | 中間的          |
| spring        | sprɪŋ           | 彈簧            |
| equilibrium   | ˌikwǝˈlɪbrɪǝm   | 平衡            |
| exert         | ɪɡˈzɝt          | 用（力）        |
| suspension    | sǝˈspɛnʃǝn      | 懸掛            |
| pillar        | ˈpɪlɚ           | 柱子；棟樑      | 
| parabola      | pǝˈræbǝlǝ       | 拋物線          |
| sketch        | skɛtʃ           | 草圖            |
| inhabitant    | ɪnˈhæbǝtǝnt     | 居民            |
| empirical     | ɛmˈpɪrɪkḷ       | 經驗（上）的     |
| approximate   | ǝˈprɑksǝmɪt     | 近似的          |
| municipality  | mjuˌnɪsǝˈpælǝtɪ | 自治市          |
| laminar       | ˈlæmɪnɚ         | 流線的          |
| fountain      | ˈfaʊntɪn        | 泉水            |
| nozzle        | ˈnɑzḷ           | 嘴              |

## Unknown Abbreviations:

| Abbreviation  | Full Name         | Chinese Meaning |
| :-----------: | :---------------: | :-------------: |
| LHS           | Left-Hand Side    | 左側的式子       |
| RHS           | Right-Hand Side   | 右側的式子       |

## Standard Functions

### 1. Polynomial Functions
   * $$f(x) = x^2$$

   ![polynomial function](photos/week%202/02-01.png)

### 2. trigonometric functions
   * $$f(x) = sin(x)$$

   ![trigonometric function](photos/week%202/02-02.png)

### 3. exponential functions
   * $$f(x) = e^x$$

   ![exponential function](photos/week%202/02-03.png)

## Function Definition

* From a set `X` to a set `Y` assigns to each element of `X` exactly one element of `Y`
* In other words, a particular value `x` determines the only value `Y`
* `Domain`: **the set `X` of the function**
* `Codomain`: **the set `y` of the function**
* **A function cannot associate one object in the domain to two different objects in the codomain, but it can associate two objects in the domain to the same object in the codomain**

## Function Description

### Notation
   1. $f: x → x^2$
   2. $f(x) = x^2$
### Graph
1. `Horizontal axis`: the input `x`
2. `Vertical axis`: the output `f(x)`
3. Example: `f(1) = -3`

    ![function graph](photos/week%202/02-03.png)

4. `Local minimum` and `rapid decrease`

    ![local minimum and rapid decrease](photos/week%202/02-04.png)

### Some Special Functions
1. `Floor function`
    * Formula
        $$f(x) = \lfloor x \rfloor$$
    * Graph

        ![floor function graph](photos/week%202/02-05.png)

    * Table

        | x    | floor(x)  |
        | :--: | :-------: |
        | -1   | -1        |
        | -0.5 | -1        |
        | 0    | 0         |
        | 0.5  | 0         |
        | 1    | 1         |

2. `Ceiling function`
    * Formula
        $$f(x) = \lceil x \rceil$$
    * Graph

        ![ceiling function graph](photos/week%202/02-06.png)

    * Table

        | x      | ceiling(x)   |
        | :----: | :---------:  |
        | -1     | -1           |
        | -0.5   | 0            |
        | 0      | 0            |
        | 0.5    | 1            |
        | 1      | 1            |

## Piecewise Function

* A function whose domain is partitioned into several intervals on which the function may be defined differently.
 * These `several intervals` called `subdomains`
 * Example: absolute function
$$
   abs(x) =
   \begin{cases} 
        x & for & x \geq 0\\
        -x & for & x < 0 
    \end{cases}
$$

## Circles

### `Open circle`: 
1. Used for numbers that are less than or greater than (< or >)
2. Indicates the line or curve **doesn't include** the point
### `Close circle`:
1. Used for numbers that are less than or equal to or greater than or equal to ($\leq$ or $\geq$)
2. Indicates the line or curve **includes** the point

## Vertical Test

* It's an easy way to test whether a plane is the graph of a function
* Steps
    1. Draw a vertical line that through a point and the plane
    2. Count the number of intersections of the vertical line and the plane
    3. If the number is more than 1, it isn's;
       otherwise, it's

## Polynomial Function

* It's a function that can be constructed from a variable and a set of numbers, and using only additions and multiplications
* Example: $f(x) = 3x^2 + 6x - 12$
* All the numbers before `x` are `coefficients`
* Example: for the above function, `3`, `6` and `12` are `coefficient`s
* The highest exponents of `x` is `degree`
* Example: for the above function, `2` is `degree`
* If the degree `x` is `much larger than (>>)` or `much less than (<<)`, the function is `asymptotically equivalent (~)` to $a_n*x^n$
* Formula:
    $$
        f(x) =
        a_nx^n + a_{n - 1}x^{n - 1} + \dots + a_1x + a_0\\
        \sim a_nx^n \quad \text {{for}} \quad x \gg 0 \quad \text{{or}} \quad x \ll 0
    $$
* NOTES
    1. Every constant function, like $f(X) = 3$ is one of polynomial function
    2. The exponent of a variable in a polynomial must be a non-negative integer, and functions with negative or fractional exponents aren't polynomial functions

## Polynomial Function Graph

1. Degree 0

    ![degree 0 polynomial function graph](photos/week%202/02-08.png)

2. Degree 1

    ![degree 1 polynomial function graph](photos/week%202/02-09.png)

3. Degree 2
    * Degree 2 Polynomial Function Graph Based On `a`

    ![degree 2 polynomial function graph](photos/week%202/02-10.png)

    * Quadratic Function

    ![degree 2 polynomial function a graph](photos/week%202/02-11.png)

    * Other forms:
        1. `Factorized form`: $f(x) = a(x - p)(x - q)$

        ![factorized form](photos/week%202/02-12.png)

        * ***Not every polynomial can be factored***
        * The polynomial function can be factored ***only if*** $b^2 - 4ac \geq 0$
        2. `Complete-square form`: $f(x) = a(x - r)^2 + s$

        ![complete-square from](photos/week%202/02-13.png)

    * Standard form to complete-square form:
        $$ax^2 + bx + c = a\left(x + \frac {b} {2a}\right)^2 + c - \frac {b^2} {4a}$$
    * Standard form to factorized form
        $$
            ax^2 + bx + c = a(x - p)(x - q)\\
                    \quad = a(x^2 - (p + q)x + pq)\\
        $$
        where
        $$
            p + q = -\frac {b} {a}\\
            pq = \frac {c} {a}
        $$
### Graph Intersects Low
* ***The number of x-axis intersections will be less than or equal to the degree of the polynomial***

![graph intersects low](photos/week%202/02-14.png)

## Rational Function

* It's a function that can be constructed from a variable and a set of numbers, using addition, multiplication and **division**
* To add them, we need to put over a common denominator
    * example:
        $$
        \frac {1} {x - 2} + \frac {1} {x^2 + 2}
        = \frac {x^2 + 2} {(x - 2)(x^2 + 2)} + \frac {x - 2} {(x - 2)(x^2 + 2)}\\
        = \frac {x^2 + x} {(x - 2)(x^2 + 2)}
        $$
### Horizontal Asymptote
* $R(x) = \frac {P(x)} {Q(x)}$
* $R(x)$ represents the rational function
* $P(x)$ represents a polynomial in terms of numerator
* $Q(x)$ represents an another polynomial in terms of denominator
* If $degree(P) \leq degree(Q)$, we should divide by $x^{degree(Q)}$
* example:
    $$
    \frac {2x^2 + 2x - 1} {x^2 + x + 1} = \frac {2 + 2\frac {1} {x} - \frac {1} {x^2}} {1 + \frac {1} {x} + \frac {1} {x^2}}\\
    \sim \frac {2} {1} \quad \text {for large x}\\
    = 2
    $$
* Then the horizontal asymptote is $y = 2$
### Vertical Asymptote
* It can only occur at $Q(x) = 0$ and $P(x) \neq 0$
* Example:
    $$
        f(x) = \frac {1} {x - 2}\\
        Q(x) = x - 2\\
        Q(2) = 0\\
        P(x) \neq 0
    $$
* Then the vertical asymptote is $x = 2$
### Oblique Asymptote
* Example:
![oblique asymptote](photos/week%202/02-15.png)
* As long as we solve a rational function $\sim$ 0, we can identify the corresponding polynomial function as an oblique asymptote
### Zeros of Rational Functions
$$
    \frac {P(x)} {Q(x)} = 0 \quad whenever\\
    P(x) = 0 \quad and \quad Q(x) \neq 0
$$

## Power Function

### Standard Formula
$$f(x) = x^a$$
* `a` is a constant named exponent$$
### Calculation Rules
1. $$x^ax^b = x^{a + b}$$
2. $$\frac {x^a} {x^b} = x^{a - b}$$
3. $$(x^a)^b = x^{ab}$$
4. $$(xy)^a = x^ay^a$$
5. $$x^{\frac {p} {q}} = \sqrt [q] {x^p} = \left(\sqrt [q] {x}\right)^p$$
6. $$x^{-\frac {p} {q}} = \frac {1} {\sqrt [q] {x^p}} = \frac {1} {\left(\sqrt [q] {x}\right)^p}$$
### Power Function With Integer Exponents Graph
1. Non-negative Integer Exponents

    ![non-negative power function graph](photos/week%202/02-16.png)

    * Properties
        1. $$f(-x) = f(x) \quad \text {for even x}$$
        2. $$f(-x) = -f(x) \quad \text {for odd x}$$
2. Negative Integer Exponents

    ![negative power function graph](photos/week%202/02-17.png)

    * Properties
        1. Horizontal asymptote: $x = 0$
        2. Vertical asymptote: $y = 0$
        3. $$f(-x) = f(x) \quad \text {for even x}$$
        4. $$f(-x) = -f(x) \quad \text {for odd x}$$
3. $\frac {1} {n}$ exponent

    ![power function graph](photos/week%202/02-18.png)

### Power Function Comparisons
1. $$x^a < x^b \quad \text {for x > 1 and a < b}$$
2. $$x^a > x^b \quad \text {for 0 < x < 1 and a < b}$$

## Domain, Codomain and Rage

### Domain
1. `Maximal domain`
    * The largest possible domain of the function **from the formula**
    * Example: maximal domain of $f(x) = \sqrt {x}: \quad x \in \mathbb {R}$, because x can be a complex number
2. `Natural domain`
    * The domain of the function in a particular range **from the context**
    * Example: natural domain of $f(x) = \sqrt {x}: \quad x \geq 0$
### Codomain
* A set containing all possible outputs, like $\mathbb {R}$
### Rage
* A set of outputs, like $y \geq 0$

## Continuity

* A small change on the x-axis gives a small change on the y-axis
* Piecewise defined function example

![piecewise defined function](photos/week%202/02-19.png)

### Intermediate Value Property
* If `f` is continuous on $[a, b]$, then it attains all values between $f(a)$ and $f(b)$
* Example

![intermediate value property](photos/week%202/02-20.png)

* continuous functions

![continuous functions](photos/week%202/02-21.png)

## Combining Continuous Functions

* If `f(x)` and `g(x)` are continuous, then
1. $$f(x) + g(x)$$
2. $$f(x) \times g(x)$$
3. $$\frac {f(x)} {g(x)} \quad g(x) \neq 0$$
are also continuous

## Taylor Polynomial

* Best approximates $f(x) = \sqrt {1 + x}$
* The more terms we use, the better the polynomial approximates the function near the chosen point
* Formula:
$$T_n(x) = \sum_{k = 0}^{n} \frac {f^{(k)}(a)} {k!} (x - a)^k$$
* example: $f(x) = \sqrt {1 + x}$ and $x = 0$
$$
f_0(0) = \frac {f(0)} {0!} = \frac {(1 + 0)^{\frac {1} {2}}} {0!} = 1\\
f_1(0) = \frac {f^{'}(0)} {1!} = \frac {\frac {1} {2}(1 + 0)^{-\frac {1} {2}}} {1!} = \frac {1} {2}x\\
f_2(0) = \frac {f^{''}(0)} {2!} = \frac {-\frac {1} {4}(1 + 0)^{-\frac {3} {2}}} {2!} = -\frac {1} {8}x^2\\
f_3(0) = \frac {f^{(3)}(0)} {3!} = \frac {\frac {3} {8}(1 + 0)^{-\frac {5} {2}}} {3!} = \frac {1} {16}x^3\\
\dots\\
\dots\\
\dots\\
$$