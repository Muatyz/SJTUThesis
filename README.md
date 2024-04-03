### Overleaf

[![Overleaf](https://img.shields.io/badge/Overleaf-SJTUThesis-green.svg)](https://www.overleaf.com/latex/templates/sjtuthesis-latex-thesis-template-for-shanghai-jiao-tong-university/mkdwbyjbtfgg?r=sdkbtJ4qGS8kDZQQ&rm=d&rs=b)

点击 [链接](https://www.overleaf.com/latex/templates/sjtuthesis-latex-thesis-template-for-shanghai-jiao-tong-university/mkdwbyjbtfgg?r=sdkbtJ4qGS8kDZQQ&rm=d&rs=b) 即可直接使用。

如果需要在其他在线 LaTeX 平台上使用（比如 [latex.sjtu.edu.cn](https://latex.sjtu.edu.cn)），您可以下载 [最新版压缩包](https://github.com/sjtug/SJTUThesis/archive/refs/heads/master.zip)，然后上传至相应平台。请注意，Overleaf 默认使用 pdflatex 编译，您需要设置使用 XeLaTeX 编译器。

## 模板使用

如果你不熟悉 LaTeX 的编译流程，请**不要**直接使用编译器进行编译。针对不同的平台，模版提供了相应的编译脚本。在编译前，需要安装最新的 TeXLive 发行版。

### VSCode 用户

安装 “LaTeX Workshop” 后，选择 `Recipe: latexmk (xelatex)` 编译即可，并在设置中将 `latex-workshop.latex.recipe.default` 改为 `lastUsed` 以一直使用该选项编译。

### Windows 用户

对于 Windows 用户，我们也提供了编译脚本 `Compile.bat`。可以双击直接编译，也可以在命令提示符窗口中使用脚本提供的额外功能：

```bash
.\Compile.bat thesis          # 编译生成 main.pdf
.\Compile.bat clean           # 删除编译所产生的中间文件
.\Compile.bat cleanall        # 删除 main.pdf 和所有中间文件
.\Compile.bat wordcount       # 论文字数统计
```

更多关于模板的实现细节以及使用信息，请查看使用文档 `sjtuthesis.pdf`。
