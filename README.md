# 使用 PyCharm 编写 LaTeX ，并实现：自动编译生成 PDF 实时查看和公式实时预览
## 一、安装 TeX Live 和 PyCharm
### （一）安装 TeX Live
#### 　　　[https://www.latex-project.org/](https://www.latex-project.org/)
### （二）安装 PyCharm
#### 　　　[https://www.jetbrains.com/pycharm/](https://www.jetbrains.com/pycharm/)
## 二、安装 2 个 PyCharm 插件（ _TeXiFy IDEA_ 和 _PDF Viewer_ ）并调试
### （一）安装 TeXiFy IDEA 插件 [[点击此处查看图片]](https://github.com/FlorianGu/latex-on-pycharm/blob/main/README_picture/01.md)
#### 　　　打开 PyCharm → File → Settings → Plugins → Marketplace → 搜索“TeXiFy IDEA” → Install → Apply → OK
### （二）安装 PDF Viewer 插件 [[点击此处查看图片]](https://github.com/FlorianGu/latex-on-pycharm/blob/main/README_picture/02.md)
#### 　　　打开 PyCharm → File → Settings → Plugins → Marketplace → 搜索“PDF Viewer” → Install → Apply → OK
### （三）调试 [[点击此处查看图片]](https://github.com/FlorianGu/latex-on-pycharm/blob/main/README_picture/03.md)
#### 　　　1. 先创建一个 tex 文件，并按图中所示修改
#### 　　　2. Run → Edit Configurations → Edit configuration templates → LaTeX → “Compiler: XeLaTeX”
#### 　　　　→ “PDF viewer: Built-in PDF Viewer” → Apply → OK
#### 　　　3. 运行该 tex 文件，发现 PDF 正常显示且中文正常显示
#### 　　　4. 此时，TeXiFy IDEA 插件和 PDF Viewer 插件已全部配置完成，若无需以下二功能者，可不看以下内容
## 三、配置功能
### （一）配置“自动编译生成 PDF 实时查看” [[点击此处查看图片]](https://github.com/FlorianGu/latex-on-pycharm/blob/main/picture/09.png)
#### 　　　File → Settings → Languages & Frameworks → TeXiFy → 勾选“Automatic Compilation ..." → Apply → OK
### （二）配置“公式实时预览” [[点击此处查看图片]](https://github.com/FlorianGu/latex-on-pycharm/blob/main/picture/10.png)
#### 　　　File → Settings → Languages & Frameworks → TeXiFy → 勾选“Automatically refresh pre..." → Apply → OK
#### 　　　此时，还不能实现“公式实时预览”. 根据 _TeXiFy IDEA_ 官方文档要求，需进行如下操作：
#### 　　　（1）下载并安装  _Inkscape_  和  _pdf2svg_  两款软件
#### 　　　　　[https://inkscape.org/release](https://inkscape.org/release)
#### 　　　　　[https://github.com/textext/pdf2svg/releases](https://github.com/textext/pdf2svg/releases)
#### 　　　（2）将如上两款软件的安装目录添加到环境变量中 [[点击此处查看图片]](https://github.com/FlorianGu/latex-on-pycharm/blob/main/README_picture/04.md)
### _现在，LaTeX 可以通过 PyCharm 编写了，并且已实现相应功能_<br/><br/>
### 参考文献：
　● [ _TeXiFy IDEA_ 官方文档](https://github.com/Hannah-Sten/TeXiFy-IDEA/wiki/Preview#instructions-for-windows)<br/><br/>
_如有任何问题，欢迎[ **Issues** ](https://github.com/FlorianGu/climb-over-the-wall/issues) 或发送邮件 `floriangu2021@gmail.com`_
