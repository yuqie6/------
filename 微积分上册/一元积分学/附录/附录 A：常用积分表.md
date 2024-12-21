本附录列出了一些常用的不定积分公式，供读者查阅。 在使用这些公式时，需要注意积分常数 $C$。

### A.1 基本初等函数的积分

| 序号 | 函数                       | 不定积分                      |
| ---- | -------------------------- | ----------------------------- |
| 1    | $k$ (常数)                  | $kx + C$                     |
| 2    | $x^\mu$ ($\mu \neq -1$)     | $\frac{x^{\mu+1}}{\mu+1} + C$ |
| 3    | $\frac{1}{x}$              | $\ln |x| + C$                |
| 4    | $e^x$                      | $e^x + C$                    |
| 5    | $a^x$ ($a > 0, a \neq 1$) | $\frac{a^x}{\ln a} + C$      |
| 6    | $\cos x$                     | $\sin x + C$                  |
| 7    | $\sin x$                     | $-\cos x + C$                 |
| 8    | $\frac{1}{\cos^2 x} = \sec^2 x$ | $\tan x + C$                  |
| 9    | $\frac{1}{\sin^2 x} = \csc^2 x$ | $-\cot x + C$                 |
| 10   | $\sec x \tan x$              | $\sec x + C$                  |
| 11   | $\csc x \cot x$              | $-\csc x + C$                 |
| 12   | $\frac{1}{1+x^2}$          | $\arctan x + C$             |
| 13   | $\frac{1}{\sqrt{1-x^2}}$   | $\arcsin x + C$            |

### A.2 常用的不定积分公式

| 序号  | 函数                         | 不定积分                                                                                                          |
| --- | -------------------------- | --------------------------------------------------------------------------------------------------------- |
| 1   | $\tan x$                   | $-\ln                                                                \cos x                          + C$ |
| 2   | $\cot x$                   | $\ln                                                                    \sin x                           + C$ |
| 3   | $\sec x$                   | $\ln                                                                    \sec x + \tan x                  + C$ |
| 4   | $\csc x$                   | $\ln                                                                    \csc x - \cot x                  + C$ |
| 5   | $\frac{1}{a^2+x^2}$        | $\frac{1}{a} \arctan \frac{x}{a} + C$                                                                         |
| 6   | $\frac{1}{\sqrt{a^2-x^2}}$ | $\arcsin \frac{x}{a} + C$                                                                                    |
| 7   | $\frac{1}{x^2-a^2}$        | $\frac{1}{2a} \ln                                                       \frac{x-a}{x+a}                  + C$ |
| 8   | $\frac{1}{\sqrt{x^2+a^2}}$ | $\ln(x + \sqrt{x^2+a^2}) + C$                                                                                 |
| 9   | $\frac{1}{\sqrt{x^2-a^2}}$ | $\ln                                                                   x + \sqrt{x^2-a^2}               + C$ |
| 10  | $\sqrt{a^2 - x^2}$         | $\frac{a^2}{2} \arcsin \frac{x}{a} + \frac{x}{2} \sqrt{a^2 - x^2} + C$ |                                       |
| 11  | $\sqrt{x^2 \pm a^2}$       | $\frac{x}{2}\sqrt{x^2 \pm a^2} \pm \frac{a^2}{2} \ln                    x+\sqrt{x^2 \pm a^2}             + C$ |
| 12  | $\int \frac{1}{\sin x}dx$  | $\ln                                                                    \tan\frac{x}{2}                  +C$  |
| 13  | $\int \frac{1}{\cos x}dx$  | $\ln                                                                   \tan(\frac{x}{2}+\frac{\pi}{4})  +C$  |

### A.3 一些特殊的定积分公式

1. **Wallis 公式:**

    $$W_n = \int_0^{\pi/2} \sin^n x dx = \int_0^{\pi/2} \cos^n x dx = \begin{cases}
    \frac{n-1}{n} \cdot \frac{n-3}{n-2} \cdots \frac{1}{2} \cdot \frac{\pi}{2}, & n \text{ 为偶数} \\
    \frac{n-1}{n} \cdot \frac{n-3}{n-2} \cdots \frac{2}{3}, & n \text{ 为大于1的奇数}
    \end{cases}$$

    利用 Wallis 公式可以推导出：

    $$\lim_{n \to \infty} \frac{1}{\sqrt{n}} \left[ \frac{(2n)!!}{(2n-1)!!} \right] = \sqrt{\pi}$$

2. **伽玛函数的几个特殊值：**

    *   $\Gamma(1) = 1$
    *   $\Gamma(\frac{1}{2}) = \sqrt{\pi}$
    *   $\Gamma(n) = (n-1)!$ ($n$ 为正整数)

---
