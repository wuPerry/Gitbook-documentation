# gitbook结构

##### gitbook的结构如下：

![](/assets/import2.png)

| **File** | **Description** |
| :--- | :--- |
| `book.json` | Stores[configuration](https://toolchain.gitbook.com/config.html)data \(**optional**\) |
| `README.md` | Preface / Introduction for your book \(**required**\) |
| `SUMMARY.md` | Table of Contents \(See[Pages](https://toolchain.gitbook.com/pages.html)\) \(**optional**\) |
| `GLOSSARY.md` | Lexicon / List of terms to annotate \(See[Glossary](https://toolchain.gitbook.com/lexicon.html)\) \(**optional**\) |

###### 1.summary.md

summary.md是book的目录，默认情况下，点击“+Add an article”时会自动添加。

嵌套的列表可以创建下级目录。

##### Simple example {#simple-example}

```
# Summary

* [Part I](part1/README.md)

    * [Writing is nice](part1/writing.md)
    * [GitBook is nice](part1/gitbook.md)

* [Part II](part2/README.md)

    * [We love feedback](part2/feedback_please.md)
    * [Better tools for authors](part2/better_tools.md)
```

###### Parts

添加标题或者写划线可以区分开每一章

```
# Summary

### Part I

* [Writing is nice](part1/writing.md)
* [GitBook is nice](part1/gitbook.md)

### Part II

* [We love feedback](part2/feedback_please.md)
* [Better tools for authors](part2/better_tools.md)

----
* [Last part without title](part3/title.md)
```

###### Anchors

一般目录会根据md文件来生成，但是导出pdf时会出现“下段同页”无法实现，如果要避免则需要在一个md文件编辑，且定义章节的锚点，然后手动编辑summary.md文件，使用Anchor添加到节。如在文章中编辑&lt;h2 id="writing"&gt;&lt;/h2&gt;，在summary中编辑README.md\#writing。

```
# Summary

### Part I

* [Part I](part1/README.md)
    * [Writing is nice](part1/README.md#writing)
    * [GitBook is nice](part1/README.md#gitbook)
* [Part II](part2/README.md)
    * [We love feedback](part2/README.md#feedback)
    * [Better tools for authors](part2/README.md#tools)
```

###### 2.book.json

除了修改书籍的主题外，还可以通过配置`book.json`文件来修改 gitbook 在编译书籍时的行为，例如：修改书籍的名称，显示效果等等。配置的信息请参考[https://toolchain.gitbook.com/config.html](https://toolchain.gitbook.com/config.html)







