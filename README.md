# dhbw-latex-template

Community driven DHBW LaTeX template for project thesis, seminar paper and
bachelor thesis.

## Disclaimer

This is an unofficial LaTeX template for DHBW thesises. Keep it in mind!

## Usage

To use this template clone the project folder with the following command:

```sh
git clone git@github.com:dateiexplorer/dhbw-latex-template
```

or download and extract the zip folder for a specific release package.
Keep in mind that you'll need a LaTeX installation e.g. with MiKTeX or Tex Live.
Then you can compile the file with:

```sh
pdflatex thesis
```

You need a working LaTeX installation to compile PDF files from this template.
If you get error messages, make sure you've installed all neccessary latex
packages.
If you use MiKTeX or Tex Live the packages should be downloaded automatically.
Make sure that you have a internet connection and (optionally) that you applied
your proxy settings.

To compile your acronyms and glossary entries, run:

```sh
makeglossaries thesis
```

To compile your biblography, run:

```sh
biber thesis
```

Afterwards rerun `pdflatex thesis` to get a new PDF file.

## Recommended way to create your own thesis

The documentation for this template itself is a LaTeX project which was created
with this template.
The easiest way to create your own thesis is to copy all files from the `docs/`
folder an copy it in an separate folder, e.g. `content/` or create this folder
an mimic the strukture of the `docs/` folder.

Then you can apply your specific settings in the `settings/` folder.
You should add metadata in the `settings/metadata.tex` file.
Which content is shown in the main part of the thesis is set up in the
`settings/content.tex` file. By default the documentation files are enabled.
Comment them out and add your specific files.

Third you should edid the `thesis.tex` file itself to set up the path for your
abstract, acronyms, bibliography, glossaries and appendix.
If you don't need any of these parts just comment it out.

You can change also the files in the `modules/` folder itself to apply it to
your needs. For example if you would change the sizes of the logos in the
`modules/cover.tex` file. But be careful if you change anything in this files.
Know what you do! Otherwise some features will not work correctly.

If you think you'll don't need some modules you can comment them out in the
`settings/modules.tex` file. Maybe there will be some compile errors, because
you must delete or comment out all references which requires this modules,
especially in the `thesis.tex` file. To make lifes easier you can automatically
search your the module name. All coressponding code is marked with the module
name as a comment at the end of the line. Find these lines and comment them
out. But it's recommended to enable all modules and install the missing
packages in your LaTeX distribution. 

## Features of this templates

* Small code base which provides modularity, extension and compile speed
* Correct pagination with roman paging for indices and arabic paging for
  the main content
* Simple usage of glossary and acronyms
* Biber for your bibliography
* Detailed documentation of the code base with many examples how to use
  this template for your thesis
* Many fixes for known issues to improve pdf generation