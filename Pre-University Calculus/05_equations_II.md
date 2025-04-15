# Course #5: Equation Part II

# Platform: Edx

# Course Name: DelftX Calc001x: Pre-University Calculus

# Author: Caesar James LEE

## Unknown Keywords

| English       | Pronunciation   | Chinese Meaning |
| :-----------: | :-------------: | :-------------: |
| G-force       | dʒi fors        | G力，移動或改變切線，或是加速度與減速度時承受力道的單位 |
| comprise      | kǝmˈpraɪz       | 包含            |
| elimination   | ɪˌlɪmǝˈnеʃǝn    | 排除            |
| papyrus       | pǝˈpaɪrǝs       | 紙莎草          |
| fragment      | ˈfræɡmǝnt       | 碎片            |
| hebrew        | ˈhibru          | 希伯來人        |
| canon         | ˈkænǝn          | 教規            |
| Testament     | ˈtɛstǝmǝnt      | 聖經舊約        |
| inclined      | ɪnˈklaɪnd       | 傾斜的          |
| magnitude     | ˈmæɡnǝˌtjud     | 巨大            |
| parallel      | ˈpærǝˌlɛl       | 平行的          |
| perpendicular | ˌpɝpǝnˈdɪkjǝlɚ  | 垂直的          |
 
## Solving Strategies

1. Substitution
    * We can substitute $\sin(\theta)$ with $x$ in the equation $\sin(\theta)^2 + \sin(\theta) = \frac {1} {2}$
2. Using Rules
    1.  Trigonometric equations
        * we can convert $\sin(\theta)\cos(\theta) = \frac {1} {2}$ into $\frac {1} {2} \sin(2\theta) = \frac {1} {2}$
    2. Exponential equations
        * we can convert $2^{x^2 + 3} \times 16^{2x} = 128$ into $2^{x^2 + 8x + 3} = 2^7$
    3. Logarithm equations
        * we can convert $\log(x)\log_5(2) = \ln(8)$ into $\frac {\ln(x)\ln(2)} {\ln(10)\ln(5)} = \ln(8)$

## Inequalities

### Notations
1. $A > B$
    * `A` is greater than `B`
2. $A < B$
    * `A` is less than `B`
3. $A \geq B$
    * `A` is greater than or equal to `B`
4. $A \leq B$
    * `A` is less than or equal to `B`
5. $($ or $)$
    * Excluding the value
6. $[$ or $]$
    * Including the value

### Solving Strategies
1. Find points at which:
    1. Both sides are equal
    2. Function is not defined, or discontinuous
2. Check inequality on each interval
3. Check inequality in each boundary point
4. Gather to find solution set

## Applying A Function

### Increasing Functions
> If you apply an increasing function to both sides of an inequality, then it remains true
* Increasing functions
    1. $f(x) = x + c$
    2. $f(x) = cx, \quad \text {with c > 0}$
    3. $f(x) = a^x, \quad \text {with a > 1}$
    4. $f(x) = \log_a(x), \quad \text {with a > 1}$
    5. $f(x) = x^a, \quad \text {a > 0 and x > 0}$
    6. Compositions of these functions

### Decreasing Functions
> If you apply a decreasing function to both sides of an inequality, then the inequality sign flips
* Decreasing functions
    1. $f(x) = cx, \quad \text {with c < 0}$
    2. $f(x) = a^x, \quad \text {with 0 < a < 1}$
    3. $f(x) = \log_a(x), \quad \text {with 0 < a < 1}$
    4. $f(x) = x^a, \quad \text {with a < 0 and x > 0}$

## System of Equations

### Definition
* Comprises two or more equations and seeks common solutions to the equations
* Example
$$
    \begin{cases}
        x + y = 5\\
        2x - y = 3
    \end{cases}
$$
### Elimination Method
* It's a method to solve a system of equations
* The solutions of the  system of equations don't change if:
    1. We multiply one or more of the equations by a nonzero constant
    2. We replace an equation by the sum or difference of that equation with one of the other equations
* We need to express  a variable using other variables
* Example
1. Original system
    $$
        \begin{cases}
            x + y = 5\\
            2x - y = 3
        \end{cases}
    $$
2. Add them
    $$x + 2x + y - y = 5 + 3$$
3. Simplify
    $$3x = 8$$
4. Solve for x
    $$x = \frac {8} {3}$$
5. Solve for y
    $$y = 5 - x$$
    $$y = 5 - \frac {8} {3}$$
    $$y = \frac {7} {3}$$