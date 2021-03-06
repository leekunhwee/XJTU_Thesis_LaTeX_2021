<div align = "center">
<img src = ".\image\latex-project-logo.png"  width=80%>
</div>


# 西安交通大学硕博论文LaTeX模板 XJTU_Thesis_LaTeX_2021
- ## Thesis LaTeX Template of Xi'an Jiaotong University
  - #### Master: Master Thesis LaTeX Template of Xi'an Jiaotong University
  - #### PhD: Doctoral Thesis LaTeX Template of Xi'an Jiaotong University

#### 本模板使用教程亦可见于：<b>[硕博学位论文 $\LaTeX$ 模板及其使用教程](https://zhuanlan.zhihu.com/p/388415963 "硕博学位论文 LaTeX 模板及其使用教程")</b>

<br>

## 目录 Table of Contents:

-  [前言](#前言)
-  [软件安装与环境配置](#软件安装与环境配置)
-  [编译运行方法](#编译运行方法)
-  [常见问题及解决方法](#常见问题及解决方法)

<br>



# 前言

为了避免学位论文撰写后期因文件过大而导致 `MS Word` 打开速度过慢或卡死、以及内容格式控制困难等问题，本人一开始就毅然决然地选择了用 $\LaTeX$ 完成博士学位论文的撰写工作。

但是在学位论文的撰写过程中，由于没有一个对应的详细使用教程，所以遇到了不少问题。经过长期的探索与试错，基本将使用 $\LaTeX$] 撰写论文中可能遇到的问题都一一解决。

本人就读于西安交通大学，在完成论文撰写工作后，遵从西安交通大学最新版（$2021$ 版）之规范，并借鉴其他多所大学的硕博学位论文之 $\LaTeX$ 模板，在原始模板（$2018$ 版）的基础之上加以补充、修正，得到了最新的西安交通大学硕博学位论文 $\LaTeX$ 模板，并将环境配置方法以及常见问题的解决方法总结为此教程。

其他学校的知友亦可以将本模板及教程作为练习使用 $\LaTeX$ 撰写硕博学位论文的参考材料。

点击此页面上名为 `Code` 的绿色按钮，然后点击 `Download ZIP` 即可下载本模板的源文件，如下图所示。
<div align = "center">
<img src = ".\image\download.png"  width=60% alt = "GitHub 上模板源文件的下载界面" title = "GitHub 上模板源文件的下载界面">
</div>
<p align = "center"><b>GitHub 上模板源文件的下载界面</b></p>


将下载得到的模板源文件压缩包解压到一个文件夹中。（注意：该文件夹的路径中千万不要出现中文或其他特殊字符，否则将给论文的编撰带来极大的不便。）

<br>

# 软件安装与环境配置

本教程所用模板在 `Windows` + `MikTeX` + `Texmaker` 平台下开发，并采用 `XeLaTeX` 编译。

在编辑文档前需要安装两个软件，即 `MikTeX` 和 `Texmaker`。`MikTeX` 是当下较为流行的一款免费且跨平台的 $\LaTeX$ 系统发行版本，其提供了 $\LaTeX$ 语言的运行环境，并能够按需下载宏包，实现了占用资源量最小；`Texmaker` 则是一款免费且跨平台的编辑器，其能够设置各种快捷键，实现轻松、高效的编辑。

这两款软件均为跨平台免费软件，所以本教程不仅适用于 `Windows` 系统，同样也适用于 `MacOS` 和 `Linux` 系统。这两款软件的下载地址分别为：

- ### [MikTeX 下载链接](https://miktex.org/download "MikTeX 下载链接")

- ### [Texmaker 下载链接](https://www.xm1math.net/texmaker/download.html "Texmaker 下载链接") （初次下载的 Windows 用户建议下载后缀为 .msi 的版本）

 <em>由于安装过程较为简单，这里不再详细叙述，只需要注意安装路径中不要出现中文或其他特殊字符。</em>

安装完成后，分别对两款软件进行配置。

## MikTeX 的配置

将 `MikTeX` 中的软件包更新到最新版本，方法是以管理员模式打开 `MiKTeX Console` ：
<div align = "center">
<img src = ".\image\MikTeX.png"  width=60% alt = "以管理员模式打开 MiKTeX Console" title = "以管理员模式打开 MiKTeX Console">
</div>
<p align = "center"><b>以管理员模式打开 MiKTeX Console</b></p>

然后点击 `Check for updates`：
<div align = "center">
<img src = ".\image\check.png" width=60% alt = "检测更新" title = "检测更新">
</div>
<p align = "center"><b>检测更新</b></p>

最后选择 `Updates`，点击其中的 `Update now`，等待其更新完毕即可：
<div align = "center">
<img src = ".\image\update.png"  width=60% alt = "现在更新" title = "现在更新">
</div>
<p align = "center"><b>现在更新</b></p>



## Texmaker 的配置

`Texmaker` 打开后的界面如下：
<div align = "center">
<img src = ".\image\texmaker.png"  width=60% alt = "Texmaker 软件界面" title = "Texmaker 软件界面">
</div>
<p align = "center"><b>Texmaker 软件界面</b></p>

如果界面不同，可以在顶部菜单栏的 `查看` 选项中进行修改，如上图所示。

`Texmaker` 的配置关键在于一些除默认配置以外的快捷键自定义设置。这里将其分成四块，分别是：**文本定位快捷键**、**编译运行快捷键**、**主要符号表快捷键**和**参考文献快捷键**。

<br>

- ### 文本定位快捷键
$\LaTeX$ 与 `MS Word` 最大的不同之处就在于其文本与效果是分离的。这样的好处是在模板确定的情况下，只需要专注于内容，而不用担心字体和格式出错；麻烦之处就是查看区与编辑区分离，所以需要将两个区域快速对应起来。

 - **PDF -> 文本**：`Texmaker` 默认可以通过 `Ctrl+鼠标左键` 的方式从 PDF 文件跳转并定位到其对应的文本位置。（如果不行，极有可能是因为文档的存放路径中包含了中文或其他特殊字符）

 - **文本 -> PDF**：这是一个可以自定义的快捷键，通过`Ctrl+，`或者“`选项`-`配置Texmaker`”可以打开配置界面，在右下角一个很隐蔽的地方有一个选项，如下图：

<div align = "center">
<img src = ".\image\switch.png"  width=60% alt = "切换定位快捷键" title = "切换定位快捷键">
</div>
<p align = "center"><b>切换定位快捷键</b></p>

我设定的是 `Alt+B`，当然也可以换成自己喜欢的快捷键，只要不发生冲突就行，这样就可以通过该快捷键从光标所在的文本处跳转到其在 PDF 文件上的对应位置。

<br>


- ### 编译运行快捷键

由于学位论文中包含中文，所以这里需要用 `XeLaTeX` 进行编译，为了实现快速编译，将快速构建命令选定为 `XeLaTeX + View PDF`，如下图：
<div align = "center">
<img src = ".\image\run.png"  width=60% alt = "编译运行快捷键" title = "编译运行快捷键">
</div>
<p align = "center"><b>编译运行快捷键</b></p>

这样设置之后，只需要按 `F1` 键就可以完成主体内容的编译，并将结果以 PDF 的格式输出查看。

<br>

- ### 主要符号表快捷键

对于公式较多的理工类学位论文，主要符号表就显得很有必要了，但是符号表和主体内容不是同步编译的，如果想要在目录之后紧接着显示主要符号表，就需要自定义一个命令。

点击顶部菜单栏 “`自定义`-`自定义命令`-`编辑自定义命令`”，在菜单项中填写 `MAKEINDEX`，在命令中填写以下命令并保存：
```
makeindex %.nlo -s nomencl.ist -o %.nls
```

如下图所示：
<div align = "center">
<img src = ".\image\command.png"  width=60% alt = "主要符号表快捷键" title = "主要符号表快捷键">
</div>
<p align = "center"><b>主要符号表快捷键</b></p>

这样，通过 `Shift+Alt+F1` 就可以生成主要符号表的格式化文件 `main.nls`。

注意：模板源文件中的主要符号表文本文件是位于模板源文件 `setup` 文件夹中的 `nomenclature.tex`，而且只有先通过 `F1` 编译主文件并在根文件夹中生成 `main.nlo` 文件之后，才可以正常使用 `Shift+Alt+F1` 命令。

在使用 `Shift+Alt+F1` 命令之后，会在根文件夹中生成主要符号表的格式化文件 `main.nls`。在此情况下，再次使用 `F1` 编译一遍，就可以将主要符号表里的内容插入到目录之后。

`Shift+Alt+F1` 命令只有在主要符号表未生成，或者主要符号表的内容发生改变的情况下才需要重新运行。

<br>

- ### 参考文献快捷键

与主要符号表类似，参考文献和主体内容也不是同步编辑的，其默认的快捷键是 `F11`，如下图所示：
<div align = "center">
<img src = ".\image\reference.png"  width=60% alt = "参考文献快捷键" title = "参考文献快捷键">
</div>
<p align = "center"><b>参考文献快捷键</b></p>

按 `F11` 键可以生成参考文献的格式化文件 `main.bbl`。

注意：模板源文件中的参考文献文本文件是位于模板源文件 `bib` 文件夹中的 `mybib.bib`，而且只有先通过 `F1` 编译主文件并在根文件夹中生成 `main.aux` 文件之后，才可以正常使用 `F11` 命令。

在使用 `F11` 命令之后，会在根文件夹中生成参考文献的格式化文件 `main.bbl`。在此情况下，再次使用 `F1` 编译一遍，就可以将参考文献内容插入到主要章节之后。但此时的参考文献是不包含编号的，不过没有关系，只需要再次按一下 `F1` 键完成编译，即可生成编号。

`F11` 命令只有在参考文献未生成，或者参考文献的内容发生改变的情况下才需要重新运行。

<br>

# 编译运行方法
在 `Texmaker` 中打开模板源文件中的 `main.tex` 文件或直接双击 `main.tex` 文件（硕士学位论文的模板文件位于 `Master` 文件夹中；博士学位论文的模板文件位于 `PhD` 文件夹中），紧接着按 `Ctrl+0` 或者点击顶部菜单栏 “`选项`-`设置当前文档为主文档`”。（这一步非常关键，因为如果不设置 `main.tex` 文件为主文档，那么就不能在编辑除 `main.tex` 的其他章节时直接按 `F1` 键进行编译，而是必须要切换到 `main.tex` 的编辑界面。

也就是说，一旦设置了主文档，不管正在编辑的是哪一个章节的内容，只要按 `F1` 键，编译都是从主文档开始的，各个章节的内容相互独立但顺序与格式又由主文档统一控制，这使得编译过程更加清晰、简便。）

设置完主文档后，按 `F1` 键可以进行编译，并展示生成的 PDF 文档。注意：第一次运行时，系统会提示需要安装一些宏包以供编译使用，如下图：
<div align = "center">
<img src = ".\image\package.png" width=60% alt = "宏包自动下载" title = "宏包自动下载">
</div>
<p align = "center"><b>宏包自动下载</b></p>


为了避免窗口反复弹出，可以将上图中 `总是显示此对话框(A)` 前面的勾选去掉。

第一次运行由于安装宏包较多，所以需要较长的时间，请务必耐心等待，这取决于网速和电脑性能，之后的速度会快很多。

如果需要插入主要符号表，则需要在按 `F1` 键编译完成后再按`Shift+Alt+F1`，之后再按 `F1` 键得到包含主要符号表的论文。

如果需要插入参考文献，则需要在按 `F1` 键编译完成后再按 `F11` 键，之后再按 `F1` 键得到包含参考文献的论文，最后再按一次 `F1` 键为参考文献添加序号。

注意：在修改文本后，要记得随手保存。带超链接的内容，例如目录和图片、公式、表格等的编号，均是在按 `F1` 键编译完成后再按一次 `F1` 键编译才能完整、正确地输出，并且要等前一次编译运行完成后再进行第二次编译。

<br>

# 常见问题及解决方法


- ## **文本编辑区和 PDF 查看区之间无法实现跳转**
原因是文档所在路径中包含中文或其他特殊字符，需要改为英文路径。

<br>

- ## **当文本编辑器为除 main.tex 以外的其他章节时，按“F1”无法完成编译**
原因是未正确设置主文档，对于该模板，其主文档为 `main.tex` 文件。需要在 `Texmaker` 中打开 `main.tex` 文件，然后 `Ctrl+0` 或者点击顶部菜单栏“`选项`-`设置当前文档为主文档`”。

<br>

- ## **'xxx.sty' not found**
注意：这里拿 `tabularx.sty` 举个例子，如果出现其他类似于 not found 的情况，亦可以参考本方法，举一反三。
如果运行后消息框提示错误 `! LaTeX Error: File 'tabularx.sty' not found.`，说明此时系统缺少一个名称为 `tabularx.sty` 的宏包。需要做的就是以管理员模式打开 `MiKTeX Console`，然后点击 `宏包` 或 `packages`，在搜索栏中输入 `tabularx.sty` 并回车搜索，搜索结果如下图：
<div align = "center">
<img src = ".\image\search.png"  width=60% alt = "搜索宏包" title = "搜索宏包">
</div>
<p align = "center"><b>搜索宏包</b></p>
选择第一个，右击点击 `安装宏包` 即可解决该问题。

<br>

- ## **在前一次按“F1”编译完成前再次按了一下“F1”启动编译而导致异常**
此报错是因为第二次编译运行时，前一次编译尚未完成，导致两次生成的中间文件之间发生了同名冲突。这种情况是无法通过修改代码的方式解决的，必须要在保留源文件的前提下删除运行过程中生成的中间文件。
在根目录文件夹中有一个 `clean.bat` 文件可以一键解决该问题，只需要双击该文件，即可删除所有编译时所生成的中间文件。
只要代码中没有语法错误，清理完中间文件后再次按 `F1` 键即可顺利运行（注意：由于所有中间文件都删除了，主要符号表和参考文献也需要按照前面给的方法重新生成一遍）。

- ## **查看”菜单中缺少“PDF查看器”选项** 
“选项-配置Texmaker-命令-PDF查看器”，勾选“嵌入”复选框，重启软件即可。
