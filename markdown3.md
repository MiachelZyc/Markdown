## 🛠一. 使用的软件

![Typora](https://i-blog.csdnimg.cn/direct/616a4fcba7624ad1a1b2149c3fc68f40.webp#pic_center)

> 💡 **软件版本说明**：
>
> - 使用软件：**Typora v1.9.5**
> - 使用方法：推荐参考以下教程（由 CSDN 博主整理）
>
> 🔗 [https://blog.csdn.net/qq_61621323/article/details/141036982](https://blog.csdn.net/qq_61621323/article/details/141036982)

## 🔗 上期内容 & 项目地址

> 📚 **上期推荐阅读**：  
> 👉 [Markdown 结合 Typora 基础使用（1）](https://blog.csdn.net/2302_77872181/article/details/149306936?spm=1001.2014.3001.5502)
> 👉 [Markdown 结合 Typora 基础使用（2）](https://blog.csdn.net/2302_77872181/article/details/149308824)

> 💻 **GitHub 源码仓库**：  
> 👉 [https://github.com/MiachelZyc/Markdown](https://github.com/MiachelZyc/Markdown)
> 👉本章对应markdown3.md

🌟 **如果你觉得本项目对你有帮助**，欢迎一键 `⭐Star` 支持，让更多人受益！
## 📚二. markdown 数学公式（3）

### 1、公式的插入

#### ① 行内公式（公式和文字在一行内）

>代码：
>```text
>$E=mc^2$
>```

>效果：  
>爱因斯坦著名的质能方程：$E=mc^2$

#### ② 独立公式（公式单独一行，居中显示）

>代码：
>```text
>$$
>\int_0^1 x^2\,dx = \frac{1}{3}
>$$
>```

>效果：  
$$
\int_0^1 x^2\,dx = \frac{1}{3}
$$

---

### 2、上下标写法

#### ① 常见上下标公式（指数、变量表示）

>代码：
>```text
>$v_{avg} = \frac{s}{t}$  
>$a^{2t+1}$
>```

>效果：  
>$v_{avg} = \frac{s}{t}$  
>$a^{2t+1}$

#### ② 高阶复杂上下标（仅进阶用户使用）

>代码：
>```text
>$\mathop{}^{a}_{b}\!\!\sum\limits^{c}_{d}$
>$x^{y^z}_{n_k}$
>```

>效果：  
>$\mathop{}^{a}_{b}\!\!\sum\limits^{c}_{d}$
>$x^{y^z}_{n_k}$

---

### 3、括号和分隔符（逐项分开展示）

#### ① 角括号（常用于内积符号）

>代码：
>```text
>$\langle x \rangle$
>```

>效果：  
>$\langle x \rangle$

---

#### ② 向上取整符号（ceil）

>代码：
>```text
>$\lceil x \rceil$
>```

>效果：  
>$\lceil x \rceil$

---

#### ③ 向下取整符号（floor）

>代码：
>```text
>$\lfloor x \rfloor$
>```

>效果：  
>$\lfloor x \rfloor$

---

#### ④ 花括号（常用于集合）

>代码：
>```text
>$\lbrace x \rbrace$
>```

>效果：  
>$\lbrace x \rbrace$

---

#### ⑤ 双竖线（表示模或范数）

>代码：
>```text
>$\lVert x \rVert$
>```

>效果：  
>$\lVert x \rVert$


### 4、分数表达（常用于代数或微积分）

>代码：
>```text
>$\frac{a}{b} \quad \dfrac{a}{b} \quad {a\over b}$
>```

>效果：  
>$\frac{a}{b} \quad \dfrac{a}{b} \quad {a\over b}$

>说明：  
>- `\frac`：普通行内分数  
>- `\dfrac`：强制显示为独立分数（更大更清晰）  
>- `{a\over b}`：更简洁的写法  

---

### 5、开方（平方根、立方根等）

>代码：
>```text
>$\sqrt{2} \quad \sqrt[3]{x+1}$
>```

>效果：  
>$\sqrt{2} \quad \sqrt[3]{x+1}$

>说明：  
>- `\sqrt{}` 表示平方根  
>- `\sqrt[n]{}` 表示 n 次方根（例如立方根 n=3）

---
### 6、极限表达（极限操作是高数中的重点）

>代码：
>```text
>$\lim\limits_{x \to 0} \dfrac{\sin x}{x} = 1$
>```

>效果：  
>$\lim\limits_{x \to 0} \dfrac{\sin x}{x} = 1$

---

### 7、积分表达（包含重积分与曲线积分）

>代码：
>```text
>$$
>\iint\limits_{R} (x^2 + y^2)\, \mathrm{d}x\,\mathrm{d}y = \oint\limits_{\partial R} x\,\mathrm{d}y - y\,\mathrm{d}x
>$$
>```

>效果：  
$$
\iint\limits_{R} (x^2 + y^2)\, \mathrm{d}x\,\mathrm{d}y = \oint\limits_{\partial R} x\,\mathrm{d}y - y\,\mathrm{d}x
$$

---

### 8、累加、累乘、并集与交集符号

>代码：
>```text
>$\sum\limits_{k=1}^{n} k^2 \quad
>\prod\limits_{i=1}^{n} i \quad
>\bigcup\limits_{i=1}^{n} A_i \quad
>\bigcap\limits_{i=1}^{n} B_i$
>```

>效果：  
>$\sum\limits_{k=1}^{n} k^2 \quad
>\prod\limits_{i=1}^{n} i \quad
>\bigcup\limits_{i=1}^{n} A_i \quad
>\bigcap\limits_{i=1}^{n} B_i$

---

### 9、省略号（用于表示省略的数列、矩阵等）

>代码：
>```text
>$\cdots$  // 横向居中省略号（常用于表达式中间）  
>$\ldots$  // 水平底部省略号（常用于向量、坐标列）  
>$\vdots$  // 垂直省略号（常用于矩阵中）  
>$\ddots$  // 对角省略号（矩阵对角线方向）
>```

>效果：  
>$\cdots \quad \ldots \quad \vdots \quad \ddots$

---

### 10、矢量与均值符号（向量方向与平均值常用写法）

>代码：
>```text
>$\vec{a} \quad \overrightarrow{AB} \quad \overline{x} = \bar{x} \quad \underline{x}$
>```

>效果：  
>$\vec{a} \quad \overrightarrow{AB} \quad \overline{x} = \bar{x} \quad \underline{x}$