# Minimum Working Example for [bookbuilderpy](https://github.com/thomasWeise/bookbuilderpy) Tool Suite

This is a Minimum Working Example for [`bookbuilderpy` Tool Suite](https://github.com/thomasWeise/bookbuilderpy).
You can use this as a blueprint for making your own books.

## 1. Introduction

The [`bookbuilderpy` Tool Suite](https://github.com/thomasWeise/bookbuilderpy) generates electronic books from [pandoc flavored markdown](http://pandoc.org/MANUAL.html#pandocs-markdown).
It can handle multiple languages of the book at once and also generates a website.
Below, you can see the output generated from this example:

<div id="files">

- English
  + [book_en.pdf](https://thomasweise.github.io/bookbuilderpy-mwe/en/book_en.pdf) for reading on PC,
  + [book_en.html](https://thomasweise.github.io/bookbuilderpy-mwe/en/book_en.html) for viewing in the browser,
  + [book_en.epub](https://thomasweise.github.io/bookbuilderpy-mwe/en/book_en.epub) for reading on a tablet or phone,
  + [book_en.azw3](https://thomasweise.github.io/bookbuilderpy-mwe/en/book_en.azw3) for reading on a Kindle device,
  + all of the above as [tar.xz archive](https://thomasweise.github.io/bookbuilderpy-mwe/en/book_en.tar.xz),
  + all of the above as [zip archive](https://thomasweise.github.io/bookbuilderpy-mwe/en/book_en.zip).
- Deutsch
  + [book_de.pdf](https://thomasweise.github.io/bookbuilderpy-mwe/de/book_de.pdf) zum Lesen am PC,
  + [book_de.html](https://thomasweise.github.io/bookbuilderpy-mwe/de/book_de.html) zum Lesen im Webbrowser,
  + [book_de.epub](https://thomasweise.github.io/bookbuilderpy-mwe/de/book_de.epub) zum Lesen auf dem Tablet oder Mobiltelefon,
  + [book_de.azw3](https://thomasweise.github.io/bookbuilderpy-mwe/de/book_de.azw3) zum Lesen auf dem Kindle,
  + alles oben als [tar.xz Archiv](https://thomasweise.github.io/bookbuilderpy-mwe/de/book_de.tar.xz),
  + alles oben als [zip Archiv](https://thomasweise.github.io/bookbuilderpy-mwe/de/book_de.zip).
- 中文
  + [book_zh.pdf](https://thomasweise.github.io/bookbuilderpy-mwe/zh/book_zh.pdf)在电脑上阅读,
  + [book_zh.html](https://thomasweise.github.io/bookbuilderpy-mwe/zh/book_zh.html)在浏览器中阅读它,
  + [book_zh.epub](https://thomasweise.github.io/bookbuilderpy-mwe/zh/book_zh.epub)在平板电脑或手机上阅读,
  + [book_zh.azw3](https://thomasweise.github.io/bookbuilderpy-mwe/zh/book_zh.azw3)在kindle阅读器上阅读,
  + 所有东西一起作为[tar.xz归档](https://thomasweise.github.io/bookbuilderpy-mwe/zh/book_zh.tar.xz),
  + 所有东西一起作为[zip归档](https://thomasweise.github.io/bookbuilderpy-mwe/zh/book_zh.zip).  

</div>

Notice: This `README.md` file is also used as contents of the [automatically generated website](https://thomasweise.github.io/bookbuilderpy-mwe/).

## 2. How To Use

If you want to learn more about using the tool suite, you can read the documentation provided in the [`README.md`](https://github.com/thomasWeise/bookbuilderpy/blob/main/README.md) of [its repository](https://github.com/thomasWeise/bookbuilderpy).

If you use [Ubuntu](https://ubuntu.com) [Linux](https://www.linux.org) and have [docker installed](https://docs.docker.com/engine/install/ubuntu/), then you can run this example on your PC using the [docker image](http://hub.docker.com/r/thomasweise/docker-bookbuilderpy/) holding a complete installation of the tool suite.


```shell
mkdir example
cd example
git clone https://github.com/thomasWeise/bookbuilderpy-mwe.git
mkdir result
sudo docker run -v "$(pwd)/bookbuilderpy-mwe":/input/:ro -v "$(pwd)/result":/output/ thomasweise/docker-bookbuilderpy book.md
sudo chown $USER -R result
```

If you want to create an own book on GitHub and have it automatically compiled and published after each commit, you can use a [GitHub Actions](https://github.com/features/actions) for this purpose.
This, again, is described in detail in the [documentation](https://github.com/thomasWeise/bookbuilderpy/blob/main/README.md).

## 3. License

This example is released under the Attribution-NonCommercial-ShareAlike 4.0 International license (CC&nbsp;BY&#8209;NC&#8209;SA&nbsp;4.0), see [http://creativecommons.org/licenses/by-nc-sa/4.0/](http://creativecommons.org/licenses/by-nc-sa/4.0/) for a summary.

## 4. Contact

If you have any questions or suggestions, please contact
Prof. Dr. [Thomas Weise](http://iao.hfuu.edu.cn/5) (汤卫思教授)
at the Institute of Applied Optimization (应用优化研究所, [IAO](http://iao.hfuu.edu.cn))
of the School of Artificial Intelligence and Big Data ([人工智能与大数据学院](http://www.hfuu.edu.cn/jsjx/))
of [Hefei University](http://www.hfuu.edu.cn/english/) ([合肥学院](http://www.hfuu.edu.cn/)),
in Hefei, Anhui, China (中国安徽省合肥市)
via email to [tweise@hfuu.edu.cn](mailto:tweise@hfuu.edu.cn) with CC to [tweise@ustc.edu.cn](mailto:tweise@ustc.edu.cn).

