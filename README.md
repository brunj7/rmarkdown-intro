# Introduction to `rmarkdown`

This is a 1h-1h30 workshop given for UCSB [Eco-Data-Science Group](https://eco-data-science.github.io/) on 2018/10/9

There are 2 main documents:
- Presentation deck: https://github.com/brunj7/rmarkdown-intro
- R Markdown document we will be playing with: [rmarkdown-myfirst.Rmd](rmarkdown-myfirst.Rmd)


## Preparing the workshop

### Required software

We will primarily be using a web browser, `R`, `RStudio`. Please be sure these are all installed on your laptop, as follows:

- **R:** We will use R version 3.5.1, which you can download and install from [CRAN](https://cran.rstudio.com)

- **RStudio**: RStudio is an excellent front-end (IDE) for R with integrated graphics and coding tools and is recommended (read: required) for this course. It is free and available for both Windows, Mac OS X and Linux.
To download RStudio (current version is 1.1.456), visit [RStudio's download page](https://www.rstudio.com/products/rstudio/download/).
  *If you don't know how up to date your version of RStudio is, please download a recent version and install it*
    
- **R packages:** Please be sure you have installed or updated the following packages:

    - `remotes` (not needed, if you have `devtools` already installed) 
    - `knitr`
    - `rmarkdown`
    - `bookdown`
    - `DT`
    - `tidyverse`
    - `leaflet`
    - `captioner`
    
    
#### There are several ways to install a R package:

- In the R console, type: `install.packages("package-name")` Note that R is **case sensitive**, and that the **package name should be in quotes**.

- In RStudio, click on the "Packages" tab in the bottom right quadrant of the interface, click Install, type the package name and click Istall _or_ click  Tools => Install Packages, type the package name and click Install

- In R for Windows clients, go to the Packages menu => Install package(s).

- In R for MacOS X clients, go to the Package & Data menu and click on Package Installer => CRAN (binaries) => Get list. Click on the box “install dependencies” in order to automatically install other necessary libraries while installing your R libraries.

In our case, you could type at the R console:

```r
workshop_pkg <- c("remotes", "knitr", "rmarkdown", "bookdown", "DT", "tidyverse", "leaflet", "captioner")
install.packages(workshop_pkg)
```

#### PDF rendering

If you want to generate PDF output from Markdown (we will mainly focus on html files), you will need to install LaTeX. For R Markdown users who have not installed LaTeX before, we recommend to follow the recommendations of [Xie et al, 2018] and that you install `TinyTeX` (https://yihui.name/tinytex/):

```r
install.packages("tinytex")
tinytex::install_tinytex()  # install TinyTeX
```
