# Course #4: Approximation

# Platform: Edx

# Course Name: DelftX MMFEC1X: Calculus I: From Functions to Differential Equations

# Author: Caesar James LEE

## Unknown Keywords

| English           | Pronunciation     | Chinese Meaning            |
| :---------------: | :---------------: | :------------------------: |
| tangible          | ˈtændʒǝbḷ         | 可觸知的；實際的            |
| propagation       | ˌprɑpǝˈɡеʃǝn      | 繁殖；宣傳                 |
| ubiquitous        | juˈbɪkwǝtǝs       | 到處存在的                 |
| rigorous          | ˈrɪɡǝrǝs          | 嚴格的                     |
| drawback          | ˈdrɒˌbæk          | 缺點                      |
| crystalize        | ˈkrɪstḷˌaɪz       | 結晶；具體化               |
| adequately        | ˈædǝkwɪtlɪ        | 適當地；足夠地；充分地      |
| perspective       | pɚˈspɛktɪv        | 透視圖法；看法；洞察力      |
| obstacle          | ˈɑbstǝkḷ          | 障礙（物）                 |
| scheme            | skim              | 計畫；方案                 |
| cylindrical       | sɪˈlɪndrɪkḷ       | 圓柱形的                   |
| rim               | rɪm               | （尤指圓形物的）邊緣        |
| hierarchy         | ˈhaɪǝˌrɑrkɪ       | 等級制度；層級             |
| arbitrarily       | ˌɑrbǝˈtrɛrǝlɪ     | 任意地                    |
| generalization    | ˌdʒɛnǝrǝlaɪˈzеʃǝn | 普遍化；概括               |
| extensively       | ɪkˈstɛnsɪvlɪ      | 廣大地；廣泛地             |
| kinetic           | kɪˈnɛtɪk          | 運動引起的；有力的         |

## Unknown Phrase

| English           | Pronunciation     | Chinese Meaning            |
| :---------------: | :---------------: | :------------------------: |
| turn out          | tɝn aʊt           | 結果是；證明是              |
| rile up           | raɪl ʌp           | 激怒                       |

## obstacle

* when trying to find the decimal expansion of a function value we can run into two major obstacles:
    1. some decimal expansions have no repeating patterns
    2. computation can cost a lot of time or other resources

## approximation

### definition

* given a function f(x) an approximation of a function value f(x) is a real number $\hat {f}(x)$ that is `close` to f(x)
* we denote this as $$f(x) \approx \hat{f}(x)$$
* example
$$\sqrt {101} \approx 10$$

### approximation error

* suppose $f(x) \approx \hat{f}(x)$ then the approximation error `E` is defined as
$$E = \lvert f(x) - \hat{f}(x) \rvert$$
* example
$$E = \sqrt {101} - 10 \approx \lvert 10.049 \, 875 \, 621 - 10 \rvert = 0.049 \, 875 \, 621$$

### relative approximation error

* the relative approximation error $\eta$ is defined as
$$\eta = \lvert \frac {f(x) - \hat {f}(x)} {f(x)}\rvert$$
* example
$$\eta = \lvert \frac {\sqrt {101} - 10} {\sqrt {101}} \rvert \approx \lvert \frac {10.049 \, 875 \, 621 - 10} {10.049 \, 875 \, 621} \rvert = \frac {49,875,621} {10,049,875,621} \approx 0.004 \, 962 \, 809$$

### approximation scheme

1. linearization
    * definition
        * given a function $y = f(x)$ the tangent line to the graph of $f$ at the point $x = a$ is given by the equation
        $$y = f(a) + f'(a)(x - a)$$
        * the linear function whose graph is the tangent line at $x = a$ is called `linearization` of $f$ at $a$
        $$L(a) = f(a) + f'(a)(x - a) = y(a)$$
    * example: $f(x) = \sqrt {x + 3}$
        $$
        f'(x) = \frac {1} {2} \cdot (x + 3)^{- \frac {1} {2}}\\
        = \frac {1} {2 \cdot \sqrt {x + 3}}\\
        L(a) = f(a) + f'(a)(x - a)\\
        L(1) = \sqrt {1 + 3} + \frac {1} {2 \cdot \sqrt {1 + 3}}(x - 1)\\
        = \frac {x} {4} + \frac {7} {4}
        $$
