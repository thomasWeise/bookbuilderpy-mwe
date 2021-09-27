# 弟子章 {#sec:theChapter}

欢迎欢迎，弟子章来了。

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

\rel.code{localCode}{这是一个本地代码文件，但我们只使用第6到12行。程序代码自动简化。}{logger.py}{6-12}{}{}

\git.code{bb}{gitCode}{这是GitHub存储库中的代码文件。我们再次只使用第6到12行。程序代码不会自动简化。}{firstChapter/logger.py}{6-12}{}{doc,comments,hints}

[@lst:localCode]是一个本地代码文件。
此文件与本章的markdown文件在同一个文件夹中。
[@lst:gitCode]这是一个来自GitHub的文件。
该文件来自元数据中声明的Git存储库`bb`。

