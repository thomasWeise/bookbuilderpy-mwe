# 弟子章 {#sec:theChapter}

欢迎欢迎，弟子章来了。

## 这是第一章的第一节 {#sec:theSection}

使用`# `，你可以开始一个章节的标题，例如在[@sec:theChapter]。
使用`## `，你可以开始一个节的标题，例如在[@sec:theSection]。
`### `开始一个分段，依此类推。

\rel.figure{myfig}{这是一个数字标题。}{figure.svg}{}

先看[@fig:myfig]把。

$$\sum_{i=1}^n \frac{y^i}{n} = \sqrt{3\sin{y} +5}$$ {#eq:sin}

现在看[@eq:sin]把。
我们也可以直接在文本中包含数学公式。
我们也可写$x = \log_2 5$。

|文本居中的表格列|文本右对齐的表格列|文本左对齐的表格列|
|:-:|--:|:--|
|bla|r|l|
|blub blub blub|abc|123|

: 这是表格标题。 {#tbl:mytable}

[@tbl:mytable]有好多的意思。
定义也可以包含在文本中并从文本中引用。
例如，请看下面的\def.ref{mydef}。

\definition{def}{mydef}{这是一个定义。}

\rel.code{localCode}{这是一个本地代码文件，但我们只使用第6到12行。程序代码自动简化。}{logger.py}{6-12}{}{}

\git.code{bb}{gitCode}{这是GitHub存储库中的代码文件。我们再次只使用第6到12行。程序代码不会自动简化。}{firstChapter/logger.py}{6-12}{}{doc,comments,hints}

[@lst:localCode]是一个本地代码文件。
此文件与本章的markdown文件在同一个文件夹中。
[@lst:gitCode]这是一个来自GitHub的文件。
该文件来自元数据中声明的Git存储库`bb`。

你可以通过命令`meta`访问元数据。
下面我们来举几个例子：

1. 关于书本身的元数据：
    - 这本书的标题（title）：\meta{title}
    - 这本书的作者（author）：\meta{author}
    - 书的关键词（keywords）：\meta{keywords}
2. 关于当前日期和时间的元数据：
    - 时间（time）：\meta{time}
    - 日期（date）：\meta{date}
    - 年（year）：\meta{year}
3. 语言：
    - lang：\meta{lang}
    - locale：\meta{locale}
    - lang.name：\meta{lang.name}
4. 只有当本书被写成`git`仓库时，与仓库相关的元数据才可用:
    - repo.name：\meta{repo.name}
    - repo.url：\meta{repo.url}
    - repo.commit：\meta{repo.commit}
    - repo.date：\meta{repo.date}
5. 使用存储库键和存储库信息查询，可以通过命令`repo`访问外部存储库信息^[注意，我们使用`bb`来标识这个示例的GitHub存储库，以使示例自包含。]：
    - 密钥`bb`的repo.name：\repo{bb}{repo.name}
    - 密钥`bb`的repo.commit：\repo{bb}{repo.commit}
    - 密钥`bb`的repo.date：\repo{bb}{repo.date}
