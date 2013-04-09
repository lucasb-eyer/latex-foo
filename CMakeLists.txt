project(thesis NONE)

cmake_minimum_required(VERSION 2.4)

include(UseLATEX.cmake)

# This is the important part.
add_latex_document(main.tex DEFAULT_PDF
#                   BIBFILES references.bib
#                   IMAGE_DIRS figs
                   INPUTS title.tex
                          settings.tex
                  )

