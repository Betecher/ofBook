ofBook
======

*All articles copy from [ofBook](https://github.com/openframeworks/ofBook)*

所有文章全都是从[ofBook](https://github.com/openframeworks/ofBook)拷贝过来的。
主要是想把这些文章翻译成中文，方便让国内朋友查看。

原教程是大家合作撰写的openFrameworks教程。  

其他语言：
- English(英文) : [README.md](README.md)
- Korean(한국어) : [README.ko.md](README.ko.md)

**原教程还在继续撰写中**


# 编译步骤

需要安装

- [LaTeX](http://www.latex-project.org/)
- [pandoc](http://johnmacfarlane.net/pandoc/)
- [python 2.7+](https://www.python.org/)
- [beauitful soup 4](http://www.crummy.com/software/BeautifulSoup/)
- [sass](http://sass-lang.com/)
- [libsass](https://github.com/dahlia/libsass-python)

编译成网页版和PDF版的脚本文件是在`scirpts/`目录下的
`createWebBook.py` 和 `createPDFBook.py`.  编译时必须在`scripts/`下运行, 双击运行或者在终端下运行脚本文件.
- 编译完网页版以后所有文件会在`output/webBook`目录下生成. `output/webBook/index.html`文件是网页版的主文件，用浏览器访问就好.
- 编译完PDF版以后，PDF文件会在`output/ofBook.pdf`. 为了调试`output/ofBook.tex`也会一起创建.

## 在 OS X 安装依赖包
1. 在终端安装pip ```sudo easy_install pip```
2. 安装 [beauitful soup 4](http://www.crummy.com/software/BeautifulSoup/) (bs4) `pip install beautifulsoup4`
3. 安装 [pandoc](https://github.com/jgm/pandoc/releases)
4. 安装 [basictex & MacTeX-Additions](http://www.tug.org/mactex/morepackages.html)
5. 安装 [libsass](https://github.com/dahlia/libsass-python) `sudo pip install libsass`

## 在 Windows 安装依赖包
1. 下载并安装 [Python 2.7+](https://www.python.org/)
2. 使用python包管理工具pip获取必须的python库 ([pip](https://pip.pypa.io/en/latest/installing.html)).
  - Python 2.7.9 或更高版本 (python2版本系列), python 3.4 或者更高版本已经默认包含了pip，所以你应该已经有了pip.  它的位置在 `C:/PythonXX/Scripts`.  如果想在在终端(cmd)运行的话你需要在系统环境变量中(path)添加 `Scripts` 目录的路径。(请参考这里 [教程](http://windowsitpro.com/systems-management/how-can-i-add-new-folder-my-system-path)).
  - 下载并安装 [beauitful soup 4](http://www.crummy.com/software/BeautifulSoup/) (bs4).  在终端(cmd)运行 `pip install beautifulsoup4` 安装 BeautifulSoup.
  - 下载并安装 [libsass](https://github.com/dahlia/libsass-python). 在终端(cmd)运行 `pip install libsass` 安装 libsass
3. 下载最新版本的 pandoc 安装文件进行安装(.msi 安装文件)。下载链接：[here](https://github.com/jgm/pandoc/releases)
4. 下载最新版本的 MiKTeX 安装文件进行安装。下载连接： [here](http://miktex.org/download)
  - 安装的时候请选中 "Install Packages on the Fly."选择框。   原因是pandoc -> PDF 导出时会用到latex包，但是在基本安装 MiKTeX时不会被安装, 所以这个过程就是在第一次编译书时会将缺少的包安装好.

## Debian (Linux)
1. 安装包: ```sudo apt-get install python-pip python2.7-dev git pandoc ruby-sass texlive```
2. 安装 [beauitful soup 4](http://www.crummy.com/software/BeautifulSoup/) and [libsass](https://github.com/dahlia/libsass-python): ```pip install beauitfulsoup4 libsass```


# 贡献步骤
这个项目是用[git](http://git-scm.com/)为管理的核心, 请参考 [Git最佳实践](https://sethrobertson.github.io/GitBestPractices/). 如果你不能完全同意这个最佳实践，那么请您至少坚持早一点提交和经常提交的规范. 这样的话其他贡献者可以很方便的复查您的提交. Github对一般的问题提供了[很多的帮助](https://help.github.com/). 所以请注册账号以后, [克隆这个项目](https://help.github.com/articles/fork-a-repo/) ，然后 [发送您的 pull requests](https://help.github.com/articles/creating-a-pull-request/).


# 邮件列表

[openFrameworks Book 讨论](http://dev.openframeworks.cc/listinfo.cgi/ofbook-openframeworks.cc).

你可以在这里找到关于老版本ofBook的讨论 [ofBook Archives](http://dev.openframeworks.cc/private.cgi/ofbook-openframeworks.cc/)
