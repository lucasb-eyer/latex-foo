project(thesis NONE)

cmake_minimum_required(VERSION 2.4)

include(UseLATEX.cmake)

# This is the important part.
add_latex_document(thesis.tex DEFAULT_PDF
                   BIBFILES references.bib
                   IMAGE_DIRS figs
                   INPUTS acknowledgements.tex
                          conclusions.tex
                          introduction.tex
                          thesis.tex
                          adding_gpus.tex
                          cpu_implementation.tex
                          gpus.tex
                          settings.tex
                          title.tex
                          visualization.tex
                  )

