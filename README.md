# dhbw-latex-template

Community driven DHBW LaTeX template for project thesis, seminar paper and
bachelor thesis.

## Disclaimer

This is an unofficial LaTeX template. Keep it in mind!

## Usage

To use this template clone the project folder with the following command:

```sh
git clone https://github.com/dateiexplorer/dhbw-latex-template
```

Then you can compile the file with:

```sh
pdflatex thesis
```

You need a working LaTeX installation to compile PDF files from this template.
If you get error messages, make sure you've installed all neccessary latex
packages.
If you use MikTex the packages should be downloaded automatically. Make sure
that you have a internet connection and (optionally) that you applied your
proxy settings.

To compile your akronyms and glossary entries, run:

```sh
makeglossaries thesis
```

To compile your biblography, run:

```sh
biber thesis
```

Afterwards run ```pdflatex thesis``` to get a new PDF file.

## Features of this templates

* Small code base which provides modularity, extension and compile speed
* Correct pagination with roman paging for indices and arabic paging for
  the main content
* Simple usage of a glossary and acronyms
* Biber for your bibliography
* Detailed documentation of the code base with many examples how to use
  this template for your thesis
* Many fixes for known issues to improve pdf generation