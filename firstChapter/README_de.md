# Erstes Kapitel {#sec:theChapter}

Wilkommen zum ersten Kapitel.

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

\rel.code{localCode}{Dies ist eine lokale Kode-Datei, aber wir verwenden nur Zeilen 6 bis 12 und vereinfachen diese automatisch.}{logger.py}{6-12}{}{}

\git.code{bb}{gitCode}{Dies ist eine lokale Kode-Datei von einem GitHub repository. Wir verwenden wieder nur Zeilen 6 bis 12 ohne zu vereinfachen.}{firstChapter/logger.py}{6-12}{}{doc,comments,hints}

[@lst:localCode] ist ein lokale Kode-Datei, die im selben Ordner wie die markdown-Datei dieses Kapitels liegt.
[@lst:gitCode] kommt direkt von GitHub, von dem Repository `bb`, welches wir in den Metadaten deklariert haben.



