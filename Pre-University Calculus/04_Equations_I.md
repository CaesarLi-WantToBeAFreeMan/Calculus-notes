# Course #4: Equation Part I

# Platform: Edx

# Course Name: DelftX Calc001x: Pre-University Calculus

# Author: Caesar James LEE

## Unknown Keywords

| English       | Pronunciation   | Chinese Meaning |
| :-----------: | :-------------: | :-------------: |
| proton        | ˈprotɑn         | 質子             |
| therapy       | ˈθɛrǝpɪ         | 療法            |
| discriminant  | dɪˈskrɪmənənt   | 判別式          |
| substitution  | ˌsʌbstǝˈtjuʃǝn  | 代換            |
| sophisticated | sǝˈfɪstɪˌkеtɪd  | 複雜的          |
| whereas       | hwɛrˈæz         | 反之            |
| inequality    | ɪnɪˈkwɑlǝtɪ     | 不等式          |
| arch          | ɑrtʃ            | 拱門            |

## Unknown Phrases

| Phrase        | Pronunciation     | Chinese Meaning   |
| :-----------: | :---------------: | :---------------: |
| vice versa    | ˌvaɪs ˈvɚsə       | 反之亦然          |

## Polynomial Functions

### Quadratic Functions
1. Factorization
    * Steps
        1. Factorize the function
        2. Check the factorization
        3. Solve these subfunctions
    * Example
        1. Factorize the function
            $$2x^2 - x - 3 = 0$$
            $$x \quad 1$$
            $$2x \quad -3$$
        2. Check the factorization
            $$-3x + 2x = -x$$
        3. Solve these subfunctions
            $$(x + 1)(2x - 3) = 0$$
            $$x_1 = -1 \quad x_2 = \frac {3} {2}$$
2. Formula
    $$x = \frac {-b \pm \sqrt{D}} {2a}$$
    $$D = b^2 - 4ac$$
    * `D` for discriminant
| Discriminant Status   | Quantity of Solutions         |
| :-------------------: | :---------------------------: |
| D < 0                 | no solution in real numbers   |
| D = 0                 | only one solution             |
| D > 0                 | two different solutions       |
3. Complete The Square
    * Steps
        1. $$a(x - r)^2 = -s$$
        2. $$(x - r)^2 = -\frac {s} {a}$$
        3. $$x - r = \pm \sqrt{-\frac {s} {a}}$$
        4. $$x = r \pm \sqrt{-\frac {s} {a}}$$
    * Example
        $$x^2 + 4x + 1 = 0$$
        1. First step
            $$-2r = 4 \rightarrow r = -2$$
            $$(x + 2)^2 - (-2)^2 + 1 = 0$$
            $$(x + 2)^2 = 3$$
        2. Second step
            $$(x + 2)^2 = 3$$
        3. Third step
            $$x + 2 = \pm \sqrt{3}$$
        4. Fourth step
            $$x = -2 \pm \sqrt{3}$$
### Degree More Than 2
* Properties
    1. For odd degree, the function has at least **1** solution
    2. For even degree, the function may have **no** solution
    3. For degree `n`, the function has at most **n** solutions
* Divide The Function
    * We can divide the function into many subfunctions, each of which has a degree less than or equal to 2
    * Example:
        $$x^3 - 7x + 6$$
        1. Guess a solution
            $$x = 1$$
            $$1^3 - 7 + 6 = 0$$
        2. Divide the function
            $$(x - 1)(x^2 + x - 6)$$
            $$(x - 1)(x + 3)(x - 2) = 0$$
        3. Solve the subfunctions
            $$x_1 = -3, x_2 = 1, x_3 = 2$$

## Rational Functions

* Steps
    1. Multiply by a common denominator
    2. Solve polynomial equation
    3. Check results
* Example
    $$\frac {x} {x - 2} + \frac {x} {x + 2} = 3$$
    1. Multiply by a common denominator
        $$x(x + 2) + x(x - 2) = 3(x - 2)(x + 2)$$
        $$x^2 - 12 = 0$$
    2. Solve polynomial equation
        $$x^2 = 12$$
        $$x^2 = \pm \sqrt{12}$$
        $$x_1 = 2\sqrt{3}, x_2 = -2\sqrt{3}$$
    3. Check results
        $$\frac {2\sqrt{3}} {2\sqrt{3} - 2} + \frac {2\sqrt{3}} {2\sqrt{3} + 2} = 3$$
        $$\frac {-2\sqrt{3}} {-2\sqrt{3} - 2} + \frac {-2\sqrt{3}} {-2\sqrt{3} + 2} = 3$$

## Strategies of Simplifying

### 1. Balanced Method
* Performing the same operation on both the left and right sides, e.g., addition, subtraction, multiplication, division, exponentiation, root operations, etc
### 2. Factorization
* Factorizing an expression, such as factorizing $x^2 + 2x - 15 = 0$ into $(x - 3)(x + 5) = 0$
### 3. Substitution
* For $x^6 - 3x^3 - 4 = 0$, we can substitute $y = x^3$, and then simplify the expression as $y^2 - 3x - 4 = 0$

## Complex Numbers

### Definition
* `i` is an **imaginary** number such that $i^2 = -1$
* `z = x + yi` with `x` and `y`  real is called `complex number`
* `x = Rez` is called the `real part` of `z`
* `y = Imz` is called the `imaginary part` of `z`
### Calculation Rules
1. Addition
    $$(x_1 + y_1i) + (x_2 + y_2i) = [x_1 + x_2 + (y_1 + y_2)i]$$
2. Subtraction
    $$(x_1 + y_1i) - (x_2 + y_2i) = [x_1 - x_2 + (y_1 - y_2)i]$$
3. Multiplication
    $$
    (x_1 + y_1i)(x_2 + y_2i) = x_1 \times x_2 + (x_1 \times y_2)i + (y_1 \times x_2)i + (y_1 \times y_2)i^2\\
    = [x_1 \times x_2 - (y_1 \times y_2) + (x_1 \times y_2 + y_1 \times x_2)i]
    $$
4. Division
    $$
    \frac {x_1 + y_1i} {x_2 + y_2i} = \frac {x_1 + y_1i} {x_2 + y_2i} \times \frac {x_2 + -y_2i} {x_2 + -y_2i}\\
    = \frac {x_1 \times x_2 - (x_1 \times y_2)i + (y_1 \times x_2)i - (x_2 \times y_2)i^2} {2_1^2 - (y_2i)^2}\\
    = \frac {x_1 \times x_2 + y_1 \times y_2} {x_2^2 + y_2^2} + \frac {y_1 \times x_2 - x_1 \times y_2} {x_2^2 + y_2^2}i
    $$