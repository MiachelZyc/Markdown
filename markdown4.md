## 🛠 一. 使用的软件

![Typora](https://i-blog.csdnimg.cn/direct/616a4fcba7624ad1a1b2149c3fc68f40.webp#pic_center)

> 💡 **软件版本说明**：
>
> - 使用软件：**Typora v1.9.5**
> - 使用方法：推荐参考以下教程（由 CSDN 大佬整理）
>
> 🔗 [教程地址（Markdown实战）](https://blog.csdn.net/qq_61621323/article/details/141036982)

---

## 🔗 上期内容 & 项目地址

> 📚 **推荐阅读**：  
> 👉 [Markdown 结合 Typora 基础使用（1）](https://blog.csdn.net/2302_77872181/article/details/149306936)  
> 👉 [Markdown 结合 Typora 基础使用（2）](https://blog.csdn.net/2302_77872181/article/details/149308824)
> 👉 [Markdown 结合 Typora 基础使用 —— 数学公式（3）](https://blog.csdn.net/2302_77872181/article/details/149314933)

> 💻 **源码仓库地址**：  
> 👉 [GitHub：Markdown-Examples](https://github.com/MiachelZyc/Markdown)  
> 📄 本章文件名：markdown4.md

🌟 **如果本项目对你有所帮助，欢迎⭐Star 支持一下~**

---
## 📚二. markdown 数学公式（4）
### 🧊 1、矩阵表达形式

矩阵是数学公式中最常见的一类结构，Markdown 中通过 `\begin{matrix}` 环境构造，下面带你掌握常见矩阵写法：

---

#### ✅ ① 无边框矩阵（最基础）

>代码：
>```text
>$$
>\begin{matrix}
>1 & x & x^2 \\
>1 & y & y^2 \\
>1 & z & z^2 \\
>\end{matrix}
>$$
>```

>效果：  
$$
\begin{matrix}
1 & x & x^2 \\
1 & y & y^2 \\
1 & z & z^2 \\
\end{matrix}
$$

📌 **说明**：最简单的矩阵写法，不带任何括号或线框，适用于行列数据展示。

---

#### 🧱 ② 有边框矩阵（带不同类型括号）

只需将 `matrix` 替换为以下关键字即可：

| 语法          | 效果示例                                   | 括号说明   |
| ------------- | ------------------------------------------ | ---------- |
| `matrix`      | $\begin{matrix}1 & 2\\3 & 4\end{matrix}$   | 无括号     |
| `pmatrix`     | $\begin{pmatrix}1 & 2\\3 & 4\end{pmatrix}$ | 圆括号     |
| `bmatrix`     | $\begin{bmatrix}1 & 2\\3 & 4\end{bmatrix}$ | 方括号     |
| `Bmatrix`     | $\begin{Bmatrix}1 & 2\\3 & 4\end{Bmatrix}$ | 花括号     |
| `vmatrix`     | $\begin{vmatrix}1 & 2\\3 & 4\end{vmatrix}$ | 单竖线     |
| `Vmatrix`     | $\begin{Vmatrix}1 & 2\\3 & 4\end{Vmatrix}$ | 双竖线     |

📌 **提示**：适合不同应用场景，如**行列式**常用 `| |`、**向量内积**常用 `⟨ ⟩`。

---

#### ✂️ ③ 带分割线的矩阵（适合线性代数表达）

>代码：
>```text
>$$
>\left[
>\begin{array}{cc|c}
>1 & 0 & 3 \\
>0 & 1 & 5
>\end{array}
>\right]
>$$
>```

>效果：  
$$
\left[
\begin{array}{cc|c}
1 & 0 & 3 \\
0 & 1 & 5
\end{array}
\right]
$$

📌 **说明**：使用 `cc|c` 来定义列格式，其中 `|` 表示列之间插入一条竖线。常用于**增广矩阵**展示。

---

#### 🧾 ④ 行内小矩阵（适合公式中嵌入）

>代码：
>```text
>$\bigl( \begin{smallmatrix} a & b \\ c & d \end{smallmatrix} \bigr)$
>```

>效果：  
$\bigl( \begin{smallmatrix} a & b \\ c & d \end{smallmatrix} \bigr)$

📌 **说明**：
- 适合在文字或行内公式中插入小矩阵；
- 搭配 `\bigl( \bigr)` 实现自动缩放的圆括号。

---

🧠 **总结小贴士：**

- 所有矩阵行之间用 `\\` 分隔，列用 `&`；
- 括号自动缩放建议使用 `\left` 和 `\right`，例如：
$$
\left[
\begin{array}{cc}
a & b \\
c & d
\end{array}
\right]
$$

### 🧾 2、方程式序列（对齐、多行、编号）

在 Markdown 中使用 `align` 环境可以轻松创建**整齐对齐**的多行公式，还能支持自动编号、手动标注和标签引用等功能。

---

#### ✅ 基础示例：多行右对齐 + 自动编号

>代码：
>```text
>$$
>\begin{align}
>f(x) &= 1 + 1 \\
>     &= 2
>\end{align}
>$$
>```

>效果：
$$
\begin{align}
f(x) &= 1 + 1 \\
     &= 2
\end{align}
$$

---

#### 🔢 使用 `align*` 取消编号

>代码：
>```text
>$$
>\begin{align*}
>a &= b + c \\
>  &= d - e
>\end{align*}
>$$
>```

>效果：
$$
\begin{align*}
a &= b + c \\
  &= d - e
\end{align*}
$$

---

#### 🏷️ 使用 `\notag` 取消某一行编号，使用 `\label{}` 与 `\eqref{}` 引用公式编号

>代码（使用 `\tag{}` 替代 `\label{}`，兼容 KaTeX）：
>```latex
>$$
>\begin{align}
>\sqrt{37} &= \sqrt{\dfrac{73^2 - 1}{12^2}} \\
>          &= \sqrt{\dfrac{73^2}{12^2} \cdot \dfrac{73^2 - 1}{73^2}} \\
>          &= \sqrt{\dfrac{73^2}{12^2}} \cdot \sqrt{\dfrac{73^2 - 1}{73^2}} \notag \\
>          &= \dfrac{73}{12} \sqrt{1 - \dfrac{1}{73^2}} \\
>          &\approx \dfrac{73}{12} \left( 1 - \dfrac{1}{2 \cdot 73^2} \right) \tag{A}
>\end{align}
>$$
>```


>效果：
>$$
>\begin{align}
>\sqrt{37} &= \sqrt{\dfrac{73^2 - 1}{12^2}} \\
>          &= \sqrt{\dfrac{73^2}{12^2} \cdot \dfrac{73^2 - 1}{73^2}} \\
>          &= \sqrt{\dfrac{73^2}{12^2}} \cdot \sqrt{\dfrac{73^2 - 1}{73^2}} \notag \\
>          &= \dfrac{73}{12} \sqrt{1 - \dfrac{1}{73^2}} \\
>          &\approx \dfrac{73}{12} \left( 1 - \dfrac{1}{2 \cdot 73^2} \right) \tag{6}
>\end{align}
>$$

✅ 若要引用编号，请使用 `\tag{A}` 自定义编号，然后在正文中手动引用该编号，例如：

- 如公式（A）所示，...
- 由上式 A 可得，...
- 进一步推导见公式 `$\tag{A}$`

❗ 请注意：KaTeX **不支持** `\label{}`、`\eqref{}` 或 `\ref{}`，以下写法将导致错误：

- ❌ `\label{A}`
- ❌ `\eqref{A}`
- ❌ `\ref{A}`

📌 推荐做法：手动编号 + 手动引用，更加兼容 Markdown 环境（Typora、CSDN、Obsidian 等）。


---
#### 🧱 补充：带编号的矩阵可以用 `equation` 环境包裹

>代码：
>```text
>$$
>\begin{equation}
>\left[
>\begin{array}{cc|c}
>1 & 2 & 3 \\
>4 & 5 & 6
>\end{array}
>\right]
>\end{equation}
>$$
>```

>效果：
$$
\begin{equation}
\left[
\begin{array}{cc|c}
1 & 2 & 3 \\
4 & 5 & 6
\end{array}
\right]
\end{equation}
$$

---

📌 **总结重点**：

| 用法        | 效果说明                  |
|-------------|---------------------------|
| `align`     | 多行右对齐，自动编号     |
| `align*`    | 取消自动编号             |
| `\notag`    | 取消某一行编号           |
| `\label{}`  | 为公式打标签             |
| `\eqref{}`  | 带括号引用公式编号       |
| `alignat{1}`| 控制列宽，去除间距       |
| `equation`  | 强制编号单个公式/结构体 |

---
### 🧾3、数组与表格

>说明：  
>在公式中插入数组与表格结构，需使用 `\begin{array}` 环境，并在后面用字母控制每一列的格式：  
>  
> - `c`：居中对齐  
> - `l`：左对齐  
> - `r`：右对齐  
> - `|`：插入垂直分割线（列间）  
>  
>使用 `\\` 表示换行，`&` 表示列间分隔。使用 `\hline` 可在两行之间加入横向分割线。文本需使用 `\text{}` 包裹。

---

#### ✅ 示例一：常规对齐表格

>代码：
>```text
>$$
>\begin{array}{c|lcr}
>n & \text{左对齐} & \text{居中对齐} & \text{右对齐} \\
>\hline
>1 & 0.24 & 1     & 125       \\
>2 & -1   & 189   & -8        \\
>3 & -20  & 2000  & 1+10i
>\end{array}
>$$

>效果：
$$
\begin{array}{c|lcr}
n & \text{左对齐} & \text{居中对齐} & \text{右对齐} \\
>\hline
>1 & 0.24 & 1     & 125       \\
>2 & -1   & 189   & -8        \\
>3 & -20  & 2000  & 1+10i
>\end{array}
>$$

#### ✅ 示例二：纯居中无边框

>代码：
>```text
>$$
>\begin{array}{ccc}
>x & y & z \\
>1 & 2 & 3 \\
>4 & 5 & 6
>\end{array}
>$$

>效果：
>$$
>\begin{array}{ccc}
>x & y & z \\
>1 & 2 & 3 \\
>4 & 5 & 6
>\end{array}
>$$

#### ✅ 示例三：完全封闭式表格（加边框）
>代码：
>```text
>$$
>\begin{array}{|c|c|c|}
>\hline
>\text{编号} & \text{变量} & \text{含义} \\
>\hline
>1 & x & \text{长度} \\
>2 & y & \text{宽度} \\
>3 & z & \text{高度} \\
>\hline
>\end{array}
>$$

>效果：
>$$
>\begin{array}{|c|c|c|}
>\hline
>\text{编号} & \text{变量} & \text{含义} \\
>\hline
>1 & x & \text{长度} \\
>2 & y & \text{宽度} \\
>3 & z & \text{高度} \\
>\hline
>\end{array}
>$$

### 4、嵌套表格或数组

>📌说明：  
>使用多个 `array` 环境可以构建复杂嵌套的数组或表格结构。常用于展示多个矩阵在**行/列方向上并排或叠加**的场景，如评分对比、差异分析等。
>结构示意：  
>外层数组控制整体排布 → 内层数组分块显示内容 → 每个小表格均为标准 `array` 结构，可自定义对齐方式和边框线。

---

>🎯代码（学生成绩示例）：

>```text
>$$
>\begin{array}{c}  % 外层垂直排布的表格
>  \begin{array}{cc}  % 内层水平排列两个小表格
>    % 学生 A、B 的期末成绩矩阵
>    \begin{array}{c|cccc}
>      \textbf{学生 A} & 数学 & 语文 & 英语 & 物理 \\
>      \hline
>      一测 & 85 & 88 & 90 & 84 \\
 >     二测 & 87 & 90 & 91 & 85 \\
  >  \end{array}
  >  &
>    \begin{array}{c|cccc}
  >    \textbf{学生 B} & 数学 & 语文 & 英语 & 物理 \\
 >     \hline
   >   一测 & 82 & 85 & 88 & 86 \\
   >   二测 & 86 & 87 & 89 & 88 \\
  >  \end{array}
 > \end{array}
>  \\[1em]  % 上下间距
>  % 下方为成绩波动矩阵（分差）
>  \begin{array}{c|cccc}
>    \textbf{成绩变化 Δ} & 数学 & 语文 & 英语 & 物理 \\
>    \hline
 >   A & +2 & +2 & +1 & +1 \\
>    B & +4 & +2 & +1 & +2
 > \end{array}
>\end{array}
>$$

>效果：

>$$
\begin{array}{c}  % 外层垂直排布的表格
  \begin{array}{cc}  % 内层水平排列两个小表格
    % 学生 A、B 的期末成绩矩阵
    \begin{array}{c|cccc}
      \textbf{学生 A} & 数学 & 语文 & 英语 & 物理 \\
      \hline
      一测 & 85 & 88 & 90 & 84 \\
      二测 & 87 & 90 & 91 & 85 \\
    \end{array}
    &
    \begin{array}{c|cccc}
      \textbf{学生 B} & 数学 & 语文 & 英语 & 物理 \\
      \hline
      一测 & 82 & 85 & 88 & 86 \\
      二测 & 86 & 87 & 89 & 88 \\
    \end{array}
  \end{array}
  \\[1em]  % 上下间距
  % 下方为成绩波动矩阵（分差）
  \begin{array}{c|cccc}
    \textbf{成绩变化 Δ} & 数学 & 语文 & 英语 & 物理 \\
    \hline
    A & +2 & +2 & +1 & +1 \\
    B & +4 & +2 & +1 & +2
  \end{array}
\end{array}
$$

### 5、方程组

> 📌 **说明**：  
> 在数学公式中，使用 `\left\{...\right.` 搭配 `array` 环境可以清晰表示一个带左大括号的方程组。  
> 如果是分段函数或条件表达式，推荐使用 `cases` 环境，它格式更紧凑，适合表示**特定条件下的多种定义情况**。

---

> 🎯 **示例代码（线性方程组）**：

> ```text
> $$
> \left\{
> \begin{array}{l}
> 2x + 3y - z = 5 \\
> 4x - y + 2z = 6 \\
> -3x + 2y + z = -4
> \end{array}
> \right.
> \quad\text{或用}\quad
> \begin{cases}
> 2x + 3y - z = 5 \\
> 4x - y + 2z = 6 \\
> -3x + 2y + z = -4
> \end{cases}
> $$

>效果：
>$$
\left\{
\begin{array}{l}
2x + 3y - z = 5 \\
4x - y + 2z = 6 \\
-3x + 2y + z = -4
\end{array}
\right.
\quad\text{或用}\quad
\begin{cases}
2x + 3y - z = 5 \\
4x - y + 2z = 6 \\
-3x + 2y + z = -4
\end{cases}
$$

### 6、连分式（Continued Fractions）

> **说明：**  
> 连分式是以分数嵌套的形式表达一个数值的数学记号。为了保持公式的垂直对齐和可读性，应使用 `\cfrac`（或`\dfrac`）代替普通的 `\frac`，以获得更清晰的展示效果。若使用`\frac`会导致视觉混乱，特别是在嵌套较多层级时。

---

#### ✅ 正确用法（推荐使用 `\cfrac`）

> **代码：**
> ```text
> $$
> x = a_0 + \cfrac{b_1}{a_1 + \cfrac{b_2}{a_2 + \cfrac{b_3}{a_3 + \cfrac{b_4}{a_4 + \cdots}}}}
> $$
> ```

> **效果：**
> $$
> x = a_0 + \cfrac{b_1}{a_1 + \cfrac{b_2}{a_2 + \cfrac{b_3}{a_3 + \cfrac{b_4}{a_4 + \cdots}}}}
> $$

---

#### ❌ 错误用法（避免使用 `\frac`）

> **代码：**
> ```text
> $$
> x = a_0 + \frac{b_1}{a_1 + \frac{b_2}{a_2 + \frac{b_3}{a_3 + \frac{b_4}{a_4 + \cdots}}}}
> $$
> ```

> **效果：**
> $$
> x = a_0 + \frac{b_1}{a_1 + \frac{b_2}{a_2 + \frac{b_3}{a_3 + \frac{b_4}{a_4 + \cdots}}}}
> $$

---

#### 📌 紧缩记法（适合简洁表达）

> **代码：**
> ```text
> $$
> x = a_0 + \frac{b_1}{a_1 +} \frac{b_2}{a_2 +} \frac{b_3}{a_3 +} \frac{b_4}{a_4 +} \cdots
> $$
> ```

> **效果：**
> $$
> x = a_0 + \frac{b_1}{a_1 +} \frac{b_2}{a_2 +} \frac{b_3}{a_3 +} \frac{b_4}{a_4 +} \cdots
> $$

---

#### 🎯 示例替换（以具体数值替代参数）

> **代码：**
> ```text
> $$
> \pi = 3 + \cfrac{1^2}{6 + \cfrac{3^2}{6 + \cfrac{5^2}{6 + \cfrac{7^2}{6 + \cdots}}}}
> $$
> ```

> **效果：**
> $$
> \pi = 3 + \cfrac{1^2}{6 + \cfrac{3^2}{6 + \cfrac{5^2}{6 + \cfrac{7^2}{6 + \cdots}}}}
> $$