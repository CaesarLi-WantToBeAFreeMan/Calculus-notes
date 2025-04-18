# Course #6: Differentiation

# Platform: Edx

# Course Name: DelftX Calc001x: Pre-University Calculus

# Author: Caesar James LEE

## Unknown Keywords

| English           | Pronunciation     | Chinese Meaning |
| :---------------: | :---------------: | :-------------: |
| differentiation   | ˌdɪfǝˌrɛnʃɪˈеʃǝn  | 微分            |
| derivative        | dǝˈrɪvǝtɪv        | 導數            |
| optimization      | ˌɑptɪmaɪˈzеʃǝn    | 最佳化          |
| instantaneous     | ˌɪnstǝnˈtеnɪǝs    | 瞬間的          |
| quotient          | ˈkwoʃǝnt          | 商              |
| tedious           | ˈtidɪǝs           | 冗長乏味的       |
| arbitrary         | ˈɑrbǝˌtrɛrɪ       | 隨心所欲的       |
| orthogonally      | ɒrˈθɑɡǝnǝlɪ       | 直角地，正交地   |
| maxima            | ˈmæksǝmǝ          | 最大數們        |
| minima            | ˈmɪnǝmǝ           | 最小數們        |
| extremum          | ˈɪkstrɪmǝm        | 極值            |
| differentiable    | ˌdɪfǝˈrɛnʃɪǝbḷ    | 可微的          |
| beware            | bɪˈwɛr            | 當心            |
| suffice           | sǝˈfaɪs           | 足夠            |
| cannon            | ˈkænǝn            | 大砲            |
| trajectory        | trǝˈdʒɛktrɪ       | 軌道            |
| kink              | kɪŋk              | 扭結            |
| lukewarm          | ˈlukˈwɒrm         | （液體）微熱的   |
| proportional      | prǝˈporʃǝnḷ       | 成常比的        |

 
## Unknown Phrases

| Phrase            | Pronunciation     | Chinese Meaning   |
| :---------------: | :---------------: | :---------------: |
| roller coaster    | ˈrolɚ ˈkostɚ      | 雲霄飛車          |

## Examples of Limit

### 1. Instantaneous Velocity
* Refers to the distance traveled in a very short time
* Formula:
$$\lim_{\Delta t \rightarrow 0} \frac {\Delta x} {\Delta t}$$
### 2. Slope
* Refers to the direction of the line on a plane
* Formula:
$$\lim_{\Delta x \rightarrow 0} \frac {\Delta y} {\Delta x}$$

## Differentiation

### Definition
* Refers to the local variation of a function
* It's a difference quotient
* Formula:
$$\frac {f(a + \Delta x) - f(x)} {\Delta x}$$

## Derivation

### Definition
* Calculating the slope of a single-variable function's tangent line, which is the best liner approximation of the function near that input value, at the point on the graph of the function

### Formula
$$\lim_{\Delta x \rightarrow 0} \frac {f(a + \Delta x) - f(a)} {\Delta x}$$

### Notation
* for $f(a)$
    1. $f'(a)$
    2. $\frac {d} {dx}(a)$

## Relationship Between Differentiation And Derivation

***Differentiation is an act of calculating a derivation***

## Derivative Rules

### Basic Standard Derivatives
| Standard Function                     | Derivative                                    |
| :-----------------------------------: | :-------------------------------------------: |
| ***BASIC***                           | ***BASIC***                                   |
| $a$                                   | $0$                                           |
| $x^a$                                 | $ax^{a - 1}$                                  |
| ***TRIGONOMETRIC***                   | ***TRIGONOMETRIC***                           |
| $\sin(x)$                             | $\cos(x)$                                     |
| $\cos(x)$                             | $-\sin(x)$                                    |
| $\tan(x)$                             | $\sec^2(x)$                                   |
| $\cot(x)$                             | $-\csc^2(x)$                                  |
| $\sec(x)$                             | $\sec(x)\tan(x)$                              |
| $\csc(x)$                             | $-\csc(x)\cot(x)$                             |
| $\arcsin(x), \quad x \neq \pm 1$      | $\frac {1} {\sqrt{1 - x^2}}$                  |
| $\arccos(x), \quad x \neq \pm 1$      | $-\frac {1} {\sqrt{1 - x^2}}$                 |
| $\arctan(x)$                          | $\frac {1} {1 + x^2}$                         |
| $\cot^{-1}(x)$                        | $-\frac {1} {1 + x^2}$                        |
| $\sec^{-1}(x), \quad x \neq \pm 1, 0$ | $\frac {1} {\lvert x \rvert \sqrt{x^2 - 1}}$  |
| $\csc^{-1}(x), \quad x \neq \pm 1, 0$ | $-\frac {1} {\lvert x \rvert \sqrt{x^2 - 1}}$ |
| $\ln(x)$                              | $\frac {1} {x}$                               |
| ***LOGARITHM & EXPONENTIAL***         | ***LOGARITHM & EXPONENTIAL***                 |
| $a^x, \quad a > 0$                    | $a^x\ln(a)$                                   |
| $e^x$                                 | $e^x$                                         |
| $\log_a(x)$                           | $\frac {1} {x\ln(a)}$                         |
| $\ln(x), \quad x > 0$                 | $\frac {1} {x}$                               |
| $\ln(\lvert x \rvert)$                | $\frac {1} {x}$                               |
| $x^x$                                 | $x^x(1 + \ln(x))$                             |

### calculation rules
| calculation           | derivative                                |
| :-------------------: | :---------------------------------------: |
| $f(x) \pm g(x)$       | $f'(x) \pm g'(x)$                         |
| $af(x)$               | $af'(x)$                                  |
| $f(x) \times g(x0)$   | $f'(x)g(x) + f(x)g'(x)$                   |
| $\frac {f(x)} {g(x)}$ | $\frac {f'(x)g(x) - f(x)g'(x)} {g(x)^2}$  |
| $f(g(x))$             | $f'(g(x))g'(x)$                           |

## Tangent Lines

### Properties
1. Slope: $f'(p) = \tan(\theta)$, $\theta$ is a intersect between the tangent line and the positive x-axis
2. Through $(p, f(p))$
3. The directive, representing the slope of the tangent line, exists even at an angel of 0 radians where the tangent function equals to 0, indicating a horizontal tangent line

### Tangent Line Equation
$$f'(p) = \frac {y - f(p)} {x - p}$$
$$y = f'(p)(x - p) + f(p)$$

### Solving Strategy
1. Solve the point(a, b)
2. Solve the directive value $f'(a)$
3. Solve the equation $\frac {y - b} {x - a} = f'(a)$

## Minima And Maxima

### Global Minimum And Maximum
* The minimum and maximum in the whole function

### Extremum (local minimum and maximum)
* The minimum and maximum in a given range in the function

### Find Extremum
Find
1. Critical points: $f'(x) = 0$
2. Singular points: $f'(x)$ doesn't exist
3. Boundary points

## Differentiable Functions

* A function whose derivative exists at each point in its domain
* A function is not differentiable at `x = a` when
    1. The function is discontinuous at `x = a`

    ![discontinuous function](photos/week%206/06-01.png)

    2. the graph of the function has a kink at `x = a`

    ![a function has a kink](photos/week%206/06-02.png)

    3. the graph of the function has a vertical tangent line at `x = a`

    ![vertical tangent line](photos/week%206/06-03.png)

* examples:
1. $$f(x) = x^2$$
2. $$f(x) = \sin(x)$$
3. $$f(x) = e^x$$