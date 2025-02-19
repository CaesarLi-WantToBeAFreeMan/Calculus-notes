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