# First Chapter {#sec:theChapter}

Welcome to the first chapter.

## First Section of First Chapter {#sec:theSection}

With `# `, you start a chapter heading, as in [@sec:theChapter].
With `## `, you start a section heading, as in [@sec:theSection].
`### ` begins a subsection, and so on.

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
Definitions can also be included and referenced.
See, for instance, \def.ref{mydef} below.

\definition{def}{mydef}{This is a definition of something.}

\rel.code{localCode}{This is a local code file but we only use lines 6 to 12 and apply automatic simplification.}{logger.py}{6-12}{}{}

\git.code{bb}{gitCode}{This is a code file from a GitHub repository. We again only use lines 6 to 12, but without simplification.}{firstChapter/logger.py}{6-12}{}{doc,comments,hints}

[@lst:localCode] is a local code file, which resides in the same folder as the markdown file of this chapter.
[@lst:gitCode] comes from GitHub, from the repository `bb` declared in the metadata.

You can access metadata via the command `meta`.
Example are:

1. Book-related metadata:
    - title: \meta{title}
    - author: \meta{author}
    - keyowords: \meta{keywords}
2. Date-related metadata:
    - time: \meta{time}
    - date: \meta{date}
    - year: \meta{year}
3. Language:
    - lang: \meta{lang}
    - locale: \meta{locale}
    - lang.name: \meta{lang.name}
4. Repository-related metadata (*only* available if the book is written as a git repository):
    - repo.name: \meta{repo.name}
    - repo.url: \meta{repo.url}
    - repo.commit: \meta{repo.commit}
    - repo.date: \meta{repo.date}
5. External Repository Information is accessible via the command `repo`, using the repository key and the repository information query:
    - repo.name for `bb`: \repo{bb}{repo.name}
    - repo.commit for `bb`: \repo{bb}{repo.commit}
    - repo.date for `bb`: \repo{bb}{repo.date}
