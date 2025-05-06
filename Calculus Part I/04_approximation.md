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