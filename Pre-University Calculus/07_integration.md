# Course #7: Integration

# Platform: Edx

# Course Name: DelftX Calc001x: Pre-University Calculus

## unknown keywords

| english           | phonetic symbol   | chinese meaning |
| :---------------: | :---------------: | :-------------: |
| integration       | ˌɪntǝˈɡrеʃǝn      | 積分            |
| accumulation      | ǝˌkjumjǝˈlеʃǝn    | 積累            |
| integral          | ˈɪntǝɡrǝl         | 積分的；積分     |
| antiderivative    | ˈæntɪ dǝˈrɪvǝtɪv  | 反導函數         |
| density           | ˈdɛnsǝtɪ          | 密度             |
| blade             | blеd              | 刀片；葉片       |
| geostationary     | ˌdʒioˈstеʃǝˌnɛrɪ  | 與地球旋轉同步的 |
| counteract        | ˌkaʊntɚˈækt       | 對……起反作用    |
| meteorological    | ˌmitɪǝrǝˈlɑdʒɪkḷ  | 氣象的         |
| radioactive       | ˌrеdɪoˈæktɪv      | 放射性的        |
| decay             | dɪˈkе             | 腐爛；蛻變      |
| uranium           | jʊˈrеnɪǝm         | 鈾             |
| slice             | slaɪs             | 薄片；部分     |
| peer              | pɪr               | （地位，能力等）同等的人  |

## definition

* Integration is a reverse process of differentiation, which combines these changes to find the accumulation over an interval
* In other words, integration calculates the accumulated total or area under a curve; differentiation calculates the rate of change or slope of a function
### formula
$$\int_a^bf(x)dx$$
### formula meaning
* It's an signed area of region between `graph`, `x-axis` and line `x = a` and `x = b`

## Riemann Sum

### definition
* It's a method to approximate the area under a curve
* It divides the area into a lot of rectangles
* You can approximate the area under a curve by adding the sum of these rectangles
* photo
![Riemann Sum photo](photos/riemann%20sum%20photo.png)

### formula
$$\int_a^b f(x)dx \approx \sum_{i = 1}^n f(x_i^*) \Delta x$$

* where
    1. $[a, b]$ is the interval of the integration
    2. $n$ is the number of subintervals (rectangles), or your calculation times
    3. $\Delta x = \frac {b - a} {n}$ is the width of each rectangle
    4. $x_i^*$ is a simple point in the i-th subinterval (usually midpoint)
    5. $f(x_i^*) \Delta x$ is the area of a rectangle

### example $\int_0^1 e^{-x^2}$
1. select $n = 4$
2. $\Delta x = \frac {1 - 0} {4} = 0.25$
3. calculate midpoints:

| subinterval   | interval      | midpoint                      |
| :-----------: | :-----------: | :---------------------------: |
| 1             | [0, 0.25]     | $\frac {0 + 0.25} {2} = 0.125$ |
| 2             | [0.25, 0.5]   | $\frac {0.25 + 0.5} {2} = 0.325$ |
| 3             | [0.5, 0.75]   | $\frac {0.5 + 0.75} {2} = 0.625$ |
| 4             | [0.75, 1]     | $\frac {0.75 + 1} {2} = 0.875$ |

4. $\approx 0.25(f(0.125) + f(0.375) + f(0.625) + f(0.875))$
5. $\approx 0.25(e^{-(0.125)^2} + e^{-(0.375)^2} + e^{-(0.625)^2} + e^{-(0.875)^2})$
6. $\approx 0.25(0.985 + 0.869 + 0.678 + 0.465)$
7. $\approx 0.749$

## integral rules

### fundamental theorem
$$\int_b^af(x)dx = F(b) - F(a)$$
where,
1. `f` is a continuous function on the interval [a, b]
2. `F` function such that `F'(x) = f`
3. `F` called `primitive function or antiderivative of f`
### calculation process
$$\int_1^2 x^2dx = [\frac {1} {3}x^3]_1^2$$
$$= \frac {1} {3}2^3-\frac {1} {3}1^3$$
$$= \frac {7} {3}$$


### basic standard integrations
| function                              | integral                                  |
| :-----------------------------------: | :---------------------------------------: |
| BASIC                                 | BASIC                                     |
| $\int adx$                            | $ax + C$                                  |
| $\int x^adx, \quad x \neq -1$         | $\frac {x^{a + 1}} {a + 1} + C$           |
| $\int x^{-1}dx$                       | $\ln(\lvert x \rvert) + C$                |
| LOGARITHM AND EXPONENTIAL             | LOGARITHM AND EXPONENTIAL                 |
| $\int e^xdx$                          | $e^x + C$                                 |
| $\int a^xdx$                          | $\frac {a^x} {\ln(a)} + C$                |
| TRIGONOMETRIC                         | TRIGONOMETRIC                             |
| $\int \sin(x)dx$                      | $-\cos(x) + C$                            |
| $\int \cos(x)dx$                      | $\sin(x) + C$                             |
| $\int \tan(x)dx$                      | $-\ln(\lvert \cos(x) \rvert) + C$         |
| $\int \cot(x)dx$                      | $\ln(\lvert \sin(x) \rvert) + C$          |
| $\int \sec^2(x)dx$                    | $\tan(x) + C$                             |
| $\int \csc^2(x)dx$                    | $-\cot(x) + C$                            |
| $\int \sec(x)\tan(x)dx$               | $\sec(x) + C$                             |
| $\int \csc(x)\cot(x)dx$               | $-\csc(x) + C$                            |
| $\int \frac {dx} {\sqrt{1 - x^2}}$    | $\arcsin(x) + C$                          |
| $\int \frac {dx} {\sqrt{a^2 - x^2}}$  | $\arcsin(\frac {x} {a}) + C$              |
| $\int \frac {dx} {1 + x^2}$           | $\arctan(x) + C$                          |
| $\int \frac {dx} {a^x + x^2}$         | $\frac {1} {a} \arctan(\frac {x} {a} + C$ |
### calculation rules
| calculation               | derivative                            |
| :-----------------------: | :-----------------------------------: |
| $\int af(x)dx$            | $a\int f(x)dx$                        |
| $\int [f(x) \pm g(x)]dx$  | $\int f(x)dx \pm \int g(x)dx$         |
### other rules
1. $$\int_0^0 f(x)dx = 0$$
2. $$\int_b^a f(x)dx = -\int_a^b f(x)dx$$
3. $$\int_b^a f(x)dx = \int_c^b f(x)dx + \int_b^a f(x)dx, \quad a > b$$
4. $$\int_a^b f(x + c)dx = \int_{a + c}^{b + c}f(x)dx$$
5. $$\int_a^b f(cx)dx = \int_{ca}^{cb} \frac {1} {c}f(x)dx$$
### combinations
* There's no one general method to solve all combinations
1. substitution without boundary
    * $$\int f(x)dx = \int f(u)du$$
    * example 1
        * $$\int \cos(x^3 + 5x)(3x^2 + 5)dx$$
        * steps
            1. $u = x^3 + 5x$
            3. $du = (3x^2 + 5)dx$
            4. $F(u) = sin(u)$
            5. $\int \cos(x^3 + 5x)(3x^2 + 5)dx = \sin(u) + C$
            6. $$= \sin(x^3 + 5x) + C$$
    * example 2
        * $$\int \frac {1} {1 + x^3}x^2dx$$
        * steps
            1. $u = 1 + x^3$
            2. $du = 3x^2dx$
            3. $F(u) = \ln(\lvert u \rvert)$
            4. $\int \frac {1} {1 + x^3}x^2dx = \frac {1} {3} \ln(\lvert u \rvert) + C$
            5. $$= \frac {1} {3} \ln(\lvert 1 + x^3 \rvert) + C$$
2. substitution with boundary
    * $$\int_b^a f(x)dx = \int_{u(b)}^{u(a)} f(u)du$$
    * example
        * $$\int_1^2 2xe^{3 + x^2}dx$$
        * steps
            1. $u = 3 + x^2$
            2. $du = 2x$
            3. $\int_1^2 2xe^{3 + x^2}dx = \int_{3 + 1^2}^{3 + 2^2}e^udu$
            4. $$= e^7 - e^4$$
3. integration by parts
    * $$\int udv = uv - \int vdu$$
    * example
        * $$\int x^2\sin(x)dx$$
        * steps
            1. $u = x^2, v' = \sin(x)$
            2. $du = 2x, v = -\cos(x)$
            3. $= x^2 \times -\cos(x) - \int (-\cos(x) \times 2x)dx$
            4. $=-x^2 \cos(x) + 2 \int x \cos(x)dx$
            5. $u = x, v' = \cos(x)$
            6. $du = 1, v = \sin(x)$
            7. $=-x^2 \cos(x) + 2(x \sin(x) - \int (\sin(x) \times 1) dx)$
            8. $=-x^2 \cos(x) + 2(x \sin(x) + \cos(x))$
            9. = $-x^2 \cos(x) + 2x \sin(x) + 2 \cos(x) + C$

## applications

### 1. mass
* basic concepts
    $$\rho = \frac {m} {V}$$
    * **density** ($\rho$) is a substance's **mass** ($m$) per unit of **volume** ($V$)
* solution
    $$m = [\rho(x)dx]^a_b$$
    * example: blade
    * $\rho(x) = \frac {5} {1 + 5x} - \frac {5} {6}$
    * $m = [\ln(1 + 5x) - \frac {5x} {6}]^a_b$

### 2. work
* basic concepts
    $$W = F \times s$$
    * **work** ($W$) is the energy transferred to or from an object via the application of **force** ($F$) along a **displacement** ($s$)
* solution
    $$W = [F(s)ds]^a_b$$
    * example: launch a satellite
    * $$F(s) = \frac {6,371^2} {(s + 6,371)^2}mg$$
    * where
        1. $6,371$ is the radius of Earth in kilometers
        2. $s$ is the height of the satellite
        3. $m$ is the satellite's mass
        4. $g$ is the gravitational acceleration of Earth
    * $W = [-\frac {9.81 \times (6,371 \times 10^3)^2 \times 2,000} {s + 6,371 \times 10^3}]^a_b$


## double integral

### definition
* It's used to calculate the volume of a substance (or solid) whose height at each point is given by a mathematical expression or function

### example
* You have a cheesecake, and which height is given by 
    $$h(x, y) = 36 - 2x - 4y, \quad 0 \leq x \leq 3, \quad 0 \leq y \leq 2$$
    at each point, and you want to know what's the height of the cheesecake
* formula
    $$\int \int_D h(x, y)dA$$
* solution
    * You should treat the `x` as a constant number when you are solving an integral for `y`
    $$= \int_0^3 \int_0^2 (36 - 2x - 4y)dy dx$$
    $$= \int_0^3 [36y - 2xy - 2y^2]_0^2 dx$$
    $$= \int_0^3 (64 - 4x)dx$$
    $$= [64x - 2x^2]_0^3$$
    $$= 174$$