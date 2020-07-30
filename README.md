# Pandoc APA Template

This is a template project for [Pandoc](https://pandoc.org) designed to help
write papers which follow the [APA style](https://apastyle.apa.org).

## Requirements

* [Python 3.8](https://www.python.org/downloads/)
* [Docker](https://www.docker.com)
* [Make](https://www.gnu.org/software/make/)
* Fonts as needed. See more info about fonts below.

## Getting started

Use [Cookiecutter](https://cookiecutter.readthedocs.io/en/1.7.2/README.html) to
quickly scaffold a Pandoc project.

```
$ pip install --user cookiecutter

$ cookiecutter git@github.com:cg433n/pandoc-apa-template.git
```

Follow the prompts.

Pull the [Docker image](https://hub.docker.com/r/pandoc/latex).

```sh
$ make install
```

Optional: Copy the fonts which you want to use to `fonts/`.

Update `title`, `date`, and `author` in `config/metadata.yaml`.

Build the PDF.

```sh
$ make build
```

## Fonts

[Times New Roman](https://en.wikipedia.org/wiki/Times_New_Roman) is not
distributed with this repository as it is copyrighted. It is installed by
default with many operating systems.

[Times Newer Roman](https://timesnewerroman.com) is a nice alternative. APA
actually allows you to use [several
fonts](https://apastyle.apa.org/style-grammar-guidelines/paper-format/font)
including [Computer Modern](https://tug.org/FontCatalogue/computermodern/)
which is included with [LaTeX](https://www.latex-project.org)

## References

Add
[BibTeX](https://tex.stackexchange.com/questions/25701/bibtex-vs-biber-and-biblatex-vs-natbib)
style references to `references/references.bib`. [ZoteroBib](https://zbib.org)
is a nice tool for generating references which can be downloaded as `BibTeX`
files. I copy and paste the references in BibTeX files to `references.bib` and
use them in `main.md` by writing `[@reference_name, page_number]` in your
content.
