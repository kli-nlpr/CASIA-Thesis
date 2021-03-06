# 中国科学院自动化研究所学位论文模板（ LaTeX & Word ）

## 模板下载

请在页面右边点击：

```
Clone or download -> Download Zip
```

## 鸣谢
本模版LaTeX部分基于[UCASThesis](https://github.com/mohuangrui/ucasthesis)制作，特别感谢原作者吴凌云和莫晃锐二位的辛勤劳动。

2018.3 更新：黄国平，施祺。

## 模板简介

* 本模板用于撰写中国科学院大学学位论文，面向对象为自动化研究所学生（硕、博）

* 考虑到大多数用户并无 LaTeX 使用经验，本模板将 LaTeX 的复杂性尽可能地进行了封装，开放出简单的接口，以便于使用者可以轻易地使用。同时，对使用 LaTeX 撰写论文所遇到的一些主要难题，如插入图片、文献索引等，进行了详细的说明，并提供了相应的代码样本，理解了上述问题后，对于初学者而言，使用此模板撰写其学文论文将不存在实质性的困难。所以，如果您是初学者，请不要直接放弃，因为同样作为初学者的我，十分明白让 LaTeX 变得简单易用的重要性，而这正是本模板所体现的。

* LaTeX模板基于中科院数学与系统科学研究院吴凌云研究员的 CASthesis 模板发展而来。当前模板满足最新的中国科学院大学学位论文撰写要求和封面设定。模板兼顾不同操作系统 (Windows，Linux，MacOS) 和 LaTeX 编译引擎（pdflatex，xelatex，lualatex），支持中文书签、中文渲染、中文粗体显示、拷贝 PDF 中的文本到其他文本编辑器等特性，此外，对模板的文档结构进行了精心设计，撰写了编译脚本提高模板的易用性和使用效率。

* 宏包的目的是简化学位论文的撰写，模板文档的默认设定是十分规范的，从而论文作者可以将精力集中到论文的内容上，而不需要在版面设置上花费精力。 同时，在编写模板的 LaTeX 文档代码过程中，作者对各结构和命令进行了十分详细的注解，并提供了整洁一致的代码结构，对文档的仔细阅读可以为初学的您提供一个学习 LaTeX 的窗口。除此之外，整个模板的架构十分注重通用性，事实上，本模板不仅是中国科学院大学学文论文模板，同时，也是使用 LaTeX 撰写中英文 Article 或 Book 的通用模板，并为使用者的个性化设定提供了接口和相应的代码。

* 建议使用TexLive。如果使用MikTex，本模板所展示文章，其引用的个别包需要单独编译和安装，需要安装的包和安装方法见/Path/To/Repo/Latex/Packages


## 用户指南

模板每次发布前，都已在 Windows，Linux，MacOS 系统上测试通过。下载模板后，若编译出现错误，则请遵从如下的用户指南:

    * 请仔细阅读并理解 `模板使用说明.pdf` 文档，根据说明文档的引导对模板进行测试。
    * 按照 `模板使用说明.pdf` 的 `先试试效果` 一节提供的方法编译模板，若出现错误，则原因可能为：
        1. 路径中存在特殊字符：请确保软件的安装路径以及模板路径中不存在奇怪的字符，
           尽量避免在路径中使用中文字符和空格。
        2. LaTeX 编译系统安装失败：请暂时抛开 ucasthesis，而是测试一个基本的中文
           LaTeX 文档，若编译无法通过，则请卸载并重新安装编译软件的最新版本。
           （MikTeX 用户：安装完后须在 CMD 内运行 `initexmf --mkmaps` 才能正常使用 pdflatex。
           并进入软件的 Package Manager (Admin) 确认启用 Repository--Synchronize 状态。
           刚安装完后的初始几次编译常会出现出错提示，需要多尝试几次才会变得流畅。）
        3. LaTeX 编译系统缺乏必要的宏包或字体：编译生成的 `.log` 文件会给出
           缺乏的宏包或字体的名称和错误提示。并且编译过程中一般会提示是否自动下载，
           请选择自动下载，即可解决大部分宏包缺乏的问题。若没能自动下载，可考虑手动安装。
        4. LaTeX 宏包过时：若编译生成的 `.log` 文件给出 `undefined` 类的错误，
           则是你的编译系统版本过旧或是其宏包库太久没有更新，
           请或是更新宏包库或是卸载安装最新版本。
    * 使用脚本编译无错，但使用 LaTeX 文本编辑器时编译出现异常：
        1. 请确保你选择了正确的文本编译器：xelatex（推荐）或 pdflatex 或 lualatex（推荐）
        2. 请确保你选择了正确的文献编译器：bibtex
    * 若按照上述步骤仍无法解决问题，请将你编译生成的完整的 `.log` 文件反馈。
