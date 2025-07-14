## 🛠一. 使用的软件

![Typora](https://i-blog.csdnimg.cn/direct/616a4fcba7624ad1a1b2149c3fc68f40.webp#pic_center)

> 💡 **软件版本说明**：
>
> - 使用软件：**Typora v1.9.5**
> - 使用方法：推荐参考以下教程（由 CSDN 大佬整理）
>
> 🔗 [https://blog.csdn.net/qq_61621323/article/details/141036982](https://blog.csdn.net/qq_61621323/article/details/141036982)

## 🔗 上期内容 & 项目地址

> 📚 **推荐阅读**：  
> 👉 [Markdown 结合 Typora 基础使用（1）](https://blog.csdn.net/2302_77872181/article/details/149306936)  
> 👉 [Markdown 结合 Typora 基础使用（2）](https://blog.csdn.net/2302_77872181/article/details/149308824)
> 👉 [Markdown 结合 Typora 基础使用 —— 数学公式（3）](https://blog.csdn.net/2302_77872181/article/details/149314933)
> 👉 [Markdown 结合 Typora 基础使用 —— 数学公式（4）](https://blog.csdn.net/2302_77872181/article/details/149315435)

> 💻 **源码仓库地址**：  
> 👉 [GitHub：Markdown-Examples](https://github.com/MiachelZyc/Markdown)  
> 📄 本章文件名：markdown5.md

🌟 **如果你觉得本项目对你有帮助**，欢迎一键 `⭐Star` 支持，让更多人受益！

## 📚二. markdown 补充扩展（5）
### 1、希腊字母（Greek Letters）📚

> 💡 **说明**  
> 希腊字母在数学、物理、工程等学科中扮演重要角色。使用 LaTeX 可以方便地调用其对应的数学符号，下面展示常见希腊字母及其变体形式，适用于公式推导、符号标记等场景。

---

| 🔤 命令及变体        | 🧮 显示效果         | 🔤 命令及变体            | 🧮 显示效果             | 🔤 命令及变体            | 🧮 显示效果             |
| ------------------- | ------------------ | ----------------------- | ---------------------- | ----------------------- | ---------------------- |
| `\Alpha` / `\alpha` | $\Alpha\ (\alpha)$ | `\Beta` / `\beta`       | $\Beta\ (\beta)$       | `\Gamma` / `\gamma`     | $\Gamma\ (\gamma)$     |
| `\Delta` / `\delta` | $\Delta\ (\delta)$ | `\Epsilon` / `\epsilon` | $\Epsilon\ (\epsilon)$ | `\varepsilon`           | $\varepsilon$          |
| `\Zeta` / `\zeta`   | $\Zeta\ (\zeta)$   | `\Eta` / `\eta`         | $\Eta\ (\eta)$         | `\Theta` / `\theta`     | $\Theta\ (\theta)$     |
| `\vartheta`         | $\vartheta$        | `\Iota` / `\iota`       | $\Iota\ (\iota)$       | `\Kappa` / `\kappa`     | $\Kappa\ (\kappa)$     |
| `\varkappa`         | $\varkappa$        | `\Lambda` / `\lambda`   | $\Lambda\ (\lambda)$   | `\Mu` / `\mu`           | $\Mu\ (\mu)$           |
| `\Nu` / `\nu`       | $\Nu\ (\nu)$       | `\Xi` / `\xi`           | $\Xi\ (\xi)$           | `\Omicron` / `\omicron` | $\Omicron\ (\omicron)$ |
| `\Pi` / `\pi`       | $\Pi\ (\pi)$       | `\varpi`                | $\varpi$               | `\Rho` / `\rho`         | $\Rho\ (\rho)$         |
| `\varrho`           | $\varrho$          | `\Sigma` / `\sigma`     | $\Sigma\ (\sigma)$     | `\varsigma`             | $\varsigma$            |
| `\Tau` / `\tau`     | $\Tau\ (\tau)$     | `\Upsilon` / `\upsilon` | $\Upsilon\ (\upsilon)$ | `\Phi` / `\phi`         | $\Phi\ (\phi)$         |
| `\varphi`           | $\varphi$          | `\Chi` / `\chi`         | $\Chi\ (\chi)$         | `\Psi` / `\psi`         | $\Psi\ (\psi)$         |
| `\Omega` / `\omega` | $\Omega\ (\omega)$ | `\ell`                  | $\ell$                 | `\eth`                  | $\eth$                 |
| `\hbar` / `\hslash` | $\hbar\ (\hslash)$ | `\mho`                  | $\mho$                 | `\partial`              | $\partial$             |

---

> 📝 **特别符号说明**  
> - `\hbar`：ℏ，普朗克常数除以 $2\pi$  
> - `\partial`：∂，常用于偏导数  
> - `\mho`：℧，电导单位（西门子）符号  
> - `\ell`：ℓ，小写花体字母，用于长度等量表示  

📌 **提示：** 某些大写命令（如 `\Alpha`）在部分 LaTeX 渲染器中不生效，推荐直接使用拉丁大写字母 `A`、`B` 代替。

### 2、特殊字符🧩

#### ① 说明 📝
> LaTeX 提供了丰富的数学符号。你还可以使用 `\large`、`\small`、`\Huge` 等命令调整字体大小：  
> 示例：${\LARGE A}{\Large A}{\large A}A{\small A}{\tiny A}$

---

#### ② 关系运算符 ➕➖✖️➗

| 输入             | 显示               | 输入                  | 显示                    | 输入          | 显示         |
| ---------------- | ------------------ | --------------------- | ----------------------- | ------------- | ------------ |
| \pm (\mp)        | $\pm\ (\mp)$       | \times                | $\times$                | \div          | $\div$       |
| \cdot            | $\cdot$            | \mid / \nmid          | $\mid$ / $\nmid$        | \parallel (\\ | )            |
| \bigoplus        | $\bigoplus$        | \bigotimes            | $\bigotimes$            | \bigodot      | $\bigodot$   |
| \le / \ge        | $\le,\ \ge$        | \leqslant / \geqslant | $\leqslant,\ \geqslant$ | \ll           | $\ll$        |
| \neq             | $\neq$             | \approx               | $\approx$               | \triangleq    | $\triangleq$ |
| \xlongequal{A=B} | $\xlongequal{A=B}$ | \equiv                | $\equiv$                | \doteq        | $\doteq$     |
| \sim             | $\sim$             | \cong                 | $\cong$                 | \propto       | $\propto$    |
| \prec            | $\prec$            | \pmod{2}              | $\pmod{2}$              | \bmod         | $\bmod$      |

---

#### ③ 集合运算符 🧮

| 输入      | 显示        | 输入        | 显示          | 输入       | 显示         |
| --------- | ----------- | ----------- | ------------- | ---------- | ------------ |
| \emptyset | $\emptyset$ | \varnothing | $\varnothing$ | \setminus  | $\setminus$  |
| \subset   | $\subset$   | \subseteq   | $\subseteq$   | \subsetneq | $\subsetneq$ |
| \supset   | $\supset$   | \supseteq   | $\supseteq$   | \supsetneq | $\supsetneq$ |
| \bigcap   | $\bigcap$   | \bigcup     | $\bigcup$     |            |              |
| \bigwedge | $\bigwedge$ | \bigvee     | $\bigvee$     |            |              |
| \in       | $\in$       | \notin      | $\notin$      | \ni        | $\ni$        |

---

#### ④ 三角运算符 📐

| 输入    | 显示      | 输入   | 显示     | 输入 | 显示   |
| ------- | --------- | ------ | -------- | ---- | ------ |
| \circ   | $\circ$   | \angle | $\angle$ | \bot | $\bot$ |
| \degree | $\degree$ |        |          |      |        |

---

#### ⑤ 微积分符号 ∫ ∬ ∮

| 输入  | 显示    | 输入   | 显示     | 输入   | 显示     |
| ----- | ------- | ------ | -------- | ------ | -------- |
| \int  | $\int$  | \iint  | $\iint$  | \iiint | $\iiint$ |
| \oint | $\oint$ | \oiint | $\oiint$ | \prime | $\prime$ |
| \lim  | $\lim$  | \infin | $\infin$ | \nabla | $\nabla$ |
| \grad | $\grad$ |        |          |        |          |

---

#### ⑥ 逻辑运算符 🔀

| 输入     | 显示       | 输入         | 显示            | 输入   | 显示     |
| -------- | ---------- | ------------ | --------------- | ------ | -------- |
| \forall  | $\forall$  | \exist       | $\exist$        | \lnot  | $\lnot$  |
| \because | $\because$ | \therefore   | $\therefore$    | \top   | $\top$   |
| \land    | $\land$    | \lor         | $\lor$          | \vdash | $\vdash$ |
| \vDash   | $\vDash$   | \not<, \not> | $\not<,\ \not>$ |        |          |

---

#### ⑦ 带帽符号 🎓

| 输入              | 显示                  | 输入            | 显示                                                         |
| ----------------- | --------------------- | --------------- | ------------------------------------------------------------ |
| \hat{xy}          | $\hat{xy}$            | \widehat{xyz}   | $\widehat{xyz}$                                              |
| \tilde{xy}        | $\tilde{xy}$          | \widetilde{xyz} | $\widetilde{xyz}$                                            |
| \check{x}         | $\check{x}$           | \breve{y}       | $\breve{y}$                                                  |
| \grave{x}         | $\grave{x}$           | \acute{y}       | $\acute{y}$                                                  |
| \dot{x}, \ddot{x} | $\dot{x}$, $\ddot{x}$ | \overparen{xy}  | ![$\overparen{xy}$](https://i-blog.csdnimg.cn/direct/2bd0b89a16b947b6a6fc3a332b905993.png) |

---
#### ⑧ 选取符号 ⌦

| 输入                           | 显示                             | 输入                            | 显示                              |
| ------------------------------ | -------------------------------- | ------------------------------- | --------------------------------- |
| \fbox{a+b+c+d}                 | $\fbox{a+b+c+d}$                 |                                 |                                   |
| \overbrace{xx\cdots x}^{10个x} | $\overbrace{xx\cdots x}^{10个x}$ | \underbrace{xx\cdots x}_{10个x} | $\underbrace{xx\cdots x}_{10个x}$ |

---

#### ⑨ 箭头符号 ⬅️➡️⬆️⬇️

| 输入           | 显示             | 输入            | 显示              | 输入                | 显示                    |
| -------------- | ---------------- | --------------- | ----------------- | ------------------- | ----------------------- |
| \leftarrow     | $\leftarrow$     | \rightarrow     | $\rightarrow$     | \leftrightarrow     | $\leftrightarrow$       |
| \longleftarrow | $\longleftarrow$ | \longrightarrow | $\longrightarrow$ | \longleftrightarrow | $\longleftrightarrow$   |
| \Leftarrow     | $\Leftarrow$     | \Rightarrow     | $\Rightarrow$     | \Leftrightarrow     | $\Leftrightarrow$       |
| \Longleftarrow | $\Longleftarrow$ | \Longrightarrow | $\Longrightarrow$ | \Longleftrightarrow | $\Longleftrightarrow$   |
| \uparrow       | $\uparrow$       | \downarrow      | $\downarrow$      | \updownarrow        | $\updownarrow$          |
| \Uparrow       | $\Uparrow$       | \Downarrow      | $\Downarrow$      | \Updownarrow        | $\Updownarrow$          |
| \to            | $\to$            | \gets           | $\gets$           | \mapsto             | $\mapsto$               |
| \swarrow       | $\swarrow$       | \searrow        | $\searrow$        | \nwarrow / \nearrow | $\nwarrow$ / $\nearrow$ |

---

#### ⑩ 空格控制符 🔡

| 输入 | 效果   | 输入     | 效果   | 输入     | 效果       |
| ---- | ------ | -------- | ------ | -------- | ---------- |
| `\!` | $|\!|$ | 默认空格 | $||$   | `\quad`  | $|\quad|$  |
| `\,` | $|\,|$ | `\;`     | $|\;|$ | `\qquad` | $|\qquad|$ |


### 3、字体 ✍️

> ⚠️ **注意：部分字体命令在 Typora 或 KaTeX 中未定义**  
> 比如 `\mit` 和 `\scr` 不是标准 MathJax / KaTeX 支持的命令，会报错：  
> `KaTeX parse error: Undefined control sequence: \mit`

---

#### ✅ 推荐使用以下通用字体命令：

| 输入    | 说明                 | 显示              | 兼容性                               |
| ------- | -------------------- | ----------------- | ------------------------------------ |
| `\rm`   | 罗马体               | ${\rm{Sample}}$   | ✅ KaTeX 支持                         |
| `\it`   | 意大利体             | ${\it{Sample}}$   | ✅ KaTeX 支持                         |
| `\bf`   | 粗体                 | ${\bf{Sample}}$   | ✅ KaTeX 支持                         |
| `\sf`   | 无衬线体             | ${\sf{Sample}}$   | ✅ KaTeX 支持                         |
| `\tt`   | 打字机体             | ${\tt{Sample}}$   | ✅ KaTeX 支持                         |
| `\Bbb`  | 黑板粗体             | ${\Bbb{Sample}}$  | ✅ KaTeX 支持，需 amssymb 宏包        |
| `\frak` | 哥特体（德式）       | ${\frak{Sample}}$ | ✅ KaTeX 支持，需 amssymb 宏包        |
| `\mit`  | 数学斜体（大写小写） | ${\mit{Sample}}$  | ❌ 非 KaTeX 内建命令，但Typora支持    |
| `\scr`  | 手写体（mathrsfs）   | ${\scr{Sample}}$  | ❌ 依赖额外宏包：mathrsfs但Typora支持 |
---

#### 🚫 以下命令 **CSDN 的markdown不支持**

| 输入   | 说明                 | 原因                     |
| ------ | -------------------- | ------------------------ |
| `\mit` | 数学斜体（大写小写） | ❌ 非 KaTeX 内建命令      |
| `\scr` | 手写体（mathrsfs）   | ❌ 依赖额外宏包：mathrsfs |
---

> ✅ **建议：**
> - 在 Typora 中写公式时，优先使用 `\rm`, `\it`, `\bf`, `\sf`, `\tt`；
> - 若需更丰富字体控制，建议使用支持完整 LaTeX 的环境（如 Overleaf、TeX Live）；
> - 若渲染器为 MathJax v3，可通过扩展配置引入额外宏包支持如 `\mathbb`, `\mathscr` 等。
---
### 4、文字命令🧪
#### ① 注释文字 📝

> 使用 `\text{}` 命令在公式中添加可读性注释。  
> 推荐搭配 `\begin{cases}` 分段函数使用。

> **代码：**
> ```text
> $\text{文字}$
> ```

> **示例效果：**
> $$
> f(n) = \begin{cases}
> n/2, & \text{if $n$ is even} \\
> 3n, & \text{if $n$ is odd}
> \end{cases}
> $$

---

#### ② 文字颜色 🎨

> 兼容 **新旧浏览器** 的语法如下：

> **代码：**
> ```text
> $\color{red}{Hello}$
> ```

| 输入    | 显示                     | 输入   | 显示                    | 输入   | 显示                    |
| ------- | ------------------------ | ------ | ----------------------- | ------ | ----------------------- |
| black   | $\color{black}{color}$   | grey   | $\color{grey}{color}$   | silver | $\color{silver}{color}$ |
| white   | $\color{white}{color}$   | maroon | $\color{maroon}{color}$ | red    | $\color{red}{color}$    |
| yellow  | $\color{yellow}{color}$  | lime   | $\color{lime}{color}$   | olive  | $\color{olive}{color}$  |
| green   | $\color{green}{color}$   | teal   | $\color{teal}{color}$   | aqua   | $\color{aqua}{color}$   |
| blue    | $\color{blue}{color}$    | navy   | $\color{navy}{color}$   | purple | $\color{purple}{color}$ |
| fuchsia | $\color{fuchsia}{color}$ |        |                         |        |                         |

> ✅ **支持新版浏览器** 的 RGB 十六进制写法：

> **代码：**
> ```text
> $\color{#F00}{红色}$
> ```

| 输入 | 显示                  | 输入 | 显示                  | 输入 | 显示                  | 输入 | 显示                  |
| ---- | --------------------- | ---- | --------------------- | ---- | --------------------- | ---- | --------------------- |
| #000 | $\color{#000}{color}$ | #555 | $\color{#555}{color}$ | #AAA | $\color{#AAA}{color}$ | #FFF | $\color{#FFF}{color}$ |
| #F00 | $\color{#F00}{color}$ | #0F0 | $\color{#0F0}{color}$ | #00F | $\color{#00F}{color}$ | #FA0 | $\color{#FA0}{color}$ |
| #F5A | $\color{#F5A}{color}$ | #5A5 | $\color{#5A5}{color}$ | #A5F | $\color{#A5F}{color}$ | #AAF | $\color{#AAF}{color}$ |

---

#### ③ 删除线 ✂️

> 需要在顶部引入：
> ```text
> \require{cancel}
> ```

> **代码：**
> ```text
> $$
> \require{cancel}\begin{array}{r1}
> \verb|y+\cancel{x}|&y+\cancel{x}\\
> \verb|y+\cancel{y+x}|&y+\cancel{y+x}\\
> \verb|y+\bcancel{x}|&y+\bcancel{x}\\
> \verb|y+\xcancel{x}|&y+\xcancel{x}\\
> \verb|y+\cancelto{0}{x}|&y+\cancelto{0}{x}\\
> \verb+\frac{1\cancel9}{\cancel95}=\frac15+&\frac{1\cancel9}>{\cancel95}=\frac15\\
> \end{array}
> $$
> ```

> **示例效果：**
> ![能在Typora里面显示](https://i-blog.csdnimg.cn/direct/04e604b0cdcf48d99b4629612e3a7f95.png)

---

> 若需整段删除线，请引入：
> ```text
> \require{enclose}
> ```

> **代码：**
> ```text
> $$
> \require{enclose}\begin{array}{r1}
> \verb|\enclose{horizontalstrike}{x+y}|&\enclose{horizontalstrike}{x+y}\\
> \verb|\enclose{verticalstrike}{\frac xy}|&\enclose{verticalstrike}{\frac xy}\\
> \verb|\enclose{updiagonalstrike}{x+y}|&\enclose{updiagonalstrike}{x+y}\\
> \verb|\enclose{downdiagonalstrike}{x+y}|&\enclose{downdiagonalstrike
> {x+y}\\
> \verb|\enclose{horizontalstrike,updiagonalstrike}
> {x+y}|&\enclose{horizontalstrike,updiagonalstrike}{x+y}\\
> \end{array}
> $$

> **示例效果：**
> ![能在Typora里面显示](https://i-blog.csdnimg.cn/direct/e58a992cae764f61b6cfce7563e9879b.png)



### 5、大括号和行标 🧮

> 📘 **说明：**  
> LaTeX 中可以使用 `\left` 和 `\right` 自动调整括号高度，适配复杂嵌套结构（如分式、乘幂等）。可选的符号包括：
> - `\left(` `\right)` 圆括号
> - `\left[` `\right]` 方括号
> - `\left\{` `\right\}` 花括号（需转义）
> - `\left|` `\right|` 绝对值
> - `\left\langle` `\right\rangle` 内积符号
> - `\left.` `\right.` 空符号（常用于仅一侧括号）

---

#### ✅ 复杂嵌套括号示例

> **代码：**
> ```text
> $$
> f\left(
> \left[
>  \dfrac{1+\{x,y\}}
>  {
>    \left(\dfrac{x}{y}+\dfrac{y}{x}\right)(u+1)
>  } + a
> \right]^{\dfrac{3}{2}}
> \right)
> \tag{14.1}
> $$
> ```

> **效果：**
> $$
> f\left(
> \left[
> \dfrac{1+\{x,y\}}{\left(\dfrac{x}{y}+\dfrac{y}{x}\right)(u+1)} + a
> \right]^{\dfrac{3}{2}}
> \right)
> \tag{14.1}
> $$

---

#### 📐 使用 `\middle` 自定义中间分隔符

> 可用于多重分隔结构中的中间位置，如条件概率、量子力学态矢。

> **代码：**
> ```text
> $$
> \left\langle q \middle\| 
> \dfrac{\dfrac{x}{y}}{\dfrac{u}{v}} 
> \middle| p \right\rangle
> \tag{14.2}
> $$
> ```

> **效果：**
> $$
> \left\langle q \middle\| 
> \dfrac{\dfrac{x}{y}}{\dfrac{u}{v}} 
> \middle| p \right\rangle
> \tag{14.2}
> $$
> ✅ 建议在 Typora 或 MathJax 中使用时保持结构完整，并避免遗漏 `\left` 与 `\right` 配对，否则会导致渲染错误。

---
### 6、配置行高 📏

> 💡 **说明：**  
> 在 LaTeX 的多行公式中，可以使用 `\\[nex]` 的方式为当前行与下一行之间插入额外的垂直间距。  
> 其中 `ex` 表示当前字体中小写字母 `x` 的高度，常用于调整多行公式的视觉效果和可读性。

---

#### ✅ 使用 `[2ex]` 进行行间距适配

> **代码：**
> ```text
> $$
> f(n) =
> \begin{cases}
> \dfrac{n}{2}, & \text{if $n$ is even} \\[2ex]
> 3n + 1, & \text{if $n$ is odd}
> \end{cases}
> \tag{适配 [2ex]}
> $$
> ```

> **效果：**
> $$
> f(n) =
> \begin{cases}
> \dfrac{n}{2}, & \text{if $n$ is even} \\[2ex]
> 3n + 1, & \text{if $n$ is odd}
> \end{cases}
> \tag{A}
> $$

---

#### ❌ 默认 `\\` 无适配效果

> **代码：**
> ```text
> $$
> f(n) =
> \begin{cases}
> \dfrac{n}{2}, & \text{if $n$ is even} \\
> 3n + 1, & \text{if $n$ is odd}
> \end{cases}
> \tag{不适配 [2ex]}
> $$
> ```

> **效果：**
> $$
> f(n) =
> \begin{cases}
> \dfrac{n}{2}, & \text{if $n$ is even} \\
> 3n + 1, & \text{if $n$ is odd}
> \end{cases}
> \tag{B}
> $$

---

### 📐 常用间距单位说明

| 单位  | 含义                  | 示例      | 效果说明                     |
| ----- | --------------------- | --------- | ---------------------------- |
| `1ex` | 当前字体中 `x` 的高度 | `\\[1ex]` | 插入约一个字母高度的空隙     |
| `2ex` | 两倍 `x` 高度         | `\\[2ex]` | 常用于较明显的换行区分       |
| `3ex` | 三倍 `x` 高度         | `\\[3ex]` | 行间更加分明（演示、注解等） |
| `1em` | 当前字体中 `M` 的宽度 | `\\[1em]` | 通常比 `ex` 更宽             |

> 📝 若需要更精细控制间距，可使用 `\vspace{}` 命令或在环境外手动设定垂直距离。
---

### 7、交换图表（Commutative Diagrams）🔁

> 📘 **说明：**  
> 交换图用于展示对象之间的映射关系，常见于代数结构、函数复合、同态映射等领域。  
> 使用 `\require{AMScd}` 加上 `\begin{CD}...\end{CD}` 可快速绘制对齐整齐的交换图。

---

#### ✅ 函数复合交换图示例

> **代码：**
> ```text
> $$
> \require{AMScd}
> \begin{CD}
> X @>f>> Y \\
> @V g VV     @V h VV \\
> Z @>>k> W
> \end{CD}
> $$
> ```

> **效果：**
> ![> $$
> \require{AMScd}
> \begin{CD}
> X @>f>> Y \\
> @V g VV     @V h VV \\
> Z @>>k> W
> \end{CD}
> $$](https://i-blog.csdnimg.cn/direct/0c3a3ed07a9149c4b42fa1f24b79a8d7.png)


> ✏️ 表示函数复合满足：$h \circ f = k \circ g$

---

#### 📐 箭头类型说明

| 指令   | 效果 | 用途说明             |
| ------ | ---- | -------------------- |
| `@>>>` | →    | 从左向右映射         |
| `@<<<` | ←    | 从右向左映射         |
| `@VVV` | ↓    | 从上向下映射         |
| `@AAA` | ↑    | 从下向上映射         |
| `@= `  | ⇒    | 恒等映射或自然等价   |
| `@|`   | ‖    | 保持不变映射（恒等） |
| `@.`   | 空白 | 留空位置无连线       |

---

#### 🔁 群同态交换图示例（含注释箭头）

> **代码：**
> ```text
> $$
> \begin{CD}
> G @>>> H @>{\text{quotient map}}>> H/N \\
> @.  @AAA                       @| \\
> K @= K @<<< L
> \end{CD}
> $$
> ```

> **效果：**
> $$
> \begin{CD}
> G @>>> H @>{\text{quotient map}}>> H/N \\
> @.  @AAA                       @| \\
> K @= K @<<< L
> \end{CD}
> $$

---

#### 📌 提示与补充

- **数学意义**：图中路径若满足合成函数结果一致，则称该图“交换”（commutes）。
- **支持嵌套**：可嵌套多行结构构造复合映射。
- **与 `TikZ` 区别**：`CD` 适合快速公式排版，`TikZ` 适合绘制复杂结构图形。

---

#### 🧮 拓展应用（如线性变换）

> **代码：**
> ```text
> $$
> \begin{CD}
> \mathbb{R}^2 @>{T}>> \mathbb{R}^2 \\
> @V{\text{rotate}}VV     @VV{\text{scale}}V \\
> \mathbb{R}^2 @>>{S}> \mathbb{R}^2
> \end{CD}
> $$
> ```

> **效果：**
> $$
> \begin{CD}
> \mathbb{R}^2 @>{T}>> \mathbb{R}^2 \\
> @V{\text{rotate}}VV     @VV{\text{scale}}V \\
> \mathbb{R}^2 @>>{S}> \mathbb{R}^2
> \end{CD}
> $$

---