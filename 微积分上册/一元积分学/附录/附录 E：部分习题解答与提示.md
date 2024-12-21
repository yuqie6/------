

本附录提供本书部分习题的解答或提示，供读者参考。 由于篇幅所限，这里只选取了一部分习题进行解答。 建议读者先独立思考并尝试解答习题，然后再参考此处的解答与提示。

### E.1 第一章习题解答与提示

**习题 1.5 第 1 题 (c):**

计算 $\int_0^1 (x^3 + 2x - 1) dx$。

**解答：**

利用定积分的线性性质和牛顿-莱布尼茨公式：

$$\int_0^1 (x^3 + 2x - 1) dx = \left( \frac{1}{4}x^4 + x^2 - x \right) \Big|_0^1 = \frac{1}{4} + 1 - 1 = \frac{1}{4}$$

**习题 1.5 第 2 题:**

已知 $F(x) = \int_0^x \sin t^2 dt$，求 $F'(x)$。

**解答：**

根据变上限积分函数的求导公式，直接得到 $F'(x) = \sin x^2$。

**习题 1.5 第 3 题:**

证明：如果 $f(x)$ 是 $[a, b]$ 上的奇函数，那么 $\int_{-a}^a f(x) dx = 0$；如果 $f(x)$ 是 $[a, b]$ 上的偶函数，那么 $\int_{-a}^a f(x) dx = 2\int_0^a f(x) dx$。

**提示：**

利用定积分的区间可加性和换元积分法。 对于奇函数，考虑将积分区间 $[-\alpha, 0]$ 上的积分用 $x = -t$ 换元。 对于偶函数，利用对称性即可得到结论。

### E.2 第二章习题解答与提示

**习题 2.4 第 1 题 (b):**

求 $\int xe^{-x^2} dx$。

**解答：**

使用第一类换元法 (凑微分法)。 令 $u = -x^2$，则 $du = -2x dx$。

$$\int xe^{-x^2} dx = -\frac{1}{2} \int e^u du = -\frac{1}{2} e^u + C = -\frac{1}{2} e^{-x^2} + C$$

**习题 2.4 第 2 题 (a):**

求 $\int \frac{1}{\sqrt{4-x^2}} dx$。

**解答：**

使用第二类换元法 (三角代换)。 令 $x = 2\sin t$，则 $dx = 2\cos t dt$。

$$\int \frac{1}{\sqrt{4-x^2}} dx = \int \frac{1}{\sqrt{4-4\sin^2 t}} 2\cos t dt = \int \frac{2\cos t}{2\cos t} dt = \int 1 dt = t + C = \arcsin \frac{x}{2} + C$$

**习题 2.4 第 3 题 (b):**

求 $\int \frac{1}{e^x + e^{-x}} dx$。

**解答：**

将分子分母同乘以 $e^x$：

$$\int \frac{1}{e^x + e^{-x}} dx = \int \frac{e^x}{e^{2x} + 1} dx$$

令 $u = e^x$，则 $du = e^x dx$。

$$\int \frac{e^x}{e^{2x} + 1} dx = \int \frac{1}{u^2 + 1} du = \arctan u + C = \arctan e^x + C$$

### E.3 第三章习题解答与提示

**习题 3.4 第 1 题 (a):**

求 $\int x \cos x dx$。

**解答：**

使用分部积分法。 令 $u = x$, $dv = \cos x dx$，则 $du = dx$, $v = \sin x$。

$$\int x \cos x dx = x \sin x - \int \sin x dx = x \sin x + \cos x + C$$

**习题 3.4 第 2 题 (a):**

求 $\int \frac{2x+3}{x^2 - 5x + 6} dx$。

**解答：**

首先将分母分解因式：$x^2 - 5x + 6 = (x-2)(x-3)$。

然后将真分式分解成部分分式：

$$\frac{2x+3}{x^2 - 5x + 6} = \frac{A}{x-2} + \frac{B}{x-3}$$

通分并比较系数，得到 $A = -7$, $B = 9$。

$$\int \frac{2x+3}{x^2 - 5x + 6} dx = \int \left( \frac{-7}{x-2} + \frac{9}{x-3} \right) dx = -7\ln|x-2| + 9\ln|x-3| + C$$

**习题 3.4 第 3 题 (b):**

求 $\int \frac{1}{\sqrt{1+e^x}} dx$。

**解答：**

令 $t = \sqrt{1+e^x}$，则 $e^x = t^2 - 1$, $x = \ln(t^2-1)$, $dx = \frac{2t}{t^2-1} dt$。

$$\int \frac{1}{\sqrt{1+e^x}} dx = \int \frac{1}{t} \cdot \frac{2t}{t^2-1} dt = \int \frac{2}{t^2-1} dt = \int \left( \frac{1}{t-1} - \frac{1}{t+1} \right) dt$$

$$= \ln|t-1| - \ln|t+1| + C = \ln \left| \frac{\sqrt{1+e^x} - 1}{\sqrt{1+e^x} + 1} \right| + C$$

### E.4 第四章习题解答与提示

**习题 4.6 第 1 题 (a):**

计算曲线 $y = x^2$，$x = 2$ 以及 $x$ 轴所围成的图形绕 $x$ 轴旋转一周所得的旋转体体积。

**解答：**

体积微元 $dV = \pi y^2 dx = \pi x^4 dx$，积分区间为 $[0, 2]$。

$$V = \int_0^2 \pi x^4 dx = \pi \cdot \frac{1}{5}x^5 \Big|_0^2 = \frac{32\pi}{5}$$

**习题 4.6 第 2 题 (c):**

计算曲线 $\rho = e^\theta$ 从 $\theta = 0$ 到 $\theta = \pi$ 的弧长。

**解答：**

