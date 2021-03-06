# 《明朝那些事儿》· 当年明月著

《明朝那些事儿》是一套在网络上连载的关于中国明朝历史小说，作者为当年明月。于2006年3月10日在天涯社区首次发表，其内容始于明太祖朱元璋的诞生，终于崇祯帝朱由检。《明朝那些事儿》在网络连载期间，每月点击率逾百万人次。截至2008年3月，当年明月发表至万历朝的国本之争，4月发表至李成梁经略辽东与努尔哈赤的崛起，7月写魏忠贤事。2008年底发表至崇祯初年，袁崇焕伏诛事。2009年1月初发表卢象昇、孙传庭等人剿寇。当年明月每天以发表文章一小篇，字数不足一千字，周末时大多休息不发表，有时会连休数天，并公布于网络上。2009年3月21日，《明朝那些事儿》连载完毕。后来，《明朝那些事儿》集结成书籍刊行，在台湾发行了繁体中文版本。之后被翻译为日文、韩文及英文等多国语言。销量超过五百万册，为中国大陆改革开放以来最畅销史学读本（也有一种说法为“1949年解放以来最畅销的通俗历史读本”），全国十大畅销书之一，2007-2008年度畅销书第一名。多次获得“新浪图书风云榜”最佳图书、当当网“终身五星级最佳图书”、“卓越亚马逊畅销书大奖”等荣誉。

+ 联想集团创始人柳传志说：“我觉得喜欢看的人都是有思想、愿意想事情的人，这是本好书，除了把史实摆出来，还要评论、挖掘，用现代的语言去说，他有他的角度。”
+ 明史专家毛佩琦说：“历史是千百万人的历史，是大家的历史。每个人都有解读历史的权利。《明朝那些事儿》的确是别开生面的，是一种创造。我热情地支持这种探索和创造！”。
+ 中国青年学者欧发伟认为，当年明月用自己的灵魂还原了历史，而人类在他的历史里还原了灵魂。


![明朝那些事儿 · 当年明月](./Images/Frontmatter.jpg)

---
编译环境：

+ **TeX Distribution**
    + [MacTeX 2020](https://www.tug.org/mactex/) (for Apple macOS)

    + [TeX Live 2020](https://www.tug.org/texlive/) (for GNU/Linux & Microsoft Windows)

+ **Fonts**
    + [Adobe Source Han Sans 2.001](https://github.com/adobe-fonts/source-han-sans)
    + [Adobe Source Han Serif 1.001](https://github.com/adobe-fonts/source-han-serif)
    + [Font Awesome Free 5.13.0](https://github.com/FortAwesome/Font-Awesome)

+ **Editor**
    + [Visual Studio Code 1.44.0](https://code.visualstudio.com/) with extension [LaTeX Workshop 8.8.0](https://github.com/James-Yu/LaTeX-Workshop)
        + Configuration for LaTeX Workshop extension to complie XeTeX source code into PDF Version 1.7 (Acrobat 8.x)
        + ```Visual Studio Code``` ⇢ ```File``` ⇢ ```Preferences``` ⇢ ```Settings``` ⇢ ```Extensions``` ⇢ ```LaTeX``` ⇢ ```Recipes```

        ```JSON
        {
                "latex-workshop.view.pdf.viewer": "tab",
                "latex-workshop.latex.tools": [
                        {
                                "name": "latexmk",
                                "command": "latexmk",
                                "args": [
                                        "-synctex=1",
                                        "-interaction=nonstopmode",
                                        "-file-line-error",
                                        "-pdf",
                                        "%DOC%"
                                ]
                        },
                        {
                                "name": "xelatex",
                                "command": "xelatex",
                                "args": [
                                        "-synctex=1",
                                "-interaction=nonstopmode",
                                "-file-line-error",
                                "--output-driver=xdvipdfmx -q -E -V 7",
                                "%DOC%"
                                ]
                        }
                ],
                "latex-workshop.latex.recipes": [
                        {
                                "name": "XeLaTeX / XeTeX",
                                "tools": [
                                        "xelatex"
                                ]
                        },
                        {
                                "name": "latexmk",
                                "tools": [
                                        "latexmk"
                                ]
                        }
                ],
                "workbench.startupEditor": "newUntitledFile",
                "window.zoomLevel": 0,
                "editor.minimap.enabled": false
        }
        ```