2. differential
    * definition
        * given a function $y = f(x)$ the differential $dy = dx$ of $f$ is given by
        $$dy = df = f'(x)dx$$
        * if we set $x = x_0$ and $dx = \Delta x$ we obtain the approximation
        $$dy \approx \Delta y = f(x_0 + \Delta x) - f(x_0)$$
        * example: $f(x) = x^3 + 2x^2, domain: [-1, -0.8]$
        $$
        f'(x) = 3x^2 + 4x\\
        df = (3 \cdot (-1)^2 + 4 \cdot (-1)) \cdot \lvert -0.8 + 1 \rvert\\
        = -0.2
        $$
    * errors
        1. approximation error
        $$
        E = \lvert \Delta f - df \rvert$$
        * example: $f(x) = x^3 + 2x^2, domain: [-1, -0.8]$
        $$
        E = \lvert f(-0.8) - f(-1) - df\rvert\\
        = \frac {96} {125} - 1 + 0.2\\
        = -\frac {4} {125}
        $$
        2. approximation absolute error
        $$df = f'(x)dx$$
        * example: a cylindrical beam with a height of $8 \, m$, a diameter of $0.6 \pm 0.01 \, m$, and a volume of $V \pm \Delta V \, m^3$
        $$\Delta V \approx dV = (8 \pi \cdot (\frac {x} {2})^2)' \cdot \Delta x\\
        = (2 \pi x^2)' \cdot 0.01\\
        = 4 \pi \cdot 0.6 \cdot 0.01\\
        \approx 0.075
        $$
        3. approximation relative error
        $$\frac {df} {f(x)} = \frac {f'(x)} {f(x)}dx$$
        * example: a cylindrical beam with a height of $8 \, m$, a diameter of $0.6 \pm 0.01 \, m$, and a volume of $V \pm \Delta V \, m^3$
        $$\frac {\Delta x} {x} = \frac {0.01} {0.6} = 1.6%$$

## taylor polynomials

### definition

* the n-th taylor polynomial of $f$ at the point $a$
$$
T_n(x) = f(a) + f'(a)(x - a) + \frac {1} {2} f''(a)(x - a)^2 + \dots + \frac {1} {n!} f^{(n)}(x - a)^n\\
= \sum_{k = 0}^n \frac {1} {k!}f^{(k)}(a)(x - a)^k
$$
* example: $\sqrt {4.05}$
    * $$f(x) = \sqrt{x}$$
    * $$f'(x) = \frac {1} {2 \sqrt{x}}$$
    * $$f''(x) = -\frac {1} {4 \sqrt {x^3}}$$
    $$
    T_2(x) = \sqrt {4} + \frac {1} {2 \sqrt {4}}(x - 4) + \frac {1} {2} \cdot (-\frac {1} {4 \sqrt{4^3}})(x - 4)^2\\
    = 2 + \frac {1} {4}(x - 4) - \frac {1} {64}(x - 4)^2\\
    T_2(4.05) = 2 + \frac {1} {4}(4.05 - 4) - \frac {1} {64}(4.05 - 4)^2\\
    = \frac {51,519} {25,600}\\
    \approx 2.012 \, 460 \, 938\\
    \sqrt {4.05} \approx 2.012 \, 461 \, 180
    $$
* the higher the degree of the taylor polynomial you use, the better the approximation

### basic property
* $$f^{(k)}(a) = T_n^{(k)}(a), \quad \text{for } k \in \{x \in \mathbb{Z} \mid 0 \leq x \leq n\}$$

### choosing the center

* when choosing the center of approximation `a` keep in mind
    1. we need to know $f^{(n)}$ for sufficiently high `n`
    2. `a` needs to be close to the point `x` at which we approximate `f(x)`
* example
    * we use $f(x) = \sqrt {x}$ to approximate $\sqrt {102}$, and the center is $a = 100$

### order

* `order` refers to the highest power of `x` or the number of derivatives used
* example: $\sqrt {102}$
    * $f = \sqrt {x}$
    * $f'(x) = \frac {1} {2 \sqrt{x}}$
    * $f''(x) = -\frac {1} {4 \sqrt {x^3}}$
    * $f^{(3)}(x) = \frac {3} {8 \sqrt {x^5}}$
    1. zeroth order
        $$T_0(102) = \sqrt {100} = 10$$
    2. first order
        $$T_1(102) = \sqrt {100} + \frac {1} {2 \sqrt {100}}(102 - 100) = 10.1$$
    3. second order
        $$T_2(102) = \sqrt {100} + \frac {1} {2 \sqrt {100}}(102 - 100) - \frac {1} {2} \frac {1} {4 \sqrt {100^3}}(102 - 100)^2 = 10.099 \, 5$$
    4. third order
        $$T_3(102) = \sqrt {100} + \frac {1} {2 \sqrt {100}}(102 - 100) - \frac {1} {2} \frac {1} {4 \sqrt {100^3}}(102 - 100)^2 + \frac {1} {6} \frac {3} {8 \sqrt {100^5}}(102 - 100)^3 = 10.099 \, 505$$

### computation rules

1. sum rule
$$T_n(x) = T_n^g(x) + T_n^h(x)$$
* example: $f(x) = e^x + \sin(x) \text{, for a = 0}$
$$
T_3^{e^x} = \frac {e^0} {0!} + \frac {e^0} {1!} \cdot (x - 0) + \frac {e^0} {2!} \cdot (x - 0)^2 + \frac {e^0} {3!} \cdot (x - 0)^3\\
= 1 + x + \frac {x^2} {2} + \frac {x^3} {6}\\
T_3^{\sin(x)} = \frac {\sin(0)} {0!} + \frac {\cos(0)} {1!} - \frac {\sin(0)} {2!} - \frac {\cos(0)} {3!}\\
= x - \frac {x^3} {6}\\
T_3 = T_3^{e^x} + T_3^{\sin(x)}\\
= 1 + x + \frac {x^2} {2} + \frac {x^3} {6} + x - \frac {x^3} {6}\\
= 1 + 2x + \frac {x^2} {2}
$$
2. product rule
$$T_{n + k}(x) = (x - a)^kT_n^g(x)$$
* example: $f(x) = (x - 1)e^x \text {, for } a = 1$
$$
T_3(x) = (x - 1)T_2^{(x - 1)e^x}\\
= (x - 1)(e + e(x - 1) + \frac {e} {2}(x - 1)^2)\\
= e(x - 1) + e(x - 1)^2 + \frac {e} {2}(x - 1)^3
$$
3. substitute rule
$$
T_{n \cdot k}(x) = \sum_{i = 0}^n \frac {g^{(i)}(0)} {i!}((x - a)^k)^i\\
= g(0) + g'(0)(x - a)^k + \frac {g''(0)(x - a)^{2k}} {2!} + \dots + \frac {g^{(n)}(0)} {n!}(x - a)^{nk}\\
\text {for function: } f(x) = g(h(x)) \text { where } h(x) = (x - a)^k
$$
* example: $f(x) = \cos(x^2) \text { , for } a = 0$
$$
g(u) = \cos(u)\\
h(x) = x^2\\
f(x) = g(h(x))\\
g'(u) = -\sin(u)\\
g''(u) = -\cos(u)\\
T_2^g(x) = \frac {g(0)} {0!} + \frac {g'(0)(x - 0)} {1!} + \frac {g''(0)(x - 0)^2} {2!}\\
= \cos(0) - \sin(0)x - \cos(0)x^2\\
= 1 + 0 - \frac {x^2} {2}\\
= 1 - \frac {x^2} {2}\\
T_4(0) = T_2^g(x^2) = 1 - \frac {(x^2)^2} {2}\\
= 1 - \frac {x^4} {2}
$$

### approximation error

* given a function $f$ and its taylor polynomial $T_n$ at the point $a$, the approximation error in $x$ is given by
$$R_n(x) = \lvert f(x) - T_n(x) \rvert$$

## taylor's inequality

### theorem

* let $f$ be a function and $T_n$ its taylor polynomial at the point $a$, $D$ be an interval that contains the point $a$ and $M$ an upper bound for the function $\lvert f^{(n + 1)}(x) \rvert$ on $D$
* you need to find the smallest integer that is greater than or equals to $f$ 
* for example, $M = 3$ for $e$
$$\lvert f^{(n + 1)} (x) \rvert \leq M \quad \text {holds for all x in D}$$ 
then for all $x \in D$
$$\lvert f(x) - T_n(x) \rvert \leq \frac {M} {(n + 1)!} \lvert x - a \rvert^{n + 1}$$
* example: $f(x) = e^x \quad a = 0$
$$
T_n(x) = \sum_{k = 0}^n \frac {f^{(k)}(0)x^k} {k!}\\
= \sum_{k = 0}^n \frac {x^k} {k!}\\
T_5(x) = 1 + x + \frac {x^2} {2} + \frac {x^3} {6} + \frac {x^4} {24} + \frac {x^5} {120}\\
T_5(1) = 1 + 1 + \frac {1} {2} + \frac {1} {6} + \frac {1} {24} + \frac {1} {120}\\
= \frac {163} {60}\\
\approx 2.716 \, 666 \, 667\\
\text {more convenient: upper bound: } M = 3 \quad \text {domain: } D = [0, 1]\\
\lvert e^x - T_5(x) \rvert \leq \frac {3} {(5 + 1)!} \lvert x - 0 \rvert^{5 + 1}\\
= \frac {x^6} {120}\\
\lvert e^1 - T_5(1) \rvert \leq \frac {3} {6!} x^{6}\\
\approx \frac {1} {240}\\
$$