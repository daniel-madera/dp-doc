## dp-doc

Documentation to master thesis.

## Instalation

sudo apt-get install texlive-full xzdec

tlmgr init-usertree
tlmgr update --self --all --reinstall-forcibly-removed
sudo tlmgr install titlesec
tlmgr install parskip

Tex compilation requires TUL package available from [NTI TUL site](http://www.nti.tul.cz/~satrapa/vyuka/latex-tul/). Unzip and save to your tex packages location. (Default texlive location ~/texmf/tex/latex/)

## Run

cd output/
pdflatex ../dp-titlepage.tex
pdflatex ../dp-madera.tex


## Custom

### Vlna

Add fixed spaces to tex document - available from [petr.olsak.net](http://petr.olsak.net/ftp/olsak/vlna/).

#### Instalation

tar zxfv vlna.tar.gz
cd vlna/
./configure
make
sudo make install

#### Usage

vlna -l -m -n dp-madera.tex 