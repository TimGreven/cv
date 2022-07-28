
![LaTeX build](../../workflows/LaTeX%20build/badge.svg)
[![Latest build of TimWassink.pdf](https://img.shields.io/badge/TimWassink.pdf-latest-orange.svg?style=flat)](../gh-action-result/pdflatex/TimWassink.pdf)
[![Latest build of TimWassink-NoPubs.pdf](https://img.shields.io/badge/TimWassink--NoPubs.pdf-latest-orange.svg?style=flat)](../gh-action-result/pdflatex/TimWassink-NoPubs.pdf)
[![Latest build of TimWassink-PubsOnly.pdf](https://img.shields.io/badge/TimWassink--PubsOnly.pdf-latest-orange.svg?style=flat)](../gh-action-result/pdflatex/TimWassink-PubsOnly.pdf)

# Tim's curriculum vitae (forked from Leo)

Please feel free to clone this repo if you like the style and want to use it for your CV.  If you're going to customize it, you need to know the layout of the contents:
- [TimWassink.tex](TimWassink.tex): The top-level file. Includes all content *except* for list of publications, list of talks, and contact info.
- [TimWassink-NoPubs.tex](TimWassink-NoPubs.tex): Another top-level file, which just sets a flag and includes the above. Generates a CV without pub list.
- [TimWassink-PubsOnly.tex](TimWassink-PubsOnly.tex): Another top-level file. Generates just a publication list (with contact info header).

The following files are included by the above (they can not be compiled by themselves):
- [ContactContent.tex](ContactContent.tex): Contains the contact info header with physical address, email address, web site, office phone
- [PubsContent.tex](PubsContent.tex): Contains list of publications, 
- [TalksContent.tex](TalksContent.tex): Contains list of talks.

If you're going to use this repo as a starting point for your own CV, you'll probably have to change a bunch of filenames.
If you're going to keep it on github and want the github action that builds the PDFs (badge links above) to work, then you'll want to change the corresponding file names in the [.github/workflows/pdflatex.yml](.github/workflows/pdflatex.yml) workflow file.
