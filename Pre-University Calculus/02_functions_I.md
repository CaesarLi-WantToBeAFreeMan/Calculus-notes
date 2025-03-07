# Course #1: Functions Part I

# Platform: Edx

# Course Name: DelftX Calc001x: Pre-University Calculus

## unknown keywords:
| english       | phonetic symbol | chinese meaning |
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

## unknown abbreviations:

| abbreviation  | full name         | chinese meaning |
| :-----------: | :---------------: | :-------------: |
| LHS           | Left-Hand Side    | 左側的式子       |
| RHS           | Right-Hand Side   | 右側的式子       |

## standard functions

### 1. polynomial functions
   * $$f(x) = x^2$$
   * ![polynomial function example photo](photos/polynomial%20function%20example.png)
### 2. trigonometric functions
   * $$f(x) = sin(x)$$
   * ![trigonometric function example photo](photos/trigonometic%20function%20example.png)
### 3. exponential functions
   * $$f(x) = e^x$$
   * ![exponential function example photo](photos/exponential%20function%20example.png)

## function definition

* from a set `X` to a set `Y` assigns to each element of `X` exactly one element of `Y`
* in other words, a particular value `x` determines the only value `y`
* `domain`: **the set `X` of the function**
* `codomain`: **the set `y` of the function**
* **a function cannot associate one object in the domain to two different objects in the codomain**
* **but it can associate two objects in the domain to the same object in the codomain**

## function description

### notation
   1. $f: x → x^2$
   2. $f(x) = x^2$
### graph
1. `horizontal axis`: the input `x`
2. `vertical axis`: the output `f(x)`
3. example: `f(1) = -3`
    ![function graph example](photos/graph%20notation.png)
4. `local minimum` and `rapid decrease`
    ![local minimum and rapid decrease example](photos/local%20minimum%20and%20rapid%20decrease%20example.png)
### some special functions
1. `floor function`
    * formula
        $$f(x) = \lfloor x \rfloor$$
    * graph

        ![floor function graph example](photos/floor%20function%20graph%20example.png)

    * table

        | x    | floor(x)  |
        | :--: | :-------: |
        | -1   | -1        |
        | -0.5 | -1        |
        | 0    | 0         |
        | 0.5  | 0         |
        | 1    | 1         |

2. `ceiling function`
    * formula
        $$f(x) = \lceil x \rceil$$
    * graph

        ![ceiling function graph example](photos/ceiling%20function%20graph%20example.png)

    * table

        | x      | ceiling(x)   |
        | :----: | :---------:  |
        | -1     | -1           |
        | -0.5   | 0            |
        | 0      | 0            |
        | 0.5    | 1            |
        | 1      | 1            |

## piecewise function

* a function whose domain is partitioned into several intervals on which the function may be defined differently.
 * these `several intervals` called `subdomains`
 * example: absolute function
$$
   abs(x) = \begin{cases} 
            x & for & x \geq 0\\
            -x & for & x < 0 
            \end{cases}
$$

## open and close circles

### `open circle`: 
1. is used for numbers that are less than or greater than (< or >`)
2. indicates the line or curve **doesn't include** the point
### `close circle`:
1. is used for numbers that are less than or equal to or greater than or equal to ($\leq$ or $\geq$)
2. indicates the line or curve **includes** the point

## vertical test

* it's an easy way to test whether a plane is the graph of a function
* steps
    1. draw a vertical line that through a point and the plane
    2. count the number of intersections of the vertical line and the plane
    3. if the number is more than 1, it isn's;
       otherwise, it's

## polynomial function

* It's a function that can be constructed from a variable and a set of numbers, and using only additions and multiplications
* example: $f(x) = 3x^2 + 6x - 12$
* All the numbers before `x` are `coefficients`
* example: for the above function, `3`, `6` and `12` are `coefficient`s
* The highest exponents of `x` is `degree`
* example: for the above function, `2` is `degree`
* if the degree `x` is `much larger than (>>)` or `much less than (<<)`, the function is `asymptotically equivalent (~)` to $a_n*x^n$
* formula:
    $$
        f(x) = a_nx^n + a_{n - 1}x^{n - 1} + \dots + a_1x + a_0\\
            \sim a_nx^n \quad \text {{for}} \quad x \gg 0 \quad \text{{or}} \quad x \ll 0
    $$
* NOTES
    1. Every constant function, like $f(X) = 3$ is one of polynomial function
    2. The exponent of a variable in a polynomial must be a non-negative integer, and functions with negative or fractional exponents aren't polynomial functions

## polynomial function graph

1. degree 0
    ![degree 0 polynomial function graph](photos/degree%200%20graph%20example.png)
2. degree 1
    ![degree 1 polynomial function graph](photos/degree%201%20graph%20example.png)
3. degree 2
    ![degree 2 polynomial function graph](photos/degree%202%20graph%20example.png)
    a functions
    ![degree 2 polynomial function a graph](photos/degree%202%20a%20graph%20example.png)
    * other forms:
        1. `factorized form`: $f(x) = a(x - p)(x - q)$
        ![factorized form graph](photos/factorized%20form.png)
            * ***not every polynomial can be factored***
            * the polynomial function can be factored ***only if*** $b^2 - 4ac \geq 0$
        2. `complete-square form`: $f(x) = a(x - r)^2 + s$
        ![complete-square from graph](photos/complete-aquare%20form.png)
    * standard form to complete-square form:
        $$ax^2 + bx + c = a\left(x + \frac {b} {2a}\right)^2 + c - \frac {b^2} {4a}$$
    * standard form to factorized form
        $$
            ax^2 + bx + c = a(x - p)(x - q)\\
                    \quad = a(x^2 - (p + q)x + pq)\\
        $$
        $$
            p + q = -\frac {b} {a}\\
            pq = \frac {c} {a}
        $$
### graph intersects low
* ***The number of x-axis intersections will be less than or equal to the degree of the polynomial***
![graph intersects low example](photos/graph%20intersects%20low.png)

## rational function

* It's a function that can be constructed from a variable and a set of numbers, using addition, multiplication and **division**
* To add them, we need to put over a common denominator
    * example:
        $$
            \frac {1} {x - 2} + \frac {1} {x^2 + 2}
            = \frac {x^2 + 2} {(x - 2)(x^2 + 2)} + \frac {x - 2} {(x - 2)(x^2 + 2)}\\
            \quad = \frac {x^2 + x} {(x - 2)(x^2 + 2)}
        $$
### horizontal asymptote
* $R(x) = \frac {P(x)} {Q(x)}$

    * $R(x)$ represents the rational function

    * $P(x)$ represents a polynomial in terms of numerator

    * $Q(x) represents an another polynomial in terms of denominator
* If $degree(P) \leq degree(Q)$, we should divide by $x^{degree(Q)}$
* example:
    $$
        \frac {2x^2 + 2x - 1} {x^2 + x + 1} = \frac {2 + 2\frac {1} {x} - \frac {1} {x^2}} {1 + \frac {1} {x} + \frac {1} {x^2}}
    $$
    $$
        \sim \frac {2} {1} \quad \text {for large x}
    $$
    $$
        = 2
    $$
* Then the horizontal asymptote is $y = 2$
### vertical asymptote
* It can only occur at $Q(x) = 0$ and $P(x) \neq 0$
* example:
    $$
        f(x) = \frac {1} {x - 2}
    $$
    $$
        Q(x) = x - 2
    $$
    $$
        Q(2) = 0
    $$
    $$
        P(x) \neq 0
    $$
* Then the vertical asymptote is $x = 2$
### oblique asymptote
* example:
![oblique asymptote example](photos/oblique%20asymptote.png)
* As long as we solve a rational function $\sim$ 0, we can identify the corresponding polynomial function as an oblique asymptote
### zeros of rational functions
$$
    \frac {P(x)} {Q(x)} = 0 \quad whenever
$$
$$
    P(x) = 0 \quad and \quad Q(x) \neq 0
$$

## power function

### standard formula
$$f(x) = x^a \quad \text {a is a constant named exponent}$$
### calculation rules
1. $$x^ax^b = x^{a + b}$$
2. $$\frac {x^a} {x^b} = x^{a - b}$$
3. $$(x^a)^b = x^{ab}$$
4. $$(xy)^a = x^ay^a$$
5. $$x^{\frac {p} {q}} = \sqrt [q] {x^p} = \left(\sqrt [q] {x}\right)^p$$
6. $$x^{-\frac {p} {q}} = \frac {1} {\sqrt [q] {x^p}} = \frac {1} {\left(\sqrt [q] {x}\right)^p}$$
### power function with integer exponents graph
1. non-negative integer exponents
    ![power function graph](photos/power%20function%20graphs%20for%20non-negative%20integer%20x.png)
    * properties
        1. $$f(-x) = f(x) \quad \text {for even x}$$
        2. $$f(-x) = -f(x) \quad \text {for odd x}$$
2. negative integer exponents
    ![power function graph](photos/power%20function%20graphs%20for%20negative%20integer%20x.png)
    * properties
        1. horizontal asymptote: $x = 0$
        2. vertival asymptote: $y = 0$
        3. $$f(-x) = f(x) \quad \text {for even x}$$
        4. $$f(-x) = -f(x) \quad \text {for odd x}$$
3. $\frac {1} {n}$ exponent
    ![power function graph](photos/power%20function%20graphs%20for%20dividing%20by%20n.png)
### power function comparisons
1. $$x^a < x^b \quad \text {for x > 1 and a < b}$$
2. $$x^a > x^b \quad \text {for 0 < x < 1 and a < b}$$

## domain, codomain and rage

### domain
1. `maximal domain`
    * The largest possible domain of the function **from the formula**
    * example: maximal domain of $f(x) = \sqrt {x}: \quad x \in \mathbb {R}$, because x can be a complex number
2. `natural domain`
    * The domain of the function in a particular range **from the context**
    * example: natural domain of $f(x) = \sqrt {x}: \quad x \geq 0$
### codomain
* A set containing all possible outputs, like $\mathbb {R}$
### rage
* A set of outputs, like $y \geq 0$

## continuity

* A small change on the x-axis gives a small change on the y-axis
* piecewise defined function example
![piecewise defined function example](photos/piecewise%20defined%20function%20example.png)
### intermediate value property
* If `f` is continuous on $[a, b]$, then it attains all values between $f(a)$ and $f(b)$
* example
![intermediate value property example](photos/intermediate%20value%20property%20example.png)
* continuous functions
![continuous functions](photos/continuous%20functions.png)

## combining continuous functions

* if `f(x)` and `g(x)` are continuous, then
$$f(x) + g(x)$$
$$f(x) \times g(x)$$
$$\frac {f(x)} {g(x)} \quad g(x) \neq 0$$
are also continuous

## Taylor polynomial

* Best approximates $f(x) = \sqrt {1 + x}$
* The more terms we use, the better the polynomial approximates the function near the chosen point
* Formula:
$$T_n(x) = \sum_{k = 0}^{n} \frac {f^{(k)}(a)} {k!} (x - a)^k$$
* example: $f(x) = \sqrt {1 + x}$ and $x = 0$
$$f_0(0) = \frac {f(0)} {0!} = \frac {(1 + 0)^{\frac {1} {2}}} {0!} = 1$$
$$f_1(0) = \frac {f^{'}(0)} {1!} = \frac {\frac {1} {2}(1 + 0)^{-\frac {1} {2}}} {1!} = \frac {1} {2}x$$
$$f_2(0) = \frac {f^{''}(0)} {2!} = \frac {-\frac {1} {4}(1 + 0)^{-\frac {3} {2}}} {2!} = -\frac {1} {8}x^2$$
$$f_3(0) = \frac {f^{(3)}(0)} {3!} = \frac {\frac {3} {8}(1 + 0)^{-\frac {5} {2}}} {3!} = \frac {1} {16}x^3$$
$$.$$
$$.$$
$$.$$