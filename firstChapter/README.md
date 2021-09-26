# First Chapter {#sec:theChapter}

Welcome to the first chapter.

\rel.figure{myfig}{This is a figure caption.}{figure.svg}{}

Take a look at [@fig:myfig].

$$\sum_{i=1}^n \frac{y^i}{n} = \sqrt{3\sin{y} +5}$$ {#eq:sin}

Take a look at [@eq:sin].
We can also embedd formulas directly in the text and write something like $x = \log_2 5$.

|centered column|right-aligned column|left-aligned column|
|:-:|--:|:--|
|bla|r|l|
|blub blub blub|abc|123|

: This is the table caption. {#tbl:mytable}

[@tbl:mytable] is also important.

\rel.code{localCode}{This is a local code file but we only use lines 6 to 12 and apply automatic simplification.}{logger.py}{6-12}{}{}

\git.code{bb}{gitCode}{This is a code file from a GitHub repository. We again only use lines 6 to 12, but without simplification.}{firstChapter/logger.py}{6-12}{}{doc,comments,hints}

[@lst:localCode] is a local code file, which resides in the same folder as the markdown file of this chapter.
[@lst:gitCode] comes from GitHub, from the repository `bb` declared in the metadata.

