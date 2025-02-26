# Course #2: Functions Part I

# Platform: Edx

# Teacher: DelftX Calc001x

## unknown kaywords:
| english       | phonetic symbol | chinese meaning |
| :-----------: | :-------------: | :-------------: |
| domain        | doˈmеn          | 定義域           |
| codomain      | ˈkəʊdomеn       | 對應域           |
| continuity    | ˌkɑntǝˈnjuǝtɪ   | 連續性           |
| polynomial    | ˌpɑlɪˈnomɪǝl    | 多項式的         |
| friction      | ˈfrɪkʃǝn        | 摩擦力           |
| trigonometric | ˌtrɪɡǝnǝˈmɛtrɪk | 三角學的         |
| piecewise     | pis waɪz        | 分段            |
| partitioned   | pɑrˈtɪʃǝn       | 分割             |
| asymptotically| еˌsɪmptɑˈtɪkḷɪ  | 漸進            |
| equivalent    | ɪˈkwɪvǝlǝnt     | 等價            |
| slope         | slop            | 斜率            |
| intercept     | ˌɪntɚˈsɛpt      | 截取            |
| factorized    | ˈfæktəˌraɪzd    | 因數的          |
| quadratic     | kwɑdˈrætɪk      | 二次的          |
| vertex        | ˈvɝtɛks         | 頂點            |
| interpret     | ɪnˈtɝprɪt       | 解釋            |
|               |                 |                 |
|               |                 |                 |
|               |                 |                 |
|               |                 |                 |
|               |                 |                 |
|               |                 |                 |
|               |                 |                 |
|               |                 |                 |
|               |                 |                 |
|               |                 |                 |
|               |                 |                 |
|               |                 |                 |
|               |                 |                 |

## standard functions
1. polynomial functions
   * $$f(x) = x^2$$
   * ![polynomial function example photo](photos/polynomial%20function%20example.png)
2. trigonometric functions
   * $$f(x) = sin(x)$$
   * ![trigonometric function example photo](photos/trigonometic%20function%20example.png)
3. exponential functions
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
* notation
   1. $f: x → x^2$
   2. $f(x) = x^2$
* graph
   1. `horizontal axis`: the input `x`
   2. `vertical axis`: the output `f(x)`
   3. example: `f(1) = -3`
      ![function graph example](photos/graph%20notation.png)
   4. `local minimum` and `rapid decrease`
      ![local minimum and rapid decrease example](photos/local%20minimum%20and%20rapid%20decrease%20example.png)
* some special functions
   1. `floor function`
      * formula
      $$f(x) = \lfloor x \rfloor$$
      * graph
      ![floor function graph example](photos/floor%20function%20graph%20example.png)
      * table
      | x    | floor(x)  |
      | :-:  | :-------: |
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
 1. `open circle`: 
   1. is used for numbers that are less than or greater than (`<` or `>`)`
   2. indicates the line or curve **doesn't include** the point
1. `close circle`:
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
* if the degree `x` is `much larger than (>>)` or `much less than (<<)`, the function is `asymptotically equivalent (~)` to *$a_n*x^n$*
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
            * the polynomial function can be factored ***only if $b^2 - 4ac \geq 0$***
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
4. graph intersects low
    * ***The number of x-axis intersections will be less than or equal to the degree of the polynomial***
    ![graph intersects low example](photos/graph%20intersects%20low.png)
5. 