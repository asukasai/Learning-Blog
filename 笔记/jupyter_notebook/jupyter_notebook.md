# jupyter notebook

## 一、什么是Jupyter Notebook

### 1. 简介

> Jupyter Notebook是基于网页的用于交互计算的应用程序。其可被应用于全过程计算：开发、文档编写、运行代码和展示结果。——[Jupyter Notebook官方介绍](https://link.jianshu.com/?t=https%3A%2F%2Fjupyter-notebook.readthedocs.io%2Fen%2Fstable%2Fnotebook.html)

简而言之，Jupyter Notebook是以网页的形式打开，可以在网页页面中**直接**编写代码和运行代码，代码的运行结果也会直接在代码块下显示。如在编程过程中需要编写说明文档，可在同一个页面中直接编写，便于作及时的说明和解释。

### 2. 组成部分

#### ① 网页应用

网页应用即基于网页形式的、结合了编写说明文档、数学公式、交互计算和其他富媒体形式的工具。**简言之，网页应用是可以实现各种功能的工具。**

#### ② 文档

即Jupyter Notebook中所有交互计算、编写说明文档、数学公式、图片以及其他富媒体形式的输入和输出，都是以文档的形式体现的。

这些文档是保存为后缀名为`.ipynb`的`JSON`格式文件，不仅便于版本控制，也方便与他人共享。

此外，文档还可以导出为：HTML、[LaTeX](https://so.csdn.net/so/search?q=LaTeX&spm=1001.2101.3001.7020)、PDF等格式。

### 3. Jupyter Notebook的主要特点

1. 编程时具有**语法高亮**、*缩进*、*tab补全*的功能。
2. 可直接通过浏览器运行代码，同时在代码块下方展示运行结果。
3. 以富媒体格式展示计算结果。富媒体格式包括：HTML，LaTeX，PNG，SVG等。
4. 对代码编写说明文档或语句时，支持Markdown语法。
5. 支持使用LaTeX编写数学性说明。

## 二、运行Jupyter Notebook

### 1. 启动

#### ① 默认启动

**直接打开**

在开始菜单中找到Anaconda3点击Jupyter Notebook

**在开始菜单中找到Anaconda3点击Anaconda Prompt输入以下命令：**

```undefined
jupyter notebook
```

**或者win+R输入cmd输入以下命令：**

```undefined
jupyter notebook
```

执行命令之后，在终端中将会显示一系列notebook的服务器信息，同时浏览器将会自动启动Jupyter Notebook。

> 注意：之后在Jupyter Notebook的所有操作，都请保持终端**不要关闭**，因为一旦关闭终端，就会断开与本地服务器的链接，你将无法在Jupyter Notebook中进行其他操作啦。

浏览器地址栏中默认地将会显示：`http://localhost:8888`。其中，“localhost”指的是本机，“8888”则是端口号。

如果你**同时**启动了多个Jupyter Notebook，由于默认端口“8888”被占用，因此地址栏中的数字将从“8888”起，每多启动一个Jupyter Notebook数字就加1，如“8889”、“8890”……

**指定端口启动**

如果你想自定义端口号来启动Jupyter Notebook，可以在终端中输入以下命令：

```cobol
jupyter notebook --port <port_number>
```

其中，“<port_number>”是自定义端口号，直接以数字的形式写在命令当中，数字两边不加尖括号“<>”。如：`jupyter notebook --port 9999`，即在端口号为“9999”的服务器启动Jupyter Notebook。

#### ② 指定文件启动

在你想要打开的文件夹中 **按住shift不动+点击鼠标右键** 选择在此处打开Power shell窗口输入以下命令：

```undifined
jupyter notebook
```

这样就能在指定文件夹中打开了

## 三、Jupyter Notebook快捷键

### 2. Jupyter Notebook笔记本的两种模式

#### ① 命令模式

- 命令模式将键盘命令与Jupyter Notebook笔记本命令相结合，可以通过键盘不同键的组合运行笔记本的命令。
- 按`esc`键进入命令模式。
- 命令模式下，单元格边框为灰色，且左侧边框线为蓝色粗线条。



命令模式

#### ② 编辑模式

- 编辑模式使用户可以在单元格内编辑代码或文档。
- 按`enter`或`return`键进入编辑模式。
- 编辑模式下，单元格边框和左侧边框线均为绿色。



编辑模式

### 3. 两种模式的快捷键

==在命令模式下按h即可查看以下所有快捷键==

#### 命令行模式（按 Esc 生效）编辑快捷键

F: 查找并且替换

Ctrl-Shift-F: 打开命令配置

Ctrl-Shift-P: 打开命令配置

Enter: 进入编辑模式

P: 打开命令配置

**Shift-Enter: 运行单元格, 选择下面的单元格**

**Ctrl-Enter: 运行选中的单元格**

**Alt-Enter: 运行单元格并且在下面插入单元格**

**Y: 把单元格变成代码快**

**M: 把单元格变成 Markdown**

R: 清除单元格格式

1: 把单元格变成标题 1

2: 把单元格变成标题 2

3: 把单元格变成标题 3

4: 把单元格变成标题 4

5: 把单元格变成标题 5

6: 把单元格变成标题 6

K: 选择上面的单元格

上: 选择上面的单元格

下: 选择下面的单元格

J: 选择下面的单元格

Shift-K: 扩展上面选择的单元格

Shift-上: 扩展上面选择的单元格

Shift-下: 扩展下面选择的单元格

Shift-J: 扩展下面选择的单元格

Ctrl-A: select all cells

**A: 在上面插入单元格**

**B: 在下面插入单元格**

**X: 剪切选择的单元格**

**C: 复制选择的单元格**

Shift-V: 粘贴到上面

V: 粘贴到下面

Z: 撤销删除单元格

**D,D: 删除选中单元格**

Shift-M: 合并选中单元格, 如果只有一个单元格被选中

Ctrl-S: 保存并建立检查点

S: 保存并建立检查点

L: 切换行号

O: 显示/隐藏选定单元格的输出

Shift-O: 切换选中单元格的输出为滚动

H: 显示键盘快捷键

I,I: 中断内核

0,0: 重启内核（带确认对话框）

Esc: 关闭分页器

Q: 关闭分页器

Shift-L: 在所有单元格中切换行号，并保持设置

Shift-空格: 向上滚动

空格: 向下滚动

#### 编辑模式（按 Enter 生效）

**Tab: 代码补全或缩进**

Shift-Tab: 工具提示

Ctrl-]: 缩进

Ctrl-[: 取消缩进

Ctrl-A: 全选

Ctrl-Z: 撤销

Ctrl-/: 注释

Ctrl-D: 删除整行

Ctrl-U: 撤销选择

Insert: 切换重写标志

Ctrl-Home: 跳到单元格起始处

Ctrl-上: 跳到单元格起始处

Ctrl-End: 跳到单元格最后

Ctrl-下: 跳到单元格最后

Ctrl-左: 往左跳一个单词

Ctrl-右: 往右跳一个单词

Ctrl-退格: 删除前面的单词

Ctrl-Delete: 删除后面的单词

Ctrl-Y: 重做

Alt-U: 重新选择

Ctrl-M: 进入命令行模式

Ctrl-Shift-F: 打开命令配置

Ctrl-Shift-P: 打开命令配置

**Esc: 进入命令行模式**

**Shift-Enter: 运行单元格, 选择下面的单元格**

**Ctrl-Enter: 运行选中的单元格**

**Alt-Enter: 运行单元格并且在下面插入单元格**

Ctrl-Shift-Minus: split cell at cursor(s)

Ctrl-S: 保存并建立检查点

下: 光标下移

上: 光标上移
