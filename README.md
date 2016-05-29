# Information Management Direction for MENA

## Dependencies

Install:

 * [R language](https://cran.r-project.org/bin/windows/base/) 
 * [R tools to compile the site under Windows OS](https://cran.r-project.org/bin/windows/Rtools/)
 * [R studio to write scripts](https://www.rstudio.com/products/rstudio/download/)
 * [Prince XML](http://www.princexml.com/) to generate automatically the PDF version fo the site.
 * [Github client](https://desktop.github.com/) to push edits on the repository

## Chapters

All chapters are written in **Rmarkdown** and encoded in UTF-8. 

When a new chapter is added, content table shoudl be automatically updated in `index.Rmd` and manually in the file `include\before_body.html`.

## Scripts 

 **R** script `verify_dependency_installation.R` 

 **R** script `make_pdf.R` allow to generate a PDF for the full site.

`Makefile` generate all the site from the **Rmarkdown** files and then call 

`make_pdf.R` to update the PDF of the site.

## Rebuild the site,

To execute `Makefile`, go to  **RStudio** & click on *Build All* in the  *Build* tab of the top right panel.

If on windows, make sure that you have configured both the path to Rtools & Prince in the *PATH* environment variable of your computer.