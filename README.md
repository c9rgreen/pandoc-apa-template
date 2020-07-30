# Pandoc APA Template

This is a template project for [Pandoc](https://pandoc.org) designed to help
write papers which follow the [APA style](https://apastyle.apa.org).

## Requirements

* [Docker](https://www.docker.com)
* [Make](https://www.gnu.org/software/make/)
* Fonts as needed. See more info about fonts below.

## Getting started

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
