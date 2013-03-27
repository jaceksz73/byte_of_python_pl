# A Byte of Python

Convert to pdf example:
windows key + R 
cmd
cd d:\zbiory\wiedza\python\byte_of_python_pl
pandoc 02-preface.pd -o 02-preface.pdf
copy/paste - right click in cmd

## Installation

Ensure Python (&gt;= 2.7) is installed.

Install Pandoc from <http://johnmacfarlane.net/pandoc/installing.html>

Install `pdflatex` from <http://www.tug.org/texlive/>.
Note that Mac users can install `MacTex.pkg` from <http://www.tug.org/mactex/2012/>.

Install `pip` if not present already:

    sudo sh -c "curl -k -O https://raw.github.com/pypa/pip/master/contrib/get-pip.py && python get-pip.py && rm get-pip.py"


Install Python libraries needed:

    sudo pip install -r requirements.txt


Convert the source files into HTML files:

    fab html

Convert the source files into PDF:

    fab pdf

Convert the source files into EPUB (ebook):

    fab epub

## Editing

If you're using Vim editor, then you may like the [vim-pandoc](https://github.com/vim-pandoc/vim-pandoc) plugin. There is one downside though - for long chapters, it becomes really slow, so I edit only in plain text mode (`:set ft=`), but when reviewing, I use the `pandoc` (`:set ft=pandoc`) mode.
