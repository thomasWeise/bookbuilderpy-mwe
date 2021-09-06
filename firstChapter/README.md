# First Chapter {#sec:theChapter}

Welcome to the first chapter.

\rel.figure{myfig}{This is a figure caption.}{figure.svg}{}

Take a look at [@fig:myfig].

$$ y = 3\sin{y} +5$$ {#eq:sin}

Take a look at [@eq:sin].

|centered column|right-aligned column|left-aligned column|
|:-:|--:|:--|
|bla|r|l|
|blub blub blub|abc|123|

: This is the table caption. {#tbl:mytable}

[@tbl:mytable] is also important.

\rel.code{localCode}{This is a local code file but we only use lines 6 to 12 and apply automatic simplification.}{logger.py}{6-12}{}{}

\git.code{bb}{gitCode}{This is a code file from a GitHub repository. We again only use lines 6 to 12, but without simplification.}{bookbuilderpy/logger.py}{6-12}{}{doc,comments,hints}

[@lst:localCode] is a local code file, [@lst:gitCode] comes from GitHub.