$$s = \int_0^\pi \sqrt{\rho^2 + (\rho')^2} d\theta = \int_0^\pi \sqrt{e^{2\theta} + e^{2\theta}} d\theta = \int_0^\pi \sqrt{2} e^\theta d\theta = \sqrt{2} e^\theta \Big|_0^\pi = \sqrt{2}(e^\pi - 1)$$

**习题 4.6 第 3 题:**

一个深度为 $h$ 米，上口半径为 $R$ 米的圆锥形水池，盛满了水。 求将池中的水全部抽出所做的功。

**提示：**

将水池分成许多薄层，每一层可以近似看作一个圆柱体。 计算将每一层水提升到水池口所做的功，然后将所有薄层做的功加起来。

**解答:**
以圆锥顶点为原点, 建立坐标系, 设向上为 $y$ 轴正方向。
考虑深度为 $y$ 处, 厚度为 $dy$ 的水层, 其体积约为 $dV = \pi r^2 dy$, 其中 $r$ 为该水层半径。
根据相似三角形, 有 $\frac{r}{y} = \frac{R}{h}$, 所以 $r = \frac{R}{h}y$.
该水层的质量约为 $dm = \rho dV = \rho \pi (\frac{R}{h}y)^2 dy$, 其中 $\rho$ 为水的密度。
将该水层提升到水池口, 需要做的功为 $dW = dm \cdot g \cdot (h-y) = \rho \pi g (\frac{R}{h}y)^2 (h-y) dy$
总功为:
$$W = \int_0^h \rho \pi g (\frac{R}{h})^2 y^2 (h-y) dy = \rho \pi g \frac{R^2}{h^2} \int_0^h (hy^2 - y^3) dy$$
$$ = \rho \pi g \frac{R^2}{h^2} (\frac{h}{3}y^3 - \frac{1}{4}y^4)\Big|_0^h = \rho \pi g \frac{R^2}{h^2} (\frac{h^4}{3} - \frac{h^4}{4}) = \frac{1}{12} \rho \pi g R^2 h^2$$

**习题 4.6 第 5 题:**

用梯形法和辛普森法计算 $\int_0^1 e^{-x^2} dx$ 的近似值 (取 $n=4$)。

**解答：**

$h = \frac{1-0}{4} = 0.25$

$x_0 = 0$, $x_1 = 0.25$, $x_2 = 0.5$, $x_3 = 0.75$, $x_4 = 1$

$f(x_0) = 1$, $f(x_1) = e^{-0.25^2} \approx 0.9394$, $f(x_2) = e^{-0.5^2} \approx 0.7788$, $f(x_3) = e^{-0.75^2} \approx 0.5698$, $f(x_4) = e^{-1} \approx 0.3679$

**梯形法：**

$$\int_0^1 e^{-x^2} dx \approx \frac{0.25}{2} [1 + 2(0.9394 + 0.7788 + 0.5698) + 0.3679] \approx 0.74295$$

**辛普森法：**

$$\int_0^1 e^{-x^2} dx \approx \frac{0.25}{3} [1 + 4(0.9394 + 0.5698) + 2(0.7788) + 0.3679] \approx 0.74685$$

### E.5 第五章习题解答与提示

**习题 5.4 第 1 题 (a):**

判断反常积分 $\int_0^{+\infty} e^{-2x} dx$ 的敛散性，如果收敛，计算其值。

**解答：**

$$\int_0^{+\infty} e^{-2x} dx = \lim_{b \to +\infty} \int_0^b e^{-2x} dx = \lim_{b \to +\infty} \left( -\frac{1}{2}e^{-2x} \right) \Big|_0^b = \lim_{b \to +\infty} \left( -\frac{1}{2}e^{-2b} + \frac{1}{2} \right) = \frac{1}{2}$$

因此，该反常积分收敛，且其值为 $\frac{1}{2}$。

**习题 5.4 第 1 题 (c):**

判断反常积分 $\int_0^1 \frac{1}{x^2} dx$ 的敛散性。

**解答：**

被积函数 $f(x) = \frac{1}{x^2}$ 在 $x=0$ 处无界，因此这是一个瑕积分。

$$\int_0^1 \frac{1}{x^2} dx = \lim_{\epsilon \to 0^+} \int_\epsilon^1 \frac{1}{x^2} dx = \lim_{\epsilon \to 0^+} \left( -\frac{1}{x} \right) \Big|_\epsilon^1 = \lim_{\epsilon \to 0^+} \left( -1 + \frac{1}{\epsilon} \right) = +\infty$$

因此，该反常积分发散。

**习题 5.4 第 2 题 (b):**

判断反常积分 $\int_0^1 \frac{\sin x}{x^2} dx$ 的敛散性。

**提示：**

利用 $\lim_{x \to 0} \frac{\sin x}{x} = 1$ 和比较判别法的极限形式。

**解答:**
由于 $\lim_{x\to 0} \frac{\sin x}{x} = 1$, 因此存在 $\delta > 0$, 当 $0 < x < \delta$ 时, $|\frac{\sin x}{x} - 1| < \frac{1}{2}$, 从而 $\frac{\sin x}{x} < \frac{3}{2}$, 当 $x \in (0, \delta)$。
因此 $\frac{\sin x}{x^2} < \frac{3}{2x}$ 在 $(0,\delta)$ 上成立。
而 $\int_0^{\delta} \frac{1}{x^2}dx$ 发散, 由比较判别法知 $\int_0^\delta \frac{\sin x}{x^2} dx$ 发散。
因此, $\int_0^1 \frac{\sin x}{x^2} dx$ 发散。

**习题 5.4 第 3 题:**

计算 $\Gamma(5)$。

**解答：**

$$\Gamma(5) = (5-1)! = 4! = 4 \times 3 \times 2 \times 1 = 24$$

**习题 5.4 第 4 题:**

利用伽玛函数计算 $\int_0^{+\infty} x^5 e^{-2x} dx$。

**提示：**

令 $t = 2x$。

**解答：**

令 $t = 2x$，则 $x = \frac{1}{2}t$, $dx = \frac{1}{2} dt$。

$$\int_0^{+\infty} x^5 e^{-2x} dx = \int_0^{+\infty} \left(\frac{t}{2}\right)^5 e^{-t} \frac{1}{2} dt = \frac{1}{64} \int_0^{+\infty} t^5 e^{-t} dt = \frac{1}{64} \Gamma(6) = \frac{1}{64} \cdot 5! = \frac{120}{64} = \frac{15}{8}$$

---