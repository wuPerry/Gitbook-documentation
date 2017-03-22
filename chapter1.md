# Gitbook的使用

##### 一. 注册好或者使用GitHub登录你的GitBook账号之后,点击新建一本书.如图所示,点击那个蓝色的按钮"+ New Book"

![](/assets/import.png)

##### 二 .gitbook的结构如下：

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

###### 2. Parts

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

###### 3. Anchors

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



