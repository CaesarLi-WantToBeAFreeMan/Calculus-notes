# Course #4: Equation Part I

# Platform: Edx

# Course Name: DelftX Calc001x: Pre-University Calculus

## unknown keywords

| english       | phonetic symbol | chinese meaning |
| :-----------: | :-------------: | :-------------: |
| proton        | ˈprotɑn         | 質子             |
| therapy       | ˈθɛrǝpɪ         | 療法            |
| discriminant  | dɪˈskrɪmənənt   | 判別式          |
| substitution  | ˌsʌbstǝˈtjuʃǝn  | 代換            |
| sophisticated | sǝˈfɪstɪˌkеtɪd  | 複雜的          |
| whereas       | hwɛrˈæz         | 反之            |
| inequality    | ɪnɪˈkwɑlǝtɪ     | 不等式          |
| arch          | ɑrtʃ            | 拱門            |

## unknown phrases

| english       | phonetic symbol   | chinese meaning   |
| :-----------: | :---------------: | :---------------: |
| vice versa    | ˌvaɪs ˈvɚsə       | 反之亦然          |

## polynomial functions

### quadratic functions
1. factorization
    * steps
        1. factorize the function
        2. check the factorization
        3. solve these subfunctions
    * example
        1. factorize the function
            $$2x^2 - x - 3 = 0$$
            $$x \quad 1$$
            $$2x \quad -3$$
        2. check the factorization
            $$-3x + 2x = -x$$
        3. solve these subfunctions
            $$(x + 1)(2x - 3) = 0$$
            $$x_1 = -1 \quad x_2 = \frac {3} {2}$$
2. formula
    $$x = \frac {-b \pm \sqrt{D}} {2a}$$
    $$D = b^2 - 4ac$$
    * `D` for discriminant
| discriminant status   | quantity of solutions         |
| :-------------------: | :---------------------------: |
| D < 0                 | no solution in real numbers   |
| D = 0                 | only one solution             |
| D > 0                 | two different solutions       |
3. complete the square
    * steps
        1. $$a(x - r)^2 = -s$$
        2. $$(x - r)^2 = -\frac {s} {a}$$
        3. $$x - r = \pm \sqrt{-\frac {s} {a}}$$
        4. $$x = r \pm \sqrt{-\frac {s} {a}}$$
    * example
        $$x^2 + 4x + 1 = 0$$
        1. first step
            $$-2r = 4 \rightarrow r = -2$$
            $$(x + 2)^2 - (-2)^2 + 1 = 0$$
            $$(x + 2)^2 = 3$$
        2. second step
            $$(x + 2)^2 = 3$$
        3. third step
            $$x + 2 = \pm \sqrt{3}$$
        4. fourth step
            $$x = -2 \pm \sqrt{3}$$
### degree more than 2
* properties
    1. For odd degree, the function has at least **1** solution
    2. For even degree, the function may have **no** solution
    3. For degree `n`, the function has at most **n** solutions
* divide the function
    * We can divide the function into many subfunctions, each of which has a degree less than or equal to 2
    * example:
        $$x^3 - 7x + 6$$
        1. guess a solution
            $$x = 1$$
            $$1^3 - 7 + 6 = 0$$
        2. divide the function
            $$(x - 1)(x^2 + x - 6)$$
            $$(x - 1)(x + 3)(x - 2) = 0$$
        3. solve the subfunctions
            $$x_1 = -3, x_2 = 1, x_3 = 2$$

## rational functions

* steps
    1. Multiply by a common denominator
    2. Solve polynomial equation
    3. Check results
* example
    $$\frac {x} {x - 2} + \frac {x} {x + 2} = 3$$
    1. multiply by a common denominator
        $$x(x + 2) + x(x - 2) = 3(x - 2)(x + 2)$$
        $$x^2 - 12 = 0$$
    2. solve polynomial equation
        $$x^2 = 12$$
        $$x^2 = \pm \sqrt{12}$$
        $$x_1 = 2\sqrt{3}, x_2 = -2\sqrt{3}$$
    3. check results
        $$\frac {2\sqrt{3}} {2\sqrt{3} - 2} + \frac {2\sqrt{3}} {2\sqrt{3} + 2} = 3$$
        $$\frac {-2\sqrt{3}} {-2\sqrt{3} - 2} + \frac {-2\sqrt{3}} {-2\sqrt{3} + 2} = 3$$

## strategies of simplifying

### 1. balanced method
* performing the same operation on both the left and right sides, e.g., addition, subtraction, multiplication, division, exponentiation, root operations, etc
### 2. factorization
* factorizing an expression, such as factorizing $x^2 + 2x - 15 = 0$ into $(x - 3)(x + 5) = 0$
### 3. substitution
* for $x^6 - 3x^3 - 4 = 0$, we can substitute $y = x^3$, and then simplify the expression as $y^2 - 3x - 4 = 0$

## complex numbers

### definition
* `i` is an **imaginary** number such that $i^2 = -1$
* `z = x + yi` with `x` and `y`  real is called `complex number`
* `x = Rez` is called the `real part` of `z`
* `y = Imz` is called the `imaginary part` of `z`
### calculation rules
1. addition
    $$(x_1 + y_1i) + (x_2 + y_2i) =$$
    $$[x_1 + x_2 + (y_1 + y_2)i]$$
2. subtraction
    $$(x_1 + y_1i) - (x_2 + y_2i) =$$
    $$[x_1 - x_2 + (y_1 - y_2)i]$$
3. multiplication
    $$(x_1 + y_1i)(x_2 + y_2i) =$$
    $$x_1 \times x_2 + (x_1 \times y_2)i + (y_1 \times x_2)i + (y_1 \times y_2)i^2 =$$
    $$[x_1 \times x_2 - (y_1 \times y_2) + (x_1 \times y_2 + y_1 \times x_2)i]$$
4. division
    $$\frac {x_1 + y_1i} {x_2 + y_2i} =$$
    $$\frac {x_1 + y_1i} {x_2 + y_2i} \times \frac {x_2 + -y_2i} {x_2 + -y_2i} =$$
    $$\frac {x_1 \times x_2 - (x_1 \times y_2)i + (y_1 \times x_2)i - (x_2 \times y_2)i^2} {2_1^2 - (y_2i)^2} =$$
    $$\frac {x_1 \times x_2 + y_1 \times y_2} {x_2^2 + y_2^2} + \frac {y_1 \times x_2 - x_1 \times y_2} {x_2^2 + y_2^2}i