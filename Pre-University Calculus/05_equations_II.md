# Course #5: Equation Part II

# Platform: Edx

# Course Name: DelftX Calc001x: Pre-University Calculus

## unknown keywords

| english       | phonetic symbol | chinese meaning |
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
 
## unknown phrases

## solving strategies

1. substitution
    * we can substitute $\sin(\theta)$ with $x$ in the equation $\sin(\theta)^2 + \sin(\theta) = \frac {1} {2}$
2. using rules
    1.  trigonometric equations
        * we can convert $\sin(\theta)\cos(\theta) = \frac {1} {2}$ into $\frac {1} {2} \sin(2\theta) = \frac {1} {2}$
    2. exponential equations
        * we can convert $2^{x^2 + 3} \times 16^{2x} = 128$ into $2^{x^2 + 8x + 3} = 2^7$
    3. logarithm equations
        * we can convert $\log(x)\log_5(2) = \ln(8)$ into $\frac {\ln(x)\ln(2)} {\ln(10)\ln(5)} = \ln(8)$

## inequalities

### notations
1. $A > B$
    * A is greater than B
2. $A < B$
    * A is less than B
3. $A \geq B$
    * A is greater than or equal to B
4. $A \leq B$
    * A is less than or equal to B
5. $($ or $)$
    * excluding the value
6. $[$ or $]$
    * including the value

### solving strategies
1. find points at which:
    1. both sides are equal
    2. function is not defined, or discontinuous
2. check inequality on each interval
3. check inequality in each boundary point
4. gather to find solution set

## applying a function

### increasing functions
> if you apply an increasing function to both sides of an inequality, then it remains true
* increasing functions
    1. $f(x) = x + c$
    2. $f(x) = cx, \quad \text {with c > 0}$
    3. $f(x) = a^x, \quad \text {with a > 1}$
    4. $f(x) = \log_a(x), \quad \text {with a > 1}$
    5. $f(x) = x^a, \quad \text {a > 0 and x > 0}$
    6. compositions of these functions

### decreasing functions
> if you apply a decreasing function to both sides of an inequality, then the inequality sign flips
* decreasing functions
    1. $f(x) = cx, \quad \text {with c < 0}$
    2. $f(x) = a^x, \quad \text {with 0 < a < 1}$
    3. $f(x) = \log_a(x), \quad \text {with 0 < a < 1}$
    4. $f(x) = x^a, \quad \text {with a < 0 and x > 0}$

## system of equations

### definition
* comprises two or more equations and seeks common solutions to the equations
* example
$$
    \begin{cases}
        x + y = 5\\
        2x - y = 3
    \end{cases}
$$
### elimination method
* it's a method to solve a system of equations
* the solutions of the  system of equations don't change if:
    1. we multiply one or more of the equations by a nonzero constant
    2. we replace an equation by the sum or difference of that equation with one of the other equations
* we need to express  a variable using other variables
* example
1. original system
    $$
        \begin{cases}
            x + y = 5\\
            2x - y = 3
        \end{cases}
    $$
2. add them
    $$x + 2x + y - y = 5 + 3$$
3. simplify
    $$3x = 8$$
4. solve for x
    $$x = \frac {8} {3}$$
5. solve for y
    $$y = 5 - x$$
    $$y = 5 - \frac {8} {3}$$
    $$y = \frac {7} {3}$$