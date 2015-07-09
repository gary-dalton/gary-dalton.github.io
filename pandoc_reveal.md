---
title: Pandoc and Reveal
subtitle: Slideshows from Markdown
author: Gary Dalton
date: 8 July 2015
github:
  user: gary-dalton
  repo: gary-dalton.github.io
  branch: "master"
css: stylesheets/stylesheet.css
pandoc: pandoc -t html5 --standalone --section-divs --template=templatecdn_revealjs.html pandoc_reveal.md -o pandoc_reveal.html
theme: night
transition: concave
tags: pandoc, revealjs, markdown, howto

---
#

1. This slideshow is written in Markdown, a plain text format.
    - [view the slideshow in markdown](https://raw.githubusercontent.com/gary-dalton/gary-dalton.github.io/master/pandoc_reveal.md)
2. Converted into an HTML5 document using Pandoc.
3. Pandoc uses a template to convert the Markdown to HTML5.
4. The HTML5 document is automatically formatted for use with and linked to reveal.js by the template.
5. Reveal is a feature-rich javascript library that displays the slideshow.

Yes, it really is that easy.

# Markdown

## Plain text, formatted

Markdown is plain text with formatting syntax designed so that it can be converted to HTML and many other formats. Markdown is often used to format readme files, for writing messages in online discussion forums, and to create rich text using a plain text editor.

## Learn more

- [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
- [Markdown Basics](https://help.github.com/articles/markdown-basics/)
- [Markdown Tutorial](http://markdowntutorial.com/)

## What software is needed?

- Markdown may be created using any plain text editor. If you are doing a lot a plain text work, a good text editor is a must.
- My favorite is the free and open source [Atom](https://atom.io/).

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

## Command line

Pandoc is run from the command line. This is not a tutorial on how to use the command line. If you are unsure of your command line skills, try one of the many excellent tutorials available though a [Google search](https://www.google.com/search?q=comand%20line%20tutorial).

I happen to be running this via Windows PowerShell but the commands are identical to a Linux BASH.

## Commands to create this slideshow are:

    cd my_working_directory
    pandoc -t html5 --template=templatecdn_revealjs.html --standalone --section-divs  pandoc_reveal.md -o pandoc_reveal.html

Pandoc has many options, see `pandoc --help`.

## Let's break it down

- **cd my_working_directory**: Change directory to my_working_directory. my_working_directory is where my files and templates are stored.

- **pandoc arguments**: Calls Pandoc with the specified arguments

## Arguments

- **-t FORMAT**: Specify the output FORMAT as HTML5
- **--template=FILE**: Selects the conversion template as templatecdn_revealjs.html. (More on this later)
- **--standalone**: Produce output with an appropriate header and footer and not just a snippet

## More arguments

- **--section-divs**: For HTML5 it wraps sections in `<section>` tags
- **pandoc_reveal.md**: This is the input file. Its format is automatically determined from the file extension
- **-o FILE**: Write output to the FILE pandoc_reveal.html

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
