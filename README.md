# SUES-Paper
上海工程技术大学（SUES）学术型硕士毕业论文Latex模板（非官方，个人简单编辑版）

# 版权说明
本工程的证书是MIT，具体内容请自行搜索。

使用者的权利包括且不限于：复制、修改源代码代个人学习或组织商用。
如果使用遇到问题：可提Issue或者发邮件到作者邮箱：yjd2008@hotmail.com。当看到时Issue时，会尽量答复。但因Latex部分格式设置问题比较复杂，鼓励使用者先自行搜索解决问题，作者并不保证Issue一定能到解决，希望能一起探索解决。

# 测试环境：
- OS: windows 或 ubuntu。其余未测试，理论上不限制。
- 编辑器：VS Code + 插件 LaTex Extension Pack
- 编译器：Texlive2018以上经过测试，具体的使用的编译指令见 .vscode/settings.json。

# 使用说明：
- 章节：根目录下的 main.tex 文件负责整个工程的结构，其余的可编辑源文件在文件夹 chapters 下面，正文每章一个 tex 文件，除正文外每页一个 tex 文件。
- 图片：工程所用到的图片均放置在 images 文件夹下面。
- 参考文献：所有的使用的参考文献都在 refer.bib 文件内部，参考文献的格式是 GB/T 7714-2005。
- .vscode：设置了与 VS Code 插件相关的一些编译设置指令。
- latex_settings：设置工程中所需要的一些格式，即 Latex 中的引言区的设置。

# 编译说明
使用前请先按照：https://github.com/Haixing-Hu/GBT7714-2005-BibTeX-Style 中的说明进行参考文献格式 GB/T 7714-2005 的设定，否则会出现编译失败。既然选择了使用了 VS Code + Latex 写论文，就要先发挥不怕折腾的精神，按照上述链接的说明很简单就可以操作。

本工具链在.vscode/settings.json 中设置了两个编译指令：xelatex 和 xelatex ➞ bibtex ➞ xelatex ➞ xelatex。其中当参考文献项更新时，需要使用第二套编译指令，其余第一套即可。