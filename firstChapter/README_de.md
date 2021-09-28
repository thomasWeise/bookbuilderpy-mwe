# Erstes Kapitel {#sec:theChapter}

Wilkommen zum ersten Kapitel.

## Erster Abschnitt des Ersten Kapitels {#sec:theSection}

Mit `# ` fängt eine Kapitelüberschrift an, wie in [@sec:theChapter].
Mit `## ` fängt eine Abschnittsüberschrift an, wie in [@sec:theSection].
`### ` started einen Unterabschnitt und so weiter und so fort.

\rel.figure{myfig}{Dies ist eine Bildüberschrift.}{figure.svg}{}

Betrachten Sie nun [@fig:myfig].

$$\sum_{i=1}^n \frac{y^i}{n} = \sqrt{3\sin{y} +5}$$ {#eq:sin}

Schauen Sie bitte auf die Gleichung [@eq:sin].
Wir können Formeln auch direkt in den Text einbetten und z.B. $x = \log_2 5$ schreiben.

|zentrierte Spalte|rechtsbündige Spalte|linksbündige Spalte|
|:-:|--:|:--|
|bla|r|l|
|blub blub blub|abc|123|

: Das ist eine Tabellenüberschrift. {#tbl:mytable}

[@tbl:mytable] ist auch wichtig.
Definitionen können auch eingefügt und aus dem Text heraus referenziert werden.
Ein Beispiel dafür ist \def.ref{mydef} unten:

\definition{def}{mydef}{Dies ist eine Definition von irgendetwas.}

\rel.code{localCode}{Dies ist eine lokale Kode-Datei, aber wir verwenden nur Zeilen 6 bis 12 und vereinfachen diese automatisch.}{logger.py}{6-12}{}{}

\git.code{bb}{gitCode}{Dies ist eine lokale Kode-Datei von einem GitHub repository. Wir verwenden wieder nur Zeilen 6 bis 12 ohne zu vereinfachen.}{firstChapter/logger.py}{6-12}{}{doc,comments,hints}

[@lst:localCode] ist ein lokale Kode-Datei, die im selben Ordner wie die markdown-Datei dieses Kapitels liegt.
[@lst:gitCode] kommt direkt von GitHub, von dem Repository `bb`, welches wir in den Metadaten deklariert haben.

Sie können auch auf die Metadaten des Buches über das Kommando `meta` zugreifen.
Beispiele dafür sind:

1. buchbezogene Metadaten:
    - Titel (title): \meta{title}
    - Autor (author): \meta{author}
    - Stichworte (keywords): \meta{keywords}
2. datumsbezogene Metadaten:
    - Datum und Uhrzeit (time): \meta{time}
    - Datum (date): \meta{date}
    - Jahr (year): \meta{year}
3. Sprache:
    - lang: \meta{lang}
    - locale: \meta{locale}
    - lang.name: \meta{lang.name}
4. Repository-bezogene Metadaten (diese stehen *nur* zur Verfügung wenn das Buch als `git` Repository geladen wurde):
    - repo.name: \meta{repo.name}
    - repo.url: \meta{repo.url}
    - repo.commit: \meta{repo.commit}
    - repo.date: \meta{repo.date}
5. externe Repository-Information sind über das Kommando `repo` mit dem Repository-Schlüssel und der Informationsanfrage zugänglich^[Beachten Sie, dass wir hier `bb` benutzen, um das GitHub repository dieses Beispiels zu referenzieren, damit das Beispiel vollständig und eigenständig bleibt.]:
    - repo.name für `bb`: \repo{bb}{repo.name}
    - repo.commit für `bb`: \repo{bb}{repo.commit}
    - repo.date für `bb`: \repo{bb}{repo.date}
