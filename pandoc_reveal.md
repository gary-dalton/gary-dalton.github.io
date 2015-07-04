---
title: Pandoc and Reveal
subtitle: Slideshows from Markdown
author: Gary Dalton
date: July 3, 2015
github:
    user: gary-dalton
    repo: code7
    branch: "gh-pages"
theme: sky
transition: concave

---

# Pandoc

## What is it?

- Universal document converter
- Convert markdown documents (and others) to many other formats
- [Pandoc](http://pandoc.org/)

## Installation

There is a download file just for you at:
[Pandoc Install](http://pandoc.org/installing.html)

- Windows
- OSX
- Linux
- BSD
- Source

## Output to PDF
Output to PDF requires LaTeX.

- Windows: [MiKTeX](http://miktex.org/download)
- OSX: [Basic TeX](http://www.tug.org/mactex/morepackages.html)
- Linux: [TeX Live](http://www.tug.org/texlive/)
    - `apt-get install texlive`

# Run Pandoc

`pandoc -t html5 --template=templatecdn-revealjs.html --standalone --section-divs  pandoc_reveal.md -o pandoc_reveal.html`

`pandoc -t html5 --standalone --section-divs --template=template.html --css=stylesheets/stylesheet.css   input.md -o output.html`

pandoc -t html5 --standalone --section-divs --template=template_github.html --css=stylesheets/stylesheet.css   index.md -o index.html

pandoc -t html5 --template=templatecdn-revealjs.html --standalone --section-divs --variable theme="beige" --variable transition="concave" code7_stage5.md -o code7_stage5.html

# In the evening

## Dinner

- Eat spaghetti
- Drink wine

------------------
## Me
![Gary Dalton](https://fbcdn-profile-a.akamaihd.net/hprofile-ak-xfa1/v/t1.0-1/c141.41.517.517/s160x160/405574_10200638271711285_451453026_n.jpg?oh=dffa9f39bd97ecda2fe3e72cc380e74c&oe=561D0596&__gda__=1446282714_cd33706f6c028055f2251032b4e4ba2c)

## Going to sleep

- Get in bed
- Count sheep
