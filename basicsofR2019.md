Syllabus
========

-   Introduction
    -   **Installing R and RStudio**: R Versions, Download and install
        R, Installing Packages, Loading Packages, Updating R and its
        Packages.
    -   **User Interface, Packages and Help**: The R Console, RStudio,
        Getting Help.
    -   **R Packages**: Listing Packages in Local Libraries, Loading
        Packages, Package Repositories, Finding and Installing Packages
        Inside R and other Repositories,
-   The R Language
    -   **Overview**: Expressions, Objects, Symbols, Functions, Special
        Values.
    -   **R Objects**: Vectors, Integers, Character, Logicals, Complex
        and Raw, Attributes of Objects, Matrices, Arrays, Class, Dates
        and Time, Factors, Coercion, Lists, Data Frames, Changing
        values, Logical Subsetting, Boolean Operators, Missing
        Information and removing NAs.
    -   **R Environment**: Symbols, Working with Environments, The
        Global Environment.
-   Working with Data in R
    -   **Loading and Saving data in R**: Entering Data within R, Data
        Editor (RStudio), Datasets in R, Working Directory, The read
        Family, HTML data links, R Files, Saving R Files, Excel
        Spreadsheets and R, Loading files from other programs.
    -   **Preparing Data**: Combining, Transforming, Binning,
        Subsetting, Cleaning, Sorting and Summarizing Data.
-   Graphics
    -   **Base Graphics**: Scatter Plots, Time Series Plots, Bar Plots,
        Histogram, Box-Plots, Customizing Charts.

What is R?
==========

-   R is an open-source software environment for statistical computing
    and graphics.
-   R compiles and runs on Windows, Mac OS X, and numerous UNIX
    platforms (such as Linux).
-   R is open source software. Other software like STATA may cost on an
    average of $1000 annual license fee.

The R Environment
=================

-   Features of R
    -   An effective data handling and storage facility.
    -   A suite of operators for calculations on arrays, in particular
        matrices.
    -   A collection of tools for data analysis.
    -   Graphical facilities for data analysis.
    -   A well developed, simple, and effective programing language.
-   The R system is a software environment for statistical computing and
    graphics.
-   The term “environment” is intended to characterize R as a fully
    planned and coherent system, rather than an incremental accretion of
    very specific and inflexible tools, as is frequently the case with
    other data analysis software.
-   R is an implementation of S language.
-   S is a language that was developed by John Chambers and others at
    Bell Labs.
-   S was initiated in 1976 as a statistical analysis environment.
-   R was created in New Zealand in the year 1991 by Ross Ihaka and
    Robert Gentleman.
-   The first version R 1.0.0 was released in the year 2000 after Ross
    and Robert agreed to make it a free software under GNU General
    Public License in 1995.
-   The name “GNU” is a recursive acronym for “GNU’s Not Unix.” See
    <a href="https://gnu.org" class="uri">https://gnu.org</a>  
-   Usually, there is an official release of R twice a year.
-   In S, statistical analysis is usually done as a series of steps with
    intermediate results being stored in objects, Thus whereas SPSS and
    SAS will give copious output from a regression analysis, R will give
    minimal output and store the results in a fit object for subsequent
    interrogation by further R functions.

Design of the R system
======================

-   R system is divided into 2 conceptual parts –
    -   The “base” R system that you download from CRAN
        <a href="https://cran.r-project.org/" class="uri">https://cran.r-project.org/</a>
    -   Everything else.
-   The “base” package contains the most fundamental functions used to
    run R.
-   The other packages can be downloaded and installed as per user
    requirements; for eg.`AER` package is required for econometrics.

The R console
=============

<img src="C:/Users/pravesh/Google Drive/Copy/R/Lecture Basics of R/Basics of R 2019 pics/RConsole.png" alt="Fig 1:The R Console" width="90%" />
<p class="caption">
Fig 1:The R Console
</p>

The R console is a tool that allows you to type commands into R and see
how the R system responds. The commands that you type into the console
are called expressions. By default, R will display a greater-than sign
(“\>”) in the console (at the beginning of a line, when nothing else is
shown) when R is waiting for you to enter a command into the console. R
is prompting you to type something, so this is called a prompt. For
example, suppose that you typed 17 + 3 on the console, you would see
something similar to this:

<img src="C:/Users/pravesh/Google Drive/Copy/R/Lecture Basics of R/Basics of R 2019 pics/RConsoleExample.PNG" alt="Fig 2:Simple operations in R Console" width="90%" />
<p class="caption">
Fig 2:Simple operations in R Console
</p>

R Studio
========

-   R Studio Integrated Development Environment (IDE) is a powerful and
    productive user interface for R.
-   Like R, it is free and multi-platform. It can be downloaded from
    <a href="https://www.rstudio.com/" class="uri">https://www.rstudio.com/</a>
-   RStudio is a separate open-source project that brings many powerful
    coding tools together into an intuitive, easy-to-learn interface.
-   The RStudio program can be run on the desktop or through a web
    browser.
-   The desktop version is available for Windows, Mac OS X, and Linux
    platforms

<img src="C:/Users/pravesh/Google Drive/Copy/R/Lecture Basics of R/Basics of R 2019 pics/RStudioLogo.png" width="30%" />

<img src="C:/Users/pravesh/Google Drive/Copy/R/Lecture Basics of R/Basics of R 2019 pics/RStudio.png" alt="Fig 3:RStudio" width="90%" />
<p class="caption">
Fig 3:RStudio
</p>

Lets begin!
===========

You can now unistall the R and RStudio already installed in your
computers so that you can actually have a fresh start.
<img src="C:/Users/pravesh/Google Drive/Copy/R/Lecture Basics of R/Basics of R 2019 pics/uninstall.png" width="90%" />

Downloading and installing R and RStudio
========================================

<img src="C:/Users/pravesh/Google Drive/Copy/R/Lecture Basics of R/Basics of R 2019 pics/downloadR1.png" width="90%" /><img src="C:/Users/pravesh/Google Drive/Copy/R/Lecture Basics of R/Basics of R 2019 pics/downloadR2.png" width="90%" /><img src="C:/Users/pravesh/Google Drive/Copy/R/Lecture Basics of R/Basics of R 2019 pics/downloadR3.png" width="90%" /><img src="C:/Users/pravesh/Google Drive/Copy/R/Lecture Basics of R/Basics of R 2019 pics/downloadRStudio1.png" width="90%" /><img src="C:/Users/pravesh/Google Drive/Copy/R/Lecture Basics of R/Basics of R 2019 pics/downloadRStudio2.png" width="90%" /><img src="C:/Users/pravesh/Google Drive/Copy/R/Lecture Basics of R/Basics of R 2019 pics/downloadRStudio3.png" width="90%" />

Getting help
============

To get a help on a specific function say “solve”, the command is

``` r
help(mean)
# or
?mean()
# or
??mean
```

For a feature specified by special characters, the argument must be
enclosed in double or single quotes making it a character string. This
is also necessary for a few words with syntatic meaning including `if`,
`for` and `function`.

``` r
help("[["); help("if")
?"[["
```

Packages in R
=============

A package is a related set of functions, help files, and data files that
have been bundled together. For example, the `stats` package contains
functions for doing statistical analysis. Some packages are included in
R, other packages are available from public package repositories. You
can also make your own packages!

Inorder to get the list of packages loaded by default use the command;

``` r
getOption("defaultPackages")
```

    ## [1] "datasets"  "utils"     "grDevices" "graphics" 
    ## [5] "stats"     "methods"

``` r
# if you wish to see the list of currently loaded packages
## (.packages())

# to see all the packages available
(.packages(all.available = TRUE))
```

    ##   [1] "abind"             "AER"              
    ##   [3] "anytime"           "askpass"          
    ##   [5] "assertthat"        "backports"        
    ##   [7] "base64enc"         "bdsmatrix"        
    ##   [9] "betareg"           "BH"               
    ##  [11] "bibtex"            "bookdown"         
    ##  [13] "brew"              "broom"            
    ##  [15] "callr"             "car"              
    ##  [17] "carData"           "cellranger"       
    ##  [19] "censReg"           "checkmate"        
    ##  [21] "classInt"          "cli"              
    ##  [23] "clipr"             "clisymbols"       
    ##  [25] "colorspace"        "commonmark"       
    ##  [27] "countrycode"       "covr"             
    ##  [29] "crayon"            "crosstalk"        
    ##  [31] "crul"              "curl"             
    ##  [33] "data.table"        "DBI"              
    ##  [35] "dbplyr"            "desc"             
    ##  [37] "devtools"          "dichromat"        
    ##  [39] "digest"            "dplyr"            
    ##  [41] "DT"                "e1071"            
    ##  [43] "EDA"               "ellipsis"         
    ##  [45] "evaluate"          "fansi"            
    ##  [47] "farver"            "fastmap"          
    ##  [49] "flexmix"           "forcats"          
    ##  [51] "Formula"           "fs"               
    ##  [53] "gbRd"              "generics"         
    ##  [55] "geojson"           "geojsonio"        
    ##  [57] "geojsonlint"       "gghighlight"      
    ##  [59] "ggplot2"           "ggrepel"          
    ##  [61] "gh"                "git2r"            
    ##  [63] "glmmML"            "glue"             
    ##  [65] "gridExtra"         "gtable"           
    ##  [67] "gtrendsR"          "haven"            
    ##  [69] "hexbin"            "highr"            
    ##  [71] "hms"               "htmltools"        
    ##  [73] "htmlwidgets"       "httpcode"         
    ##  [75] "httpuv"            "httr"             
    ##  [77] "ini"               "isoband"          
    ##  [79] "jqr"               "jsonlite"         
    ##  [81] "jsonvalidate"      "kableExtra"       
    ##  [83] "knitr"             "labeling"         
    ##  [85] "later"             "lazyeval"         
    ##  [87] "leaflet"           "leaflet.providers"
    ##  [89] "leafsync"          "lifecycle"        
    ##  [91] "lme4"              "lmtest"           
    ##  [93] "lubridate"         "lwgeom"           
    ##  [95] "magick"            "magrittr"         
    ##  [97] "maptools"          "margins"          
    ##  [99] "markdown"          "MatrixModels"     
    ## [101] "matrixStats"       "maxLik"           
    ## [103] "memoise"           "mfx"              
    ## [105] "mgsub"             "mime"             
    ## [107] "minqa"             "miscTools"        
    ## [109] "modelr"            "modeltools"       
    ## [111] "munsell"           "nloptr"           
    ## [113] "openssl"           "openxlsx"         
    ## [115] "pander"            "pbkrtest"         
    ## [117] "pdftools"          "pillar"           
    ## [119] "pkgbuild"          "pkgconfig"        
    ## [121] "pkgload"           "plm"              
    ## [123] "plogr"             "plotly"           
    ## [125] "plyr"              "png"              
    ## [127] "praise"            "prediction"       
    ## [129] "prettyunits"       "processx"         
    ## [131] "progress"          "promises"         
    ## [133] "protolite"         "pryr"             
    ## [135] "ps"                "purrr"            
    ## [137] "qpdf"              "quantreg"         
    ## [139] "R6"                "rappdirs"         
    ## [141] "rapportools"       "raster"           
    ## [143] "rclipboard"        "rcmdcheck"        
    ## [145] "RColorBrewer"      "Rcpp"             
    ## [147] "RcppEigen"         "Rdpack"           
    ## [149] "readr"             "readstata13"      
    ## [151] "readxl"            "RefManageR"       
    ## [153] "rematch"           "remotes"          
    ## [155] "reprex"            "reshape"          
    ## [157] "reshape2"          "rex"              
    ## [159] "rgdal"             "rgeos"            
    ## [161] "Rgretl"            "rio"              
    ## [163] "rJava"             "rjson"            
    ## [165] "rlang"             "rmapshaper"       
    ## [167] "rmarkdown"         "roxygen2"         
    ## [169] "rprojroot"         "rstudioapi"       
    ## [171] "rversions"         "rvest"            
    ## [173] "sandwich"          "scales"           
    ## [175] "selectr"           "sessioninfo"      
    ## [177] "sf"                "shape"            
    ## [179] "shiny"             "shinyjs"          
    ## [181] "shinyWidgets"      "sourcetools"      
    ## [183] "sp"                "SparseM"          
    ## [185] "spData"            "stargazer"        
    ## [187] "stringi"           "stringr"          
    ## [189] "summarytools"      "sys"              
    ## [191] "testthat"          "tibble"           
    ## [193] "tidyr"             "tidyselect"       
    ## [195] "tidyverse"         "tigris"           
    ## [197] "tinytex"           "titanic"          
    ## [199] "tmap"              "tmaptools"        
    ## [201] "triebeard"         "units"            
    ## [203] "urltools"          "usethis"          
    ## [205] "utf8"              "uuid"             
    ## [207] "V8"                "vctrs"            
    ## [209] "viridis"           "viridisLite"      
    ## [211] "wbstats"           "webshot"          
    ## [213] "whisker"           "withr"            
    ## [215] "wooldridge"        "xfun"             
    ## [217] "xlsxjars"          "XML"              
    ## [219] "xml2"              "xopen"            
    ## [221] "xtable"            "yaml"             
    ## [223] "zip"               "zoo"              
    ## [225] "base"              "boot"             
    ## [227] "class"             "cluster"          
    ## [229] "codetools"         "compiler"         
    ## [231] "datasets"          "foreign"          
    ## [233] "graphics"          "grDevices"        
    ## [235] "grid"              "KernSmooth"       
    ## [237] "lattice"           "MASS"             
    ## [239] "Matrix"            "methods"          
    ## [241] "mgcv"              "nlme"             
    ## [243] "nnet"              "parallel"         
    ## [245] "rpart"             "spatial"          
    ## [247] "splines"           "stats"            
    ## [249] "stats4"            "survival"         
    ## [251] "tcltk"             "tools"            
    ## [253] "translations"      "utils"

``` r
# or
library()
```

To install and load a specific package use the following command.
Remember that you have to load the package everytime when you are in a
new R session.

``` r
install.packages("AER")
library(AER)
```

Some packages can contatin data. Inorder to access data from a specific
package use the following command.

``` r
## data(package = "AER")
data(SwissLabor, package = "AER") ; head(SwissLabor)
```

    ##   participation   income age education youngkids oldkids
    ## 1            no 10.78750 3.0         8         1       1
    ## 2           yes 10.52425 4.5         8         0       1
    ## 3            no 10.96858 4.6         9         0       0
    ## 4            no 11.10500 3.1        11         2       0
    ## 5            no 11.10847 4.4        12         0       2
    ## 6           yes 11.02825 4.2        12         0       1
    ##   foreign
    ## 1      no
    ## 2      no
    ## 3      no
    ## 4      no
    ## 5      no
    ## 6      no

Finally, to remove any R package use the function;

``` r
remove.packages("AER")
```

R Commands and Case Sensitivity
===============================

-   Technically R is an ‘expression language’ and is case sensitive, so
    `A` and `a` are different symbols and would refer to different
    variables.
-   Commands are seperated either by a new-line or a semi colon (;).
-   Comments can be put almost anywhere starting with a hashmark (\#).
-   If a command is not complete at the end of a line, R will give a
    different prompt, by default + on second and subsequent lines and
    continue to read input until the command is syntatically complete.

Expressions
===========

Examples of expressions in R include assignment statements, conditional
statements and arithmetic expressions.

``` r
x <- 1; x
```

    ## [1] 1

``` r
if (1>2) "yes" else "no"
```

    ## [1] "no"

Expressions are composed of objects and fuctions they may be seperated
with new lines or semicolons.

``` r
"hello how are you" ;100+50 ; sqrt(100) 
```

    ## [1] "hello how are you"

    ## [1] 150

    ## [1] 10

Objects
=======

An object is a thing that is represented by the computer.

-   The entries that R creates and manipulates are known as ‘objects’
    (more on this later).
-   During an R session objects are created and stored by name.
-   The R command `objects()` can be used to display the names of the
    objects that are currently stored within R.
-   The collection of objects currently stored is called the
    ‘workspace’.
-   To remove objects the function `rm()` is available

``` r
objects(); x <- c("my", 12, TRUE); x
```

    ##  [1] "a"                "A"               
    ##  [3] "Age"              "b"               
    ##  [5] "c1"               "c2"              
    ##  [7] "c3"               "char"            
    ##  [9] "comp"             "confidence"      
    ## [11] "confidenceLevels" "cyl_matrix"      
    ## [13] "d"                "d1"              
    ## [15] "d2"               "dat"             
    ## [17] "depth_cut"        "df"              
    ## [19] "DF"               "dframe"          
    ## [21] "dog"              "dt"              
    ## [23] "duck"             "e"               
    ## [25] "f"                "funny"           
    ## [27] "Funny"            "gender"          
    ## [29] "Gender"           "i"               
    ## [31] "interviewKolkata" "interviewLondon" 
    ## [33] "iris_col"         "iris_pch"        
    ## [35] "k"                "labs"            
    ## [37] "labs1"            "m"               
    ## [39] "m.lev"            "MaleSurvived"    
    ## [41] "marks"            "mean.mar.stu"    
    ## [43] "Month.Birth"      "my_df"           
    ## [45] "my_list"          "my_matrix"       
    ## [47] "my_vector"        "mydata"          
    ## [49] "mydatafile"       "myvec"           
    ## [51] "n"                "Name"            
    ## [53] "Names"            "newrecord"       
    ## [55] "no.na"            "nos"             
    ## [57] "num"              "num1"            
    ## [59] "num2"             "nums"            
    ## [61] "nums1"            "p"               
    ## [63] "party"            "party_fac"       
    ## [65] "party_fac_comb"   "party0"          
    ## [67] "party1"           "person"          
    ## [69] "prod"             "roll"            
    ## [71] "s"                "sex"             
    ## [73] "sex_fac"          "sex_fac_comb"    
    ## [75] "sex0"             "students"        
    ## [77] "SwissLabor"       "titanic_full"    
    ## [79] "titanic_test"     "titanic_test_mod"
    ## [81] "totalCol"         "totalRow"        
    ## [83] "x"                "y"               
    ## [85] "yes.na"           "z"

    ## [1] "my"   "12"   "TRUE"

``` r
objects()
```

    ##  [1] "a"                "A"               
    ##  [3] "Age"              "b"               
    ##  [5] "c1"               "c2"              
    ##  [7] "c3"               "char"            
    ##  [9] "comp"             "confidence"      
    ## [11] "confidenceLevels" "cyl_matrix"      
    ## [13] "d"                "d1"              
    ## [15] "d2"               "dat"             
    ## [17] "depth_cut"        "df"              
    ## [19] "DF"               "dframe"          
    ## [21] "dog"              "dt"              
    ## [23] "duck"             "e"               
    ## [25] "f"                "funny"           
    ## [27] "Funny"            "gender"          
    ## [29] "Gender"           "i"               
    ## [31] "interviewKolkata" "interviewLondon" 
    ## [33] "iris_col"         "iris_pch"        
    ## [35] "k"                "labs"            
    ## [37] "labs1"            "m"               
    ## [39] "m.lev"            "MaleSurvived"    
    ## [41] "marks"            "mean.mar.stu"    
    ## [43] "Month.Birth"      "my_df"           
    ## [45] "my_list"          "my_matrix"       
    ## [47] "my_vector"        "mydata"          
    ## [49] "mydatafile"       "myvec"           
    ## [51] "n"                "Name"            
    ## [53] "Names"            "newrecord"       
    ## [55] "no.na"            "nos"             
    ## [57] "num"              "num1"            
    ## [59] "num2"             "nums"            
    ## [61] "nums1"            "p"               
    ## [63] "party"            "party_fac"       
    ## [65] "party_fac_comb"   "party0"          
    ## [67] "party1"           "person"          
    ## [69] "prod"             "roll"            
    ## [71] "s"                "sex"             
    ## [73] "sex_fac"          "sex_fac_comb"    
    ## [75] "sex0"             "students"        
    ## [77] "SwissLabor"       "titanic_full"    
    ## [79] "titanic_test"     "titanic_test_mod"
    ## [81] "totalCol"         "totalRow"        
    ## [83] "x"                "y"               
    ## [85] "yes.na"           "z"

``` r
rm(x); objects()
```

    ##  [1] "a"                "A"               
    ##  [3] "Age"              "b"               
    ##  [5] "c1"               "c2"              
    ##  [7] "c3"               "char"            
    ##  [9] "comp"             "confidence"      
    ## [11] "confidenceLevels" "cyl_matrix"      
    ## [13] "d"                "d1"              
    ## [15] "d2"               "dat"             
    ## [17] "depth_cut"        "df"              
    ## [19] "DF"               "dframe"          
    ## [21] "dog"              "dt"              
    ## [23] "duck"             "e"               
    ## [25] "f"                "funny"           
    ## [27] "Funny"            "gender"          
    ## [29] "Gender"           "i"               
    ## [31] "interviewKolkata" "interviewLondon" 
    ## [33] "iris_col"         "iris_pch"        
    ## [35] "k"                "labs"            
    ## [37] "labs1"            "m"               
    ## [39] "m.lev"            "MaleSurvived"    
    ## [41] "marks"            "mean.mar.stu"    
    ## [43] "Month.Birth"      "my_df"           
    ## [45] "my_list"          "my_matrix"       
    ## [47] "my_vector"        "mydata"          
    ## [49] "mydatafile"       "myvec"           
    ## [51] "n"                "Name"            
    ## [53] "Names"            "newrecord"       
    ## [55] "no.na"            "nos"             
    ## [57] "num"              "num1"            
    ## [59] "num2"             "nums"            
    ## [61] "nums1"            "p"               
    ## [63] "party"            "party_fac"       
    ## [65] "party_fac_comb"   "party0"          
    ## [67] "party1"           "person"          
    ## [69] "prod"             "roll"            
    ## [71] "s"                "sex"             
    ## [73] "sex_fac"          "sex_fac_comb"    
    ## [75] "sex0"             "students"        
    ## [77] "SwissLabor"       "titanic_full"    
    ## [79] "titanic_test"     "titanic_test_mod"
    ## [81] "totalCol"         "totalRow"        
    ## [83] "y"                "yes.na"          
    ## [85] "z"

R has 5 basic/atomic classes of objects

> -   character: `"Hello"`
> -   numeric(real numbers/decimal numbers): `c(1,2.36)`.
> -   integer: `10L`
> -   complex :`2+4i`
> -   logical: `TRUE/FALSE`.

The most basic object is a vector. Vectors can contain objects of same
class only. However, `list()` is an exception and can contain a mixture
of objects.

`Inf` is a special number.

``` r
1/Inf
```

    ## [1] 0

``` r
Inf/Inf
```

    ## [1] NaN

`NaN` (Not A Number) is a value that represents an undefined value `NaN`
may represent missing values as well.

Objects in R have attributes like `names()`, `dimnames()` (for a matrix,
array or data frame), `class()`, `length()`.

``` r
class(10L)
```

    ## [1] "integer"

``` r
class("Hello!")
```

    ## [1] "character"

``` r
length(12)
```

    ## [1] 1

``` r
names(12)
```

    ## NULL

``` r
roll <- c(170, 150, 200)
names(roll) <- "Amit"; names(roll)
```

    ## [1] "Amit" NA     NA

``` r
names(roll) <- c("Amit", "Sourav", "Sneha"); names(roll)
```

    ## [1] "Amit"   "Sourav" "Sneha"

The things that we are typing/ we type in R are called expressions. `<-`
is called the assignment operator that assigns a value to a symbol.

``` r
num <- 1200
char <- "Hello!"
comp <- 2+4i
```

You can name an object in R almost anything you want, but there are a
few rules.

1.  First, a name cannot start with a number.
2.  Second, a name cannot use some special symbols,like `^`, `!`, `$`,
    `@`, `+`, `-`, `/`, or `*`.

Assignment can also be made using the function

``` r
assign("num", 1200 )
num
```

    ## [1] 1200

``` r
assign("nos", c(1, 1.2, 300, 45)); class(nos)
```

    ## [1] "numeric"

``` r
nos
```

    ## [1]   1.0   1.2 300.0  45.0

Sorting
=======

`sort(x)` returns a vector of same size as x with the elements arranged
in increasing order.

``` r
d <- c(10,50,12,63,74,1,89,5,3,6,4)
sort(d)
```

    ##  [1]  1  3  4  5  6 10 12 50 63 74 89

``` r
e <- c("anish", "zebra", "p", "e")
sort(e)
```

    ## [1] "anish" "e"     "p"     "zebra"

To sort in descending order use the argument `decreasing = TRUE`.

``` r
sort(d, decreasing  = TRUE)
```

    ##  [1] 89 74 63 50 12 10  6  5  4  3  1

Generating regular sequences
============================

``` r
x <- 1:30; x 
```

    ##  [1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17
    ## [18] 18 19 20 21 22 23 24 25 26 27 28 29 30

``` r
x <- 30:1; x
```

    ##  [1] 30 29 28 27 26 25 24 23 22 21 20 19 18 17 16 15 14
    ## [18] 13 12 11 10  9  8  7  6  5  4  3  2  1

``` r
x <- c(1,2,3,4,5,6,7,8,9); x
```

    ## [1] 1 2 3 4 5 6 7 8 9

``` r
x <- seq(1,30); x
```

    ##  [1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17
    ## [18] 18 19 20 21 22 23 24 25 26 27 28 29 30

``` r
x <- seq(-5, 5, by = 0.2); x
```

    ##  [1] -5.0 -4.8 -4.6 -4.4 -4.2 -4.0 -3.8 -3.6 -3.4 -3.2
    ## [11] -3.0 -2.8 -2.6 -2.4 -2.2 -2.0 -1.8 -1.6 -1.4 -1.2
    ## [21] -1.0 -0.8 -0.6 -0.4 -0.2  0.0  0.2  0.4  0.6  0.8
    ## [31]  1.0  1.2  1.4  1.6  1.8  2.0  2.2  2.4  2.6  2.8
    ## [41]  3.0  3.2  3.4  3.6  3.8  4.0  4.2  4.4  4.6  4.8
    ## [51]  5.0

``` r
x <- seq(10, 2, length.out = 5); x
```

    ## [1] 10  8  6  4  2

``` r
x <- seq(length = 51, from = -5, by = 0.2); x
```

    ##  [1] -5.0 -4.8 -4.6 -4.4 -4.2 -4.0 -3.8 -3.6 -3.4 -3.2
    ## [11] -3.0 -2.8 -2.6 -2.4 -2.2 -2.0 -1.8 -1.6 -1.4 -1.2
    ## [21] -1.0 -0.8 -0.6 -0.4 -0.2  0.0  0.2  0.4  0.6  0.8
    ## [31]  1.0  1.2  1.4  1.6  1.8  2.0  2.2  2.4  2.6  2.8
    ## [41]  3.0  3.2  3.4  3.6  3.8  4.0  4.2  4.4  4.6  4.8
    ## [51]  5.0

A related function is rep() which can be used for replicating objects in
various ways.

``` r
x <- c("hi","hello"); x
```

    ## [1] "hi"    "hello"

``` r
y <- rep(x, times = 2); y
```

    ## [1] "hi"    "hello" "hi"    "hello"

``` r
y <- rep(3, times = 10);y
```

    ##  [1] 3 3 3 3 3 3 3 3 3 3

The paste() function takes an arbitrary number of arguments and
concatenates one by one into character strings. Any numbers given among
the arguments are coerced into character strings.

``` r
x <- paste("a", 1:10, sep = "")
x
```

    ##  [1] "a1"  "a2"  "a3"  "a4"  "a5"  "a6"  "a7"  "a8" 
    ##  [9] "a9"  "a10"

To collapse the output into a single string pass the `collapse`
argument.

``` r
labs <- paste(c("x", "y"), 1:10, sep = "")
labs
```

    ##  [1] "x1"  "y2"  "x3"  "y4"  "x5"  "y6"  "x7"  "y8" 
    ##  [9] "x9"  "y10"

``` r
labs1 <- paste(c("x", "y"), 1:10, sep = "", collapse = "-")
labs1
```

    ## [1] "x1-y2-x3-y4-x5-y6-x7-y8-x9-y10"

Working directory
=================

To check the location of your workig derectory, use `getwd()`and to set
a specific folder as your working directory use `setwd("file path")`.

The “pass-by-value” and “pass-by-reference” in R
================================================

By defalut R uses “pass-by-value” paradigm. Consider the following
example;

``` r
x <- 1:10
x*2
```

    ##  [1]  2  4  6  8 10 12 14 16 18 20

``` r
x
```

    ##  [1]  1  2  3  4  5  6  7  8  9 10

``` r
# or consider
y <- x
x*3
```

    ##  [1]  3  6  9 12 15 18 21 24 27 30

``` r
y
```

    ##  [1]  1  2  3  4  5  6  7  8  9 10

> If you want to use the pass-by-reference paradigm, have a look at the
> `R.oo`, `mutatr` and `proto` packages..

Coercion
========

1.  Implicit Coercion
2.  Explicit Coercion

Implicit Coercion occurs when we try to combine objects of two or more
different classes. The ordering is roughly **LINCL** i.e
`logical < integer < numeric < complex < character<list`.

``` r
x <- c(1.7, "a"); class(x)
```

    ## [1] "character"

``` r
y <- c(TRUE, 2);class(y)
```

    ## [1] "numeric"

``` r
z <- c("a", TRUE);class(z)
```

    ## [1] "character"

We can explicitly coerce objects by using `as.*()` functions.

``` r
x <- c(0,1,2,3,4,5,6)
class(x)
```

    ## [1] "numeric"

``` r
as.character(x)
```

    ## [1] "0" "1" "2" "3" "4" "5" "6"

``` r
as.complex(x)
```

    ## [1] 0+0i 1+0i 2+0i 3+0i 4+0i 5+0i 6+0i

``` r
as.logical(x)
```

    ## [1] FALSE  TRUE  TRUE  TRUE  TRUE  TRUE  TRUE

Nonsensical coercion result in NAs. NA stands for Not Available.

``` r
x <- c("my", "name ", "is", "khan!")
as.numeric(x)
```

    ## Warning: NAs introduced by coercion

    ## [1] NA NA NA NA

``` r
as.complex(x)
```

    ## Warning: NAs introduced by coercion

    ## [1] NA NA NA NA

``` r
as.logical(x)
```

    ## [1] NA NA NA NA

Operations on Matrices
======================

Matrices are vectors with `dimension()` attribute.

``` r
m <- matrix(1:10, nrow = 2, ncol = 5)
m
```

    ##      [,1] [,2] [,3] [,4] [,5]
    ## [1,]    1    3    5    7    9
    ## [2,]    2    4    6    8   10

``` r
dim(m)
```

    ## [1] 2 5

``` r
length(m)
```

    ## [1] 10

``` r
class(m)
```

    ## [1] "matrix"

Filling direction of a matrix

``` r
m <- matrix(1:10, nrow = 2, ncol = 5); m
```

    ##      [,1] [,2] [,3] [,4] [,5]
    ## [1,]    1    3    5    7    9
    ## [2,]    2    4    6    8   10

``` r
m <- matrix(1:10, nrow = 2, ncol = 5, byrow = TRUE);m
```

    ##      [,1] [,2] [,3] [,4] [,5]
    ## [1,]    1    2    3    4    5
    ## [2,]    6    7    8    9   10

#### Row and column binding

This applies to multiple vectors of equal length column-binding and
row-biding to create matrices.

``` r
x <- 1:5
y <- 6:10
cbind(x,y)
```

    ##      x  y
    ## [1,] 1  6
    ## [2,] 2  7
    ## [3,] 3  8
    ## [4,] 4  9
    ## [5,] 5 10

``` r
rbind(x,y)
```

    ##   [,1] [,2] [,3] [,4] [,5]
    ## x    1    2    3    4    5
    ## y    6    7    8    9   10

``` r
# or
cbind(1:5, 6:10)
```

    ##      [,1] [,2]
    ## [1,]    1    6
    ## [2,]    2    7
    ## [3,]    3    8
    ## [4,]    4    9
    ## [5,]    5   10

#### Subsetting

Subsetting a matrix with `[` will subset objects of the same class

``` r
x <- matrix(1:10, 2, 5); x
```

    ##      [,1] [,2] [,3] [,4] [,5]
    ## [1,]    1    3    5    7    9
    ## [2,]    2    4    6    8   10

``` r
x[1,2]
```

    ## [1] 3

``` r
x[2,5]
```

    ## [1] 10

``` r
x[,2]
```

    ## [1] 3 4

``` r
x[2,]
```

    ## [1]  2  4  6  8 10

``` r
x[,1:3] # subset the first 3 columns of the matrix
```

    ##      [,1] [,2] [,3]
    ## [1,]    1    3    5
    ## [2,]    2    4    6

``` r
x[,c(2,4)] # subset the second and fourth columns
```

    ##      [,1] [,2]
    ## [1,]    3    7
    ## [2,]    4    8

``` r
x[1,c(2,4)] # subset the 1st row and second + fourth columns
```

    ## [1] 3 7

``` r
diag(x) # this works only for a square matrix
```

    ## [1] 1 4

When we subset a matrix it is seen that the output is a vector and not
in a matrix form. This can be corrected by setting `drop = FALSE`
argument.

``` r
x <- matrix(1:10, 2, 5); x
```

    ##      [,1] [,2] [,3] [,4] [,5]
    ## [1,]    1    3    5    7    9
    ## [2,]    2    4    6    8   10

``` r
colnames(x) <- c("Kolkata", "Delhi", "Mumbai", "Chennai", "Bangalore")
row.names(x) <- c("temp", "rain")
x
```

    ##      Kolkata Delhi Mumbai Chennai Bangalore
    ## temp       1     3      5       7         9
    ## rain       2     4      6       8        10

What is the temperature for Delhi?

``` r
x[1,3]
```

    ## [1] 5

Now let’s see the temperature values in all the cities.

``` r
x[1,]
```

    ##   Kolkata     Delhi    Mumbai   Chennai Bangalore 
    ##         1         3         5         7         9

How does the output look different with the `drop` argument?

``` r
x[1,3, drop = FALSE]
```

    ##      Mumbai
    ## temp      5

``` r
x[1,, drop = FALSE]
```

    ##      Kolkata Delhi Mumbai Chennai Bangalore
    ## temp       1     3      5       7         9

#### Omitting and Overwriting

``` r
x <- matrix(c(0.3,4.5,55.3,91,0.1,105.5,-4.2,8.2,27.9),nrow=3,ncol=3); x
```

    ##      [,1]  [,2] [,3]
    ## [1,]  0.3  91.0 -4.2
    ## [2,]  4.5   0.1  8.2
    ## [3,] 55.3 105.5 27.9

``` r
x[,-2]
```

    ##      [,1] [,2]
    ## [1,]  0.3 -4.2
    ## [2,]  4.5  8.2
    ## [3,] 55.3 27.9

``` r
x[-1,3:2] # notice the change in the positions too
```

    ##      [,1]  [,2]
    ## [1,]  8.2   0.1
    ## [2,] 27.9 105.5

``` r
x[-1,-2] # without first row and second column
```

    ##      [,1] [,2]
    ## [1,]  4.5  8.2
    ## [2,] 55.3 27.9

``` r
x[2,] <- 1:3
x[c(1,3),2] <- 900 # overwrites the second and the third row of the second column
x[c(1,3), c(1,3)] <- c(-7,7)
```

Replacing diagonals

``` r
diag(x) <- c(1,2,3)
```

#### Matrix transpose

``` r
t(x)
```

    ##      [,1] [,2] [,3]
    ## [1,]    1    1    7
    ## [2,]  900    2  900
    ## [3,]   -7    3    3

#### Creating identity matrix

``` r
i <- diag(3); i
```

    ##      [,1] [,2] [,3]
    ## [1,]    1    0    0
    ## [2,]    0    1    0
    ## [3,]    0    0    1

#### Scalar multiple of a matrix

``` r
a <- 2; a; x
```

    ## [1] 2

    ##      [,1] [,2] [,3]
    ## [1,]    1  900   -7
    ## [2,]    1    2    3
    ## [3,]    7  900    3

``` r
b <- a*x; b
```

    ##      [,1] [,2] [,3]
    ## [1,]    2 1800  -14
    ## [2,]    2    4    6
    ## [3,]   14 1800    6

``` r
a+b; a-b # Matrix addition and substraction
```

    ##      [,1] [,2] [,3]
    ## [1,]    4 1802  -12
    ## [2,]    4    6    8
    ## [3,]   16 1802    8

    ##      [,1]  [,2] [,3]
    ## [1,]    0 -1798   16
    ## [2,]    0    -2   -4
    ## [3,]  -12 -1798   -4

#### Matrix multiplication

> Note that matrix multiplication is not elementwise calculation, so the
> standard `*` cannot be used.

``` r
dim(x); dim(b)
```

    ## [1] 3 3

    ## [1] 3 3

``` r
x%*%b
```

    ##      [,1]  [,2] [,3]
    ## [1,] 1704 -7200 5344
    ## [2,]   48  7208   16
    ## [3,] 1856 21600 5320

#### Inverse of a matrix

``` r
A <- matrix(data=c(3,4,1,2),nrow=2,ncol=2);A 
```

    ##      [,1] [,2]
    ## [1,]    3    1
    ## [2,]    4    2

``` r
solve(A)
```

    ##      [,1] [,2]
    ## [1,]    1 -0.5
    ## [2,]   -2  1.5

An alternative way of creating a matrix using `dim()`.

``` r
m <- 1:10; m
```

    ##  [1]  1  2  3  4  5  6  7  8  9 10

``` r
dim(m) <- c(2,5)
m
```

    ##      [,1] [,2] [,3] [,4] [,5]
    ## [1,]    1    3    5    7    9
    ## [2,]    2    4    6    8   10

The functions `rowSums()` and `colSums()` calculate the total for each
row and column of a matrix.

``` r
a <- c(460.998, 314.4, 290.475, 247.900, 309.306, 165.8)
b <- matrix(a, nrow = 3, byrow = TRUE,
              dimnames = list(c("1","2", "3"), c("x", "y")))
b
```

    ##         x     y
    ## 1 460.998 314.4
    ## 2 290.475 247.9
    ## 3 309.306 165.8

``` r
totalRow <- rowSums(b); totalRow
```

    ##       1       2       3 
    ## 775.398 538.375 475.106

``` r
totalCol <- colSums(b); totalCol
```

    ##        x        y 
    ## 1060.779  728.100

Working with date and time
==========================

The `date()` function returns a character string of current date and
time.

``` r
date()
```

    ## [1] "Sun Apr 19 23:00:50 2020"

``` r
class(date())
```

    ## [1] "character"

The `Sys.Date()` rerturns the current day in the current time zone.

``` r
Sys.Date()
```

    ## [1] "2020-04-19"

``` r
class(Sys.Date())
```

    ## [1] "Date"

`Sys.time()` returns returns the absolute date-time value.

``` r
Sys.time()
```

    ## [1] "2020-04-19 23:00:50 IST"

### Formatting dates

The follwoing codes are required while formating dates.

| Code | Output that you get   |
|------|-----------------------|
| %d   | day as number (0-31)  |
| %a   | abbreviated weekday   |
| A    | Unabbreviated weekday |
| m    | months (00-12)        |
| b    | abbreviated month     |
| B    | unabbreviated month   |
| y    | two digit year        |
| Y    | Four digit year       |

``` r
d <- Sys.Date()
d
```

    ## [1] "2020-04-19"

``` r
format(d, "%d %B %Y")
```

    ## [1] "19 April 2020"

``` r
d1 <- format(d, "%d-%B-%Y")
d1; class(d1)
```

    ## [1] "19-April-2020"

    ## [1] "character"

### Creating dates

``` r
x <- c("1jan2016", "1feb2017", "1mar2018"); x
```

    ## [1] "1jan2016" "1feb2017" "1mar2018"

``` r
k <- as.Date(x, "%d %b %Y");k; class(k)
```

    ## [1] "2016-01-01" "2017-02-01" "2018-03-01"

    ## [1] "Date"

``` r
d2 <- Sys.time()
d2
```

    ## [1] "2020-04-19 23:00:50 IST"

``` r
format(d2, "%d-%B-%Y %H:%M:%S %Y")
```

    ## [1] "19-April-2020 23:00:50 2020"

There are basically two major data types related to time

1.  **POSIXct:** **(Portable Operating System Interface)** *ct* stands
    for calander time. It is the number of seconds since 1-Jan-1970.
    Negative numbers represent the number of seconds before this time.
2.  **POSIXlt:** *lt* stands for local time and is a named list of
    vectors representing seconds, minutes, hour, day, month, year and
    time zones.

``` r
# current time as POSIXct
unclass(Sys.time()) # What does unclass do?
```

    ## [1] 1587317451

``` r
# as POSIXlt
unclass(as.POSIXlt(Sys.time()))
```

    ## $sec
    ## [1] 50.63232
    ## 
    ## $min
    ## [1] 0
    ## 
    ## $hour
    ## [1] 23
    ## 
    ## $mday
    ## [1] 19
    ## 
    ## $mon
    ## [1] 3
    ## 
    ## $year
    ## [1] 120
    ## 
    ## $wday
    ## [1] 0
    ## 
    ## $yday
    ## [1] 109
    ## 
    ## $isdst
    ## [1] 0
    ## 
    ## $zone
    ## [1] "IST"
    ## 
    ## $gmtoff
    ## [1] 19800
    ## 
    ## attr(,"tzone")
    ## [1] ""      "IST"   "+0630"

Working with dates and time with `lubridate()`.

``` r
## install.packages("lubridate")
library(lubridate)
y <- ymd("2018-08-07");y; class(y)
```

    ## [1] "2018-08-07"

    ## [1] "Date"

``` r
dmy(180807)
```

    ## [1] "2007-08-18"

``` r
ydm(180807)
```

    ## [1] "2018-07-08"

You can also add the hour, minute and second information.

``` r
dmy_hms("08-09-2019 08:30:00")
```

    ## [1] "2019-09-08 08:30:00 UTC"

### Time zones.

For example, you have a scheduled admission interview over Skype in a
University in London on 25 Sept 2019 at 09:45 am, what time shall it be
for you in Kolkata?

``` r
Sys.timezone() # System time zone
```

    ## [1] "Asia/Calcutta"

``` r
head(OlsonNames(), 20) # Time zone directory
```

    ##  [1] "Africa/Abidjan"       "Africa/Accra"        
    ##  [3] "Africa/Addis_Ababa"   "Africa/Algiers"      
    ##  [5] "Africa/Asmara"        "Africa/Asmera"       
    ##  [7] "Africa/Bamako"        "Africa/Bangui"       
    ##  [9] "Africa/Banjul"        "Africa/Bissau"       
    ## [11] "Africa/Blantyre"      "Africa/Brazzaville"  
    ## [13] "Africa/Bujumbura"     "Africa/Cairo"        
    ## [15] "Africa/Casablanca"    "Africa/Ceuta"        
    ## [17] "Africa/Conakry"       "Africa/Dakar"        
    ## [19] "Africa/Dar_es_Salaam" "Africa/Djibouti"

``` r
interviewLondon <- dmy_hms("25-Sep-2019 09:45:00", tz = "Europe/London")
interviewLondon
```

    ## [1] "2019-09-25 09:45:00 BST"

``` r
interviewKolkata <- with_tz(interviewLondon,tz = "Asia/Calcutta")
interviewKolkata
```

    ## [1] "2019-09-25 14:15:00 IST"

> So your interview timings are; (a) 2019-09-25 09:45:00 if you are in
> London, and (b) 2019-09-25 14:15:00 if you are in Kolkata.

Logical Operators
=================

<table class="table table-bordered" style="width: auto !important; margin-left: auto; margin-right: auto;">
<thead>
<tr>
<th style="text-align:left;">
Operator
</th>
<th style="text-align:left;">
Interpretation
</th>
<th style="text-align:left;">
Results
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;vertical-align: middle !important;" rowspan="4">
&
</td>
<td style="text-align:left;vertical-align: middle !important;" rowspan="4">
AND (element-wise)
</td>
<td style="text-align:left;">
TRUE & TRUE = TRUE
</td>
</tr>
<tr>
<td style="text-align:left;">
TRUE & FALSE = FALSE
</td>
</tr>
<tr>
<td style="text-align:left;">
FALSE & TRUE = FALSE
</td>
</tr>
<tr>
<td style="text-align:left;">
FALSE & FALSE = FALSE
</td>
</tr>
<tr>
<td style="text-align:left;">
&&
</td>
<td style="text-align:left;">
AND (single comparison)
</td>
<td style="text-align:left;">
same as above
</td>
</tr>
<tr>
<td style="text-align:left;vertical-align: middle !important;" rowspan="4">
\|
</td>
<td style="text-align:left;vertical-align: middle !important;" rowspan="4">
OR (element-wise)
</td>
<td style="text-align:left;">
TRUE \| TRUE = TRUE
</td>
</tr>
<tr>
<td style="text-align:left;">
TRUE \| FALSE is TRUE
</td>
</tr>
<tr>
<td style="text-align:left;">
FALSE \| TRUE is TRUE
</td>
</tr>
<tr>
<td style="text-align:left;">
FALSE \| FALSE is FALSE
</td>
</tr>
<tr>
<td style="text-align:left;">
\|\|
</td>
<td style="text-align:left;">
OR (single comparison)
</td>
<td style="text-align:left;">
same as above
</td>
</tr>
<tr>
<td style="text-align:left;vertical-align: middle !important;" rowspan="2">
!
</td>
<td style="text-align:left;vertical-align: middle !important;" rowspan="2">
NOT
</td>
<td style="text-align:left;">
!TRUE = FALSE
</td>
</tr>
<tr>
<td style="text-align:left;">
!FALSE = TRUE
</td>
</tr>
</tbody>
</table>

Some examples

``` r
a <- c(T,F,T,F); a
```

    ## [1]  TRUE FALSE  TRUE FALSE

``` r
b <- c(F,T,T,T); b
```

    ## [1] FALSE  TRUE  TRUE  TRUE

``` r
a&b; a&&b
```

    ## [1] FALSE FALSE  TRUE FALSE

    ## [1] FALSE

``` r
a|b; a||b
```

    ## [1] TRUE TRUE TRUE TRUE

    ## [1] TRUE

### Logical subsetting and extraction

``` r
myvec <- c(5,-2.3,4,4,4,6,8,10,40221,-8)
myvec[c(F,T,F,F,F,F,F,F,F,T)] # extracts the negative numbers in the vector
```

    ## [1] -2.3 -8.0

``` r
myvec<0
```

    ##  [1] FALSE  TRUE FALSE FALSE FALSE FALSE FALSE FALSE
    ##  [9] FALSE  TRUE

``` r
myvec[myvec < 0] # same operation as above
```

    ## [1] -2.3 -8.0

To extract every second elment from the vector starting with the first

``` r
myvec[c(T,F)] # the flag vector c(T,F) is recycled if it's too short.
```

    ## [1]     5     4     4     8 40221

Relational and logical operators together

``` r
myvec[(myvec>0) & (myvec < 1000)]
```

    ## [1]  5  4  4  4  6  8 10

Identifying the index positions of a vector

``` r
which(myvec < 0)
```

    ## [1]  2 10

Let’s apply logical subsetting and extraction in matrices as an example.
In the following example we shall

1.  Extract elements from a row or column.
2.  Change the elements in the matrix.

``` r
A <- matrix(c(0.3,4.5,55.3,91,0.1,105.5,-4.2,8.2,27.9),nrow=3,ncol=3); A
```

    ##      [,1]  [,2] [,3]
    ## [1,]  0.3  91.0 -4.2
    ## [2,]  4.5   0.1  8.2
    ## [3,] 55.3 105.5 27.9

``` r
A[c(T,F,F),c(F,T,T)] #extracts the second and the third elements of first row. c(T, F,F) selects the first row, c(F,T,T) selects the elements from the selected first row.
```

    ## [1] 91.0 -4.2

``` r
A[c(F,T,F),c(F,T,T)] #extracts the second and the third elements of second row.
```

    ## [1] 0.1 8.2

``` r
A[A<1] <- 100 # Changes the elements in the matrix with values less than 1.
A
```

    ##       [,1]  [,2]  [,3]
    ## [1,] 100.0  91.0 100.0
    ## [2,]   4.5 100.0   8.2
    ## [3,]  55.3 105.5  27.9

More on Characters
==================

Let’ create a character string and assign it to **s**.

``` r
s <- "This is a character string"
```

We can check the length and number of characters in `s`.

``` r
length(s)
```

    ## [1] 1

``` r
nchar(s)
```

    ## [1] 26

### Escape Sequences

| Sequence         | Result                     |
|------------------|----------------------------|
|  ∖ *n*           | Starts a new line          |
|  ∖ *t*           | Horizontal tab             |
|  ∖ *b*           | Invokes a backspace        |
|  ∖ ∖             | Used as a single backslash |
| $\\backslash{"}$ | Includes a double quote    |

Example

``` r
cat("here is a string \n split \t to neww\b \n\n\t lines")
```

    ## here is a string 
    ##  split    to neww 
    ## 
    ##   lines

### substring and matching

The function `substr()` takes a string **x** and extracts the part of
the string between two character positions (inclusive)

``` r
substr(s, start = 11, stop = 19)
```

    ## [1] "character"

``` r
substr(s, start = 11, stop = 19) <- "CHARACTER"
```

Its more easier to do with `sub()` and `gsub()`

``` r
duck <- "Mother duck said quack, quack, quack."
duck
```

    ## [1] "Mother duck said quack, quack, quack."

``` r
dog <- sub(pattern = "duck", replacement = "dog", duck )
dog
```

    ## [1] "Mother dog said quack, quack, quack."

``` r
gsub(pattern = "quack", replacement = "bow", dog)
```

    ## [1] "Mother dog said bow, bow, bow."

Factors
=======

-   Factors represent categorical data.
-   Factors can be ordered or unordered.
-   Factors can be thought as integer vector with labels, like 1 means
    ‘low’, 2 means ‘high’, 3 means ‘very high’.
-   Example data set
    <table class="table table-striped table-hover" style="width: auto !important; margin-left: auto; margin-right: auto;">
    <thead>
    <tr>
    <th style="text-align:left;">
    Names
    </th>
    <th style="text-align:left;">
    Gender
    </th>
    <th style="text-align:left;">
    Month.Birth
    </th>
    </tr>
    </thead>
    <tbody>
    <tr>
    <td style="text-align:left;">
    Kunal
    </td>
    <td style="text-align:left;">
    Male
    </td>
    <td style="text-align:left;">
    January
    </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    Ben
    </td>
    <td style="text-align:left;">
    Male
    </td>
    <td style="text-align:left;">
    March
    </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    Kritika
    </td>
    <td style="text-align:left;">
    Female
    </td>
    <td style="text-align:left;">
    March
    </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    Reena
    </td>
    <td style="text-align:left;">
    Female
    </td>
    <td style="text-align:left;">
    December
    </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    Narendra
    </td>
    <td style="text-align:left;">
    Male
    </td>
    <td style="text-align:left;">
    October
    </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    Smriti
    </td>
    <td style="text-align:left;">
    Female
    </td>
    <td style="text-align:left;">
    October
    </td>
    </tr>
    </tbody>
    </table>

We can create factors using the information in the above table:

``` r
(Names <- c("Kunal", "Ben", "Kritika", "Reena", "Narendra", "Smriti"))
```

    ## [1] "Kunal"    "Ben"      "Kritika"  "Reena"   
    ## [5] "Narendra" "Smriti"

``` r
(Gender <- factor(c("Male", "Male", "Female", "Female", "Male", "Female")))
```

    ## [1] Male   Male   Female Female Male   Female
    ## Levels: Female Male

``` r
(Month.Birth <- factor(c("January", "March", "March", "December", "October", "October")))
```

    ## [1] January  March    March    December October  October 
    ## Levels: December January March October

``` r
(Month.Birth <- factor(c("January", "March", "March", "December", "October", "October"), levels = c("January", "March", "October", "December")))
```

    ## [1] January  March    March    December October  October 
    ## Levels: January March October December

Extraction and subsetting
-------------------------

Which boy was born in March?

``` r
Names[Gender == "Male" & Month.Birth == "March"]
```

    ## [1] "Ben"

Releveling a factor
-------------------

``` r
(levels(Month.Birth) <- c(1, 3, 10, 12))
```

    ## [1]  1  3 10 12

``` r
(levels(Gender) <- c(0, 1)) # 0 indicates female
```

    ## [1] 0 1

Defining and Ordering levels
----------------------------

``` r
(m <- c("January", "March", "March", "December", "October", "October"))
```

    ## [1] "January"  "March"    "March"    "December"
    ## [5] "October"  "October"

``` r
(Month.Birth <- factor(m))
```

    ## [1] January  March    March    December October  October 
    ## Levels: December January March October

``` r
(Month.Birth <- factor(m, ordered = TRUE))
```

    ## [1] January  March    March    December October  October 
    ## Levels: December < January < March < October

``` r
# we can explicity convert it to an ordered level
m.lev <- c("January", "March", "October", "December")
Month.Birth <- factor(m,levels = m.lev, ordered = TRUE)
levels(Month.Birth)
```

    ## [1] "January"  "March"    "October"  "December"

``` r
# Checking the order
Month.Birth[1] < Month.Birth[5]
```

    ## [1] TRUE

Cutting/binning
---------------

Suppose you want to bin **y** into **small\[0,2)**, **medium\[2,4)**,
and **large \[4,6\]**

``` r
y <- c(0.53,5.4,1.5,3.33,0.45,0.01,2,4.2,1.99,1.01)
table(cut(y, breaks = c(0,2,4,6), right = FALSE))
```

    ## 
    ## [0,2) [2,4) [4,6) 
    ##     6     2     2

``` r
table(cut(y, breaks = c(0,2,4,6), right = FALSE, include.lowest = TRUE)) # Note. include.lowest = TRUE only if right = FALSE
```

    ## 
    ## [0,2) [2,4) [4,6] 
    ##     6     2     2

``` r
table(cut(y, breaks = c(0,2,4,6), right = FALSE, include.lowest = TRUE, 
    labels = c("small","medium", "large")))
```

    ## 
    ##  small medium  large 
    ##      6      2      2

Lists
=====

-   Lists are sepecial types of vectors which can contain elements of
    different classes. You can also have a list as a component of
    another list.
-   A single list can contain a numeric matrix, a logical array, a
    single character string, and a factor object.

``` r
(x <- list(10:20, "Khan", 1+2i, TRUE)); length(x)
```

    ## [[1]]
    ##  [1] 10 11 12 13 14 15 16 17 18 19 20
    ## 
    ## [[2]]
    ## [1] "Khan"
    ## 
    ## [[3]]
    ## [1] 1+2i
    ## 
    ## [[4]]
    ## [1] TRUE

    ## [1] 4

``` r
(f <- list(matrix(data = 1:4, nrow = 2, ncol = 2), x)); length(f)
```

    ## [[1]]
    ##      [,1] [,2]
    ## [1,]    1    3
    ## [2,]    2    4
    ## 
    ## [[2]]
    ## [[2]][[1]]
    ##  [1] 10 11 12 13 14 15 16 17 18 19 20
    ## 
    ## [[2]][[2]]
    ## [1] "Khan"
    ## 
    ## [[2]][[3]]
    ## [1] 1+2i
    ## 
    ## [[2]][[4]]
    ## [1] TRUE

    ## [1] 2

We can create lists out of vectors, matrices and data frames.

``` r
my_vector <- 1:10 
my_matrix <- matrix(1:9, ncol = 3)
my_df <- mtcars[1:10,] # to know about `mtcars` use ?mtcars

# Construct list with these different elements:
(my_list <- list(my_vector, my_matrix, my_df)) 
```

    ## [[1]]
    ##  [1]  1  2  3  4  5  6  7  8  9 10
    ## 
    ## [[2]]
    ##      [,1] [,2] [,3]
    ## [1,]    1    4    7
    ## [2,]    2    5    8
    ## [3,]    3    6    9
    ## 
    ## [[3]]
    ##                    mpg cyl  disp  hp drat    wt  qsec vs
    ## Mazda RX4         21.0   6 160.0 110 3.90 2.620 16.46  0
    ## Mazda RX4 Wag     21.0   6 160.0 110 3.90 2.875 17.02  0
    ## Datsun 710        22.8   4 108.0  93 3.85 2.320 18.61  1
    ## Hornet 4 Drive    21.4   6 258.0 110 3.08 3.215 19.44  1
    ## Hornet Sportabout 18.7   8 360.0 175 3.15 3.440 17.02  0
    ## Valiant           18.1   6 225.0 105 2.76 3.460 20.22  1
    ## Duster 360        14.3   8 360.0 245 3.21 3.570 15.84  0
    ## Merc 240D         24.4   4 146.7  62 3.69 3.190 20.00  1
    ## Merc 230          22.8   4 140.8  95 3.92 3.150 22.90  1
    ## Merc 280          19.2   6 167.6 123 3.92 3.440 18.30  1
    ##                   am gear carb
    ## Mazda RX4          1    4    4
    ## Mazda RX4 Wag      1    4    4
    ## Datsun 710         1    4    1
    ## Hornet 4 Drive     0    3    1
    ## Hornet Sportabout  0    3    2
    ## Valiant            0    3    1
    ## Duster 360         0    3    4
    ## Merc 240D          0    4    2
    ## Merc 230           0    4    2
    ## Merc 280           0    4    4

``` r
# Adapt list() call to give the components names
(my_list <- list(vector = my_vector, matrix =  my_matrix, dataframe = my_df))
```

    ## $vector
    ##  [1]  1  2  3  4  5  6  7  8  9 10
    ## 
    ## $matrix
    ##      [,1] [,2] [,3]
    ## [1,]    1    4    7
    ## [2,]    2    5    8
    ## [3,]    3    6    9
    ## 
    ## $dataframe
    ##                    mpg cyl  disp  hp drat    wt  qsec vs
    ## Mazda RX4         21.0   6 160.0 110 3.90 2.620 16.46  0
    ## Mazda RX4 Wag     21.0   6 160.0 110 3.90 2.875 17.02  0
    ## Datsun 710        22.8   4 108.0  93 3.85 2.320 18.61  1
    ## Hornet 4 Drive    21.4   6 258.0 110 3.08 3.215 19.44  1
    ## Hornet Sportabout 18.7   8 360.0 175 3.15 3.440 17.02  0
    ## Valiant           18.1   6 225.0 105 2.76 3.460 20.22  1
    ## Duster 360        14.3   8 360.0 245 3.21 3.570 15.84  0
    ## Merc 240D         24.4   4 146.7  62 3.69 3.190 20.00  1
    ## Merc 230          22.8   4 140.8  95 3.92 3.150 22.90  1
    ## Merc 280          19.2   6 167.6 123 3.92 3.440 18.30  1
    ##                   am gear carb
    ## Mazda RX4          1    4    4
    ## Mazda RX4 Wag      1    4    4
    ## Datsun 710         1    4    1
    ## Hornet 4 Drive     0    3    1
    ## Hornet Sportabout  0    3    2
    ## Valiant            0    3    1
    ## Duster 360         0    3    4
    ## Merc 240D          0    4    2
    ## Merc 230           0    4    2
    ## Merc 280           0    4    4

``` r
# print out the vector from the list
my_list[[1]]
```

    ##  [1]  1  2  3  4  5  6  7  8  9 10

``` r
# now print the second element in the vector
my_list[[1]][2]
```

    ## [1] 2

``` r
my_list[[3]][1]
```

    ##                    mpg
    ## Mazda RX4         21.0
    ## Mazda RX4 Wag     21.0
    ## Datsun 710        22.8
    ## Hornet 4 Drive    21.4
    ## Hornet Sportabout 18.7
    ## Valiant           18.1
    ## Duster 360        14.3
    ## Merc 240D         24.4
    ## Merc 230          22.8
    ## Merc 280          19.2

``` r
my_list[[3]]["disp"]
```

    ##                    disp
    ## Mazda RX4         160.0
    ## Mazda RX4 Wag     160.0
    ## Datsun 710        108.0
    ## Hornet 4 Drive    258.0
    ## Hornet Sportabout 360.0
    ## Valiant           225.0
    ## Duster 360        360.0
    ## Merc 240D         146.7
    ## Merc 230          140.8
    ## Merc 280          167.6

The retrieved component of a list can be treated as a stand-alone
object. For e.g

``` r
f <- list(matrix(data=1:4,nrow=2,ncol=2),c(T,F,T,T),"hello")
f[[1]] # retrieves the matrix
```

    ##      [,1] [,2]
    ## [1,]    1    3
    ## [2,]    2    4

``` r
# performing normal operations
f[[1]] + 5.5 
```

    ##      [,1] [,2]
    ## [1,]  6.5  8.5
    ## [2,]  7.5  9.5

``` r
f[[1]][1,2]
```

    ## [1] 3

``` r
cat(f[[3]], "you!" )
```

    ## hello you!

To overwrite a member of `f`, the assignment operator can be used.

``` r
f[[3]] <- paste(f[[3]], "you!"); f
```

    ## [[1]]
    ##      [,1] [,2]
    ## [1,]    1    3
    ## [2,]    2    4
    ## 
    ## [[2]]
    ## [1]  TRUE FALSE  TRUE  TRUE
    ## 
    ## [[3]]
    ## [1] "hello you!"

Inorder to access the second and third components of `f`, we use `[]`
instead of `[[]]` because using double brackets on a list is always
interpreted with respect to a single member. This is referred to as
**list slicing** and lets you select multiple list items at once.

``` r
(f[c(2,3)])
```

    ## [[1]]
    ## [1]  TRUE FALSE  TRUE  TRUE
    ## 
    ## [[2]]
    ## [1] "hello you!"

Naming list components
----------------------

We can name list components using `name()`:

``` r
names(f) <- c("matrix", "logical", "char"); f
```

    ## $matrix
    ##      [,1] [,2]
    ## [1,]    1    3
    ## [2,]    2    4
    ## 
    ## $logical
    ## [1]  TRUE FALSE  TRUE  TRUE
    ## 
    ## $char
    ## [1] "hello you!"

You can now perform member referencing using these names and the `$`
operator, rather than the double square brackets.

``` r
f$matrix
```

    ##      [,1] [,2]
    ## [1,]    1    3
    ## [2,]    2    4

``` r
f$logical
```

    ## [1]  TRUE FALSE  TRUE  TRUE

Nesting lists
-------------

-   A member of a list can itself be a list.

``` r
f
```

    ## $matrix
    ##      [,1] [,2]
    ## [1,]    1    3
    ## [2,]    2    4
    ## 
    ## $logical
    ## [1]  TRUE FALSE  TRUE  TRUE
    ## 
    ## $char
    ## [1] "hello you!"

``` r
names(x) <- c("num", "char", "complex", "logical" ); x
```

    ## $num
    ##  [1] 10 11 12 13 14 15 16 17 18 19 20
    ## 
    ## $char
    ## [1] "Khan"
    ## 
    ## $complex
    ## [1] 1+2i
    ## 
    ## $logical
    ## [1] TRUE

``` r
f$list_x <- x; f 
```

    ## $matrix
    ##      [,1] [,2]
    ## [1,]    1    3
    ## [2,]    2    4
    ## 
    ## $logical
    ## [1]  TRUE FALSE  TRUE  TRUE
    ## 
    ## $char
    ## [1] "hello you!"
    ## 
    ## $list_x
    ## $list_x$num
    ##  [1] 10 11 12 13 14 15 16 17 18 19 20
    ## 
    ## $list_x$char
    ## [1] "Khan"
    ## 
    ## $list_x$complex
    ## [1] 1+2i
    ## 
    ## $list_x$logical
    ## [1] TRUE

To retreive members of the inner list;

``` r
f$list_x$num[c(1,3,6)]
```

    ## [1] 10 12 15

Data frames
===========

-   Data frames are used to store tabular data.
-   Data frames have an advantage over matrices in that they can store
    objects of different classes.
-   So in a way data frames are a collection of lists with the same
    length.

``` r
(x <- data.frame(Sl = 1:4, Countries = c("Germany", "Brazil", "Argentina", "France"), Rank = c(1,3,2,4))
)
```

    ##   Sl Countries Rank
    ## 1  1   Germany    1
    ## 2  2    Brazil    3
    ## 3  3 Argentina    2
    ## 4  4    France    4

``` r
dim(x)
```

    ## [1] 4 3

-   Each row in the data frame is called a ‘record’ and each column
    called ‘variable’.
-   Portions of data can be extracted with `[]`

``` r
x[1,2] # this gives the element at row 1, col 2
```

    ## [1] Germany
    ## Levels: Argentina Brazil France Germany

``` r
# or 
x$Countries[1]
```

    ## [1] Germany
    ## Levels: Argentina Brazil France Germany

Each variables retain their class upon extraction. For e.g

``` r
class(x$Countries)
```

    ## [1] "factor"

Lets look at another example

``` r
Name <-  c("Kunal", "Ben", "Kritika", "Reena", "Narendra", "Smriti")
Gender <- c("M", "M", "F", "F", "M", "F")
Age <- c(20, 18, 30, 24, 24, 27)
mydata <- data.frame(Name, Gender, Age)
class(mydata$Name)
```

    ## [1] "factor"

To prevent this automatic conversion of strings to factors when using
`data.frame`, set the optional argument `stringsAsFactors = FALSE`.

``` r
mydata <- data.frame(Name, Gender, Age, stringsAsFactors = FALSE)
class(mydata$Name)
```

    ## [1] "character"

Adding data columns and combining data frames
---------------------------------------------

``` r
newrecord <- data.frame(Name = "Manoj", Gender = "M", Age = 18)
(mydata <- rbind(mydata, newrecord))
```

    ##       Name Gender Age
    ## 1    Kunal      M  20
    ## 2      Ben      M  18
    ## 3  Kritika      F  30
    ## 4    Reena      F  24
    ## 5 Narendra      M  24
    ## 6   Smriti      F  27
    ## 7    Manoj      M  18

Lets create a new column

``` r
Funny <- c("High","High","Low","Med","High","Med", "High")
(Funny <- factor(x=Funny,levels=c("Low","Med","High")))
```

    ## [1] High High Low  Med  High Med  High
    ## Levels: Low Med High

Using `cbind()` we can now add this column

``` r
dim(mydata); length(Funny)
```

    ## [1] 7 3

    ## [1] 7

``` r
(mydata <- cbind(mydata, Funny))
```

    ##       Name Gender Age Funny
    ## 1    Kunal      M  20  High
    ## 2      Ben      M  18  High
    ## 3  Kritika      F  30   Low
    ## 4    Reena      F  24   Med
    ## 5 Narendra      M  24  High
    ## 6   Smriti      F  27   Med
    ## 7    Manoj      M  18  High

Logical Record Subsets
----------------------

Say you want to subset using a particular level. Lets look at the
`'mydata'` example

``` r
names(mydata)
```

    ## [1] "Name"   "Gender" "Age"    "Funny"

Lets subset the data frame only for males

``` r
mydata[mydata$Gender == "M",]
```

    ##       Name Gender Age Funny
    ## 1    Kunal      M  20  High
    ## 2      Ben      M  18  High
    ## 5 Narendra      M  24  High
    ## 7    Manoj      M  18  High

Since the subset belongs only to males, you could now remove the Gender
column

``` r
mydata[mydata$Gender == "M", -2]
```

    ##       Name Age Funny
    ## 1    Kunal  20  High
    ## 2      Ben  18  High
    ## 5 Narendra  24  High
    ## 7    Manoj  18  High

Let’s extract from mydata the full records for individuals who are more
than 20 years old AND/OR have a high degree of funniness.

``` r
(mydata[mydata$Age >= 20 & mydata$Funny == "High",])
```

    ##       Name Gender Age Funny
    ## 1    Kunal      M  20  High
    ## 5 Narendra      M  24  High

``` r
(mydata[mydata$Age >= 20 | mydata$Funny == "Low",])
```

    ##       Name Gender Age Funny
    ## 1    Kunal      M  20  High
    ## 3  Kritika      F  30   Low
    ## 4    Reena      F  24   Med
    ## 5 Narendra      M  24  High
    ## 6   Smriti      F  27   Med

Basic plotting
==============

Coordinate vectors
------------------

-   R has incredibly flexible plotting tools for data and model
    visualisations.
-   Treat your screen as a blan, 2 dimensional canvas.
-   Plot points using x- and y- coordinates.
-   The `plot()` function takes two vectors (x and y) and opens a
    *graphics device* where it displays the result.
-   If a graphics device is already open, R’s default behaviour is to
    refresh the device, overwriting the current contents with the new
    plot.

``` r
f <- c(1.1,2,3.5,3.9,4.2)
b <- c(2,2.2,-1.3,0,0.2)
plot(f,b)
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-95-1.png)

You could also use a matrix instead. Try this one!

``` r
plot(cbind(f,b))
```

Plot types
----------

The arguments that enter the `plot()` function are called graphical
parameters. Some most commonly used graphical parameters are **type**,
**main**, **xlab**, **ylab**, **col**, **pch**, **cex** (character
expansion), **lty**, **lwd**, **xlim**, **ylim**.

``` r
plot(f,b, type = "l")
plot(f,b, type = "b")
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-97-1.png)

Title and axis labels
---------------------

``` r
plot(f,b, type = "o", main = "My Title", xlab = "My x-axis label", ylab = "My y-axis label")
plot(f,b, type = "s", main = "My Title", xlab = "", ylab = "")
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-98-1.png)

Colour
------

``` r
plot(f,b, type = "o", main = "My Title", col = "firebrick4", xlab = "", ylab = "")
title(xlab = "My X-axis label", col.lab = "green")
title(ylab = "My Y-axis label", col.lab = "blue")
plot(f,b, type = "s", main = "My Title", xlab = "", ylab = "", col = "gold", col.main = "red")
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-99-1.png)

<html>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<object width="100%" height="500" data="https://www.nceas.ucsb.edu/~frazier/RSpatialGuides/colorPaletteCheatsheet.pdf">
</object>
If the above pdf is not displayed in your mobile, click
[here](https://www.nceas.ucsb.edu/~frazier/RSpatialGuides/colorPaletteCheatsheet.pdf)
to download the pdf.
<p>
**Source**:[www.nceas.ucsb.edu](https://www.nceas.ucsb.edu/~frazier/RSpatialGuides/colorPaletteCheatsheet.pdf)
</p>
</html>

Appearances
-----------

Use `?par()`, `?pch()` to know about graphical parameters in
appearances.

``` r
plot(f,b, type = "o", main = "My Title", col = "firebrick4", xlab = "", ylab = "", xlim = c(2,3))
title(xlab = "My X-axis label", col.lab = "green")
title(ylab = "My Y-axis label", col.lab = "blue")
plot(f,b, type = "s", main = "My Title", xlab = "", ylab = "", col = "gold", col.main = "red", ylim = c(0, 2))
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-100-1.png)

``` r
plot(f,b, type = "o", main = "My Title", col = "firebrick4", xlab = "", ylab = "", pch = 4)
title(xlab = "My X-axis label", col.lab = "green")
title(ylab = "My Y-axis label", col.lab = "blue")
plot(f,b, type = "b", main = "My Title", xlab = "", ylab = "", col = "blue", col.main = "red", pch = 10)
plot(f,b, type = "o", main = "My Title", col = "firebrick4", xlab = "", ylab = "", pch = 4, lwd = 4)
title(xlab = "My X-axis label", col.lab = "green")
title(ylab = "My Y-axis label", col.lab = "blue")
plot(f,b, type = "b", main = "My Title", xlab = "", ylab = "", col = "blue", col.main = "red", pch = 10, lwd = 6)
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-101-1.png)

Adding Points, Lines, and Text
------------------------------

-   Normally `plot()` refreshes the active graphics device for a new
    plotting region.
-   We might want to add points, lines and text to an existing plot.
-   Some useful functions include:
    -   `points()`: adds points
    -   `lines()`, `abline()`, `segments()`: adds lines
    -   `text()`: writes text
    -   `arrows()`: adds arrows
    -   `legend()`: adds a legend

Lets consider an example. We shall recreate the following plot. The data
points will be plotted differently according to their `x` and `y`
locations, depending on their relation to the “sweet spot” pointed out
in the figure.

-   Points with a `y` value greater than 5 are marked with a purple ×;
-   points with a `y` value less than −5 are marked with a green +.
-   Points between these two `y` values but still outside of the sweet
    spot are marked with a ◦.
-   Finally, points in the sweet spot (with `x` between 5 and 15 and
    with `y` between −5 and 5) are marked as a blue •.
-   Red horizontal and vertical lines delineate the sweet spot, which is
    labeled with an arrow, and there’s also a legend.

Lets begin by creating a hypothetical dataset.

``` r
(x <- 1:20)
```

    ##  [1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17
    ## [18] 18 19 20

``` r
(y <- c(-1.49,3.37,2.59,-2.78,-3.94,-0.92,6.43,8.51,3.41,-8.23,
-12.01,-6.58,2.87,14.12,9.63,-4.58,-14.78,-11.67,1.17,15.62))
```

    ##  [1]  -1.49   3.37   2.59  -2.78  -3.94  -0.92   6.43
    ##  [8]   8.51   3.41  -8.23 -12.01  -6.58   2.87  14.12
    ## [15]   9.63  -4.58 -14.78 -11.67   1.17  15.62

So now that we have the dataset ready we can start plotting. We shall
recreate the plot given below stepwise.
![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-103-1.png)

1.  Lets create an empty plotting region where lines and points can be
    added.

``` r
plot(x, y, type = "n", main = "")
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-104-1.png)

1.  The `abline` function is a simple way to add straight lines spanning
    a plot.

``` r
abline(h = c(-5, 5), col = "red", lty = 2, lwd = 2) # h adds a horizontal line at the values of y (-5 and 5), to add verticle lines you could have used v = (5,15)
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-106-1.png)

1.  Now we can add shorter line segments (and not lines spannig the
    entire plot) between the horizontal lines drawn in step 2.

``` r
segments(x0=c(5,15),y0=c(-5,-5),x1=c(5,15),y1=c(5,5),col="red",lty=3, lwd=2)
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-108-1.png)

1.  Now we can start adding points to the plot using `points()`.
    1.  `x[y>=5]` gives all the values of `x` for which the
        corresponding `y` values are `>=` 5.
    2.  `y[y>=5]` gives the subset of `y` values `>=` 5.
    3.  Both i. and ii. combine to give the coordinates in the plot.

    ``` r
    points(x[y>=5],y[y>=5],pch=4,col="darkmagenta",cex=2)
    ```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-110-1.png)

1.  Now let’s extracts the coordinates where y values are less than or
    equal to −5. A + point character is used, and you set the color to
    dark green.

``` r
points(x[y<=-5],y[y<=-5],pch=3,col="darkgreen",cex=2)
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-112-1.png)

1.  The sixth step adds the blue “sweet spot” points, which are
    identified with `(x>=5&x<=15)&(y>-5&y<5)`.

``` r
points(x[(x>=5&x<=15)&(y>-5&y<5)],y[(x>=5&x<=15)&(y>-5&y<5)],pch=19, col="blue")
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-114-1.png)

1.  This next command identifies the remaining points in the data set
    (with an x value that is either less than 5 OR greater than 15 AND a
    y value between −5 and 5). No graphical parameters are specified, so
    these points are plotted with the default black ◦.

``` r
points(x[(x<5|x>15)&(y>-5&y<5)],y[(x<5|x>15)&(y>-5&y<5)])
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-116-1.png)

1.  To draw lines connecting the coordinates in x and y, you use lines.
    Here you’ve also set lty to 4, which draws a dash-dot-dash style
    line.

``` r
lines(x,y,lty=4)
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-118-1.png)

1.  The ninth line of code adds the arrow pointing to the sweet spot.

``` r
arrows(x0=8,y0=14,x1=11,y1=2.5)
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-120-1.png)

1.  Now we shall add a text.

``` r
text(x=8,y=15,labels="sweet spot")
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-122-1.png)

1.  Finally, we can add alegend to the plot.

``` r
legend("bottomleft",
    legend=c("overall process","sweet","standard",
    "too big","too small","sweet y range","sweet x range"),
    pch=c(NA,19,1,4,3,NA,NA),lty=c(4,NA,NA,NA,NA,2,3),
    col=c("black","blue","black","darkmagenta","darkgreen","red","red"),
    lwd=c(1,NA,NA,NA,NA,2,2),pt.cex=c(NA,1,1,2,2,NA,NA),ncol = 2, cex = 0.7)
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-124-1.png)

Barplots
--------

Let’s use the `mtcars` data set to draw barplots. You can use`?mtcars`
to check the details of the data set.

``` r
mtcars[1:5,] #gives you the first five rows 
```

    ##                    mpg cyl disp  hp drat    wt  qsec vs
    ## Mazda RX4         21.0   6  160 110 3.90 2.620 16.46  0
    ## Mazda RX4 Wag     21.0   6  160 110 3.90 2.875 17.02  0
    ## Datsun 710        22.8   4  108  93 3.85 2.320 18.61  1
    ## Hornet 4 Drive    21.4   6  258 110 3.08 3.215 19.44  1
    ## Hornet Sportabout 18.7   8  360 175 3.15 3.440 17.02  0
    ##                   am gear carb
    ## Mazda RX4          1    4    4
    ## Mazda RX4 Wag      1    4    4
    ## Datsun 710         1    4    1
    ## Hornet 4 Drive     0    3    1
    ## Hornet Sportabout  0    3    2

``` r
barplot(table(mtcars$cyl))
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-125-1.png)

To make tings interesting, we can use another variable (factor) like
`am` which describes the transmission as 0 = automatic and 1 = manual.
So how many 4, 6, and 8 cylinder cars are manual or automatic?

``` r
par(mfrow = c(2,2))
cyl_matrix <- table(mtcars$am, mtcars$cyl)

barplot(cyl_matrix, legend=TRUE, main = "(A)") # gives you a stacked plot with a legend

barplot(cyl_matrix, legend.text = c("automatic", "manual"), args.legend = list(x = "top", cex = 0.6), main = "(B)")

barplot(cyl_matrix, beside = TRUE, legend.text = c("automatic", "manual"), args.legend = list(x = "top", cex = 0.75), las = 1, main = "(C)") # las=1 forces the lables on the vertical axis to appear horizontally rather than parallel to it.

barplot(cyl_matrix, col = c("red", "blue"), beside = TRUE, horiz = TRUE,legend.text = c("automatic", "manual"), args.legend = list(x = "bottomright", cex = 0.65), names.arg = c("4-Cyl", "6-Cyl", "8-Cyl"), las = 1, main="(D)")
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-126-1.png)

> **Note:** <br> You could have drawn a legend separately as done in
> case of `plot()` via `legend()`, but this way automates the color
> assignment to ensure the reference keys match the precise shading of
> the bars themselves.

Pie Chart
---------

``` r
pie(table(mtcars$cyl),labels=c("V4","V6","V8"),col=c("white","gray","black"),main="Performance cars\nby cylinders")
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-127-1.png)

> **Note** Pie charts are a very bad way of displaying information. The
> eye is good at judging linear measures and bad at judging relative
> areas. A bar chart or dot chart is a preferable way of displaying this
> type of data. Cleveland (1985), page 264: “Data that can be shown by
> pie charts always can be shown by a dot chart. This means that
> judgements of position along a common scale can be made instead of the
> less accurate angle judgements.” This statement is based on the
> empirical investigations of Cleveland and McGill as well as
> investigations by perceptual psychologists.

You can see in the following charts that `pie()` is rather fun than
science, as mentionend in the domcumentation.

``` r
par(mfrow = c(1,2))
n <- 200
pie(rep(1, n), labels = "", col = rainbow(n), border = NA)

pie(c(Sky = 85, "Sunny side of\npyramid" = 17, "Shady side of\npyramid" = 5),
    init.angle = 315, col = c("deepskyblue", "yellow", "yellow3"), border = FALSE)
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-128-1.png)

Histograms
----------

-   Barplots are really good in case of categorical variables but not
    good enough for numeric-continuous variables.
-   To draw a histogram, let’s use the `hp` horsepower in the `mtcars`
    dataset.

``` r
hist(mtcars$hp)
arrows(x0 = 280, x1 = 180, y0 = 9, y1 = 7, pch = -9658)
text(x = 285, y = 9.5, labels = "Positively Skewed")
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-129-1.png)

Let’s customise the histogram:

``` r
hist(mtcars$hp,breaks=seq(0,400,25),col="gray",main="Horsepower",xlab="HP", las = 1, ylim = c(0,9))
abline(v=c(mean(mtcars$hp),median(mtcars$hp)),lty=c(1,2),lwd=2, col= c("red", "blue"))
legend("topright",legend=c("mean HP","median HP"),lty=c(1,2),lwd=3, col= c("red", "blue"))
text(x = mean(mtcars$hp) +13, y = 8.5, col = "red", labels = round(mean(mtcars$hp)))
text(x = median(mtcars$hp) -13, y = 8.5, col = "blue", labels = round(median(mtcars$hp)))
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-130-1.png)

Box-and-Whisker plot
--------------------

Lets use the `mag` column in the `quakes` data set. Use `?quakes` to
read about the data set.

``` r
boxplot(quakes$mag)
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-131-1.png)

-   We can also create side-by-side box plots.
-   Consider the `quakes` data set.
-   The variable `mag` defines the Richter magnitude, and `stations`
    defines the number of stations reporting.

``` r
str(quakes)
```

    ## 'data.frame':    1000 obs. of  5 variables:
    ##  $ lat     : num  -20.4 -20.6 -26 -18 -20.4 ...
    ##  $ long    : num  182 181 184 182 182 ...
    ##  $ depth   : int  562 650 42 626 649 195 82 194 211 622 ...
    ##  $ mag     : num  4.8 4.2 5.4 4.1 4 4 4.8 4.4 4.7 4.3 ...
    ##  $ stations: int  41 15 43 19 11 12 43 15 35 19 ...

``` r
max(quakes$depth); min(quakes$depth)
```

    ## [1] 680

    ## [1] 40

``` r
depth_cut <- cut(quakes$stations, breaks = c(0, 50,  100, 150, 200), right = FALSE)
head(depth_cut)
```

    ## [1] [0,50) [0,50) [0,50) [0,50) [0,50) [0,50)
    ## Levels: [0,50) [50,100) [100,150) [150,200)

-   So the depth have been put in threee groups.
-   Now we are interested to know **how the magnitue is correlated to
    the depth of an earthquake**.

``` r
boxplot(quakes$mag ~ depth_cut, xlab = "Depth (in km)", ylab = "Magnitude", col = "grey")
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-133-1.png)

-   We can see the **the more the depth of an earthquake, the greater is
    the magnitude**.

Scatterplots
------------

-   We will work with the `iris` data set.
-   Collected in the mid- 1930s, this data frame of 150 rows and 5
    columns consists of petal and sepal measurements for three species
    of perennial iris flowers—*Iris setosa*, *Iris virginica*, and *Iris
    versicolor* (Anderson, 1935; Fisher, 1936).
-   Lets see the frequency distribution of these different species of
    flowers.

``` r
head(iris)
```

    ##   Sepal.Length Sepal.Width Petal.Length Petal.Width
    ## 1          5.1         3.5          1.4         0.2
    ## 2          4.9         3.0          1.4         0.2
    ## 3          4.7         3.2          1.3         0.2
    ## 4          4.6         3.1          1.5         0.2
    ## 5          5.0         3.6          1.4         0.2
    ## 6          5.4         3.9          1.7         0.4
    ##   Species
    ## 1  setosa
    ## 2  setosa
    ## 3  setosa
    ## 4  setosa
    ## 5  setosa
    ## 6  setosa

``` r
table(iris$Species)
```

    ## 
    ##     setosa versicolor  virginica 
    ##         50         50         50

-   Lets see a simple plot of petal length and width (see fig (A)).

> We see that **longer petals also wider**.

-   But, we do not know how they vary with species.

> Similarly, **virginica** has the longest and widest petals.

``` r
par(mfrow = c(1,2))

plot(iris[,4],iris[,3],xlab="Petal Width (cm)", ylab="Petal Length (cm)", las = 1, main = "(A)")

plot(iris[,4],iris[,3],type="n",xlab="Petal Width (cm)", ylab="Petal Length (cm)", las = 1, main = "(B)")
points(iris[iris$Species=="setosa",4],iris[iris$Species=="setosa",3],pch=19,col="green")
points(iris[iris$Species=="virginica",4],iris[iris$Species=="virginica",3],pch=19,col="blue")
points(iris[iris$Species=="versicolor",4],iris[iris$Species=="versicolor",3],pch=19,col="red")
legend("topleft",legend=c("setosa","virginica","versicolor"), col=c("green","blue","red"),pch=c(19,19,19), cex = 0.8)
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-135-1.png)

-   You can generate the same image more simply by first setting up
    vectors that specify the desired point character and color for each
    individual observation.

``` r
# Create pch for iris, 
iris_pch <- rep(19, nrow(iris))

# Overwrite and change the pch for setosa species = 1, where 1 is the pch
iris_pch[iris$Species == "setosa"] <- 1

# You can also have a diferent pch for virginica = 3
iris_pch[iris$Species == "virginica"] <- 3

# Now we can set the colors, starting with any default col
iris_col <- rep("red", times = nrow(iris))

# Lets set the col for setosa and virginica as green and blue
iris_col[iris$Species == "setosa"] <- "green"
iris_col[iris$Species == "virginica"] <- "blue"

# Now, `iris_pch` and `iris_col` now can be used as the defined pch and col
# Lets plot:
plot(iris[,4], iris[,3], pch = iris_pch, col = iris_col, xlab="Petal Width (cm)", ylab="Petal Length (cm)", las = 1)
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-136-1.png)

-   This **vectorised operation** as done above has made it easier to
    create a **matrix of plots**:

``` r
# This is the default plot without any custoimisation.
plot(iris, main = "Default Plot\nNo Customisation")
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-137-1.png)

``` r
# This is the plot that you create with the customised pch and col
plot(iris, pch = iris_pch, col = iris_col, main = "Customised Plot")
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-137-2.png)

``` r
# You can also do this for a select number of variables
plot(iris[,2:4],pch = iris_pch, col = iris_col, main = "Customised Plot\nFor Three Variables Only" )
```

![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-137-3.png)

More on data frames:
====================

Finding missing values i.e. **NA**s or **NaN**s in dataset objects.
-------------------------------------------------------------------

Example:

``` r
x <- c(1,2,NA,4,5,6)
is.na(x)
```

    ## [1] FALSE FALSE  TRUE FALSE FALSE FALSE

``` r
is.nan(x)
```

    ## [1] FALSE FALSE FALSE FALSE FALSE FALSE

-   A NaN is also NA but the converse is not true.

``` r
x<- c(1,2,NA, NaN, 5,6)
is.na(x)
```

    ## [1] FALSE FALSE  TRUE  TRUE FALSE FALSE

``` r
is.nan(x)
```

    ## [1] FALSE FALSE FALSE  TRUE FALSE FALSE

-   Removing NAs

``` r
x <- c(12, 56, 78, NA, 55, NA, NA, 78)
yes.na <- is.na(x)
x[!yes.na]
```

    ## [1] 12 56 78 55 78

``` r
# or
no.na <- !yes.na
x[no.na]
```

    ## [1] 12 56 78 55 78

``` r
# or

DF <- data.frame(x = c(1, 2, 3), y = c(0, 10, NA))
na.omit(DF)
```

    ##   x  y
    ## 1 1  0
    ## 2 2 10

The `apply()` function
----------------------

-   Applying a function to each element of an object

``` r
x <- 1:20
dim(x) <- c(5,4)
colnames(x) <- c("a", "b", "c", "d")
apply(x, MARGIN=1, sum) #sums over the rows of the matrix x 
```

    ## [1] 34 38 42 46 50

``` r
apply(x, MARGIN=2, mean)
```

    ##  a  b  c  d 
    ##  3  8 13 18

The `tapply()` function.
------------------------

-   The tapply function is useful when we need to break up a vector into
    groups defined by some classifying factor, compute a function on the
    subsets, and return the results in a convenient form. You can even
    specify multiple factors as the grouping variable, for example
    treatment and gender, or team and handedness.
-   Lets say we have two vectors

``` r
students <- factor(c("a","b", "c", "d", "e", "a","b", "c", "d", "e","a","b", "c", "d","a","b", "c", "a", "b", "c"))
levels(students); length(students)
```

    ## [1] "a" "b" "c" "d" "e"

    ## [1] 20

``` r
marks <- c(12, 10, 15,16,12,18,19,13,15,14,1,12,18,20,21,15,16, 12, 14, 15)
length(marks)
```

    ## [1] 20

-   We now want to calculate the mean of a, b, c,d and e

``` r
(mean.mar.stu <- tapply(X = marks, INDEX = students, FUN = mean))
```

    ##    a    b    c    d    e 
    ## 12.8 14.0 15.4 17.0 13.0

``` r
(mean.mar.stu <- tapply(X = marks, INDEX = marks, FUN = length)) # this is like creating a frequency distribution.
```

    ##  1 10 12 13 14 15 16 18 19 20 21 
    ##  1  1  4  1  2  4  2  2  1  1  1

``` r
(mean.mar.stu <- tapply(X = students, INDEX = students, FUN = length))
```

    ## a b c d e 
    ## 5 5 5 3 2

-   another example: using the `iris` dataset from the base R (we have
    used this data set before).

``` r
str(iris)
```

    ## 'data.frame':    150 obs. of  5 variables:
    ##  $ Sepal.Length: num  5.1 4.9 4.7 4.6 5 5.4 4.6 5 4.4 4.9 ...
    ##  $ Sepal.Width : num  3.5 3 3.2 3.1 3.6 3.9 3.4 3.4 2.9 3.1 ...
    ##  $ Petal.Length: num  1.4 1.4 1.3 1.5 1.4 1.7 1.4 1.5 1.4 1.5 ...
    ##  $ Petal.Width : num  0.2 0.2 0.2 0.2 0.2 0.4 0.3 0.2 0.2 0.1 ...
    ##  $ Species     : Factor w/ 3 levels "setosa","versicolor",..: 1 1 1 1 1 1 1 1 1 1 ...

``` r
tapply(iris$Sepal.Length, iris$Species, mean)
```

    ##     setosa versicolor  virginica 
    ##      5.006      5.936      6.588

The `lapply()` function:
------------------------

-   Applying a function to a list or vector

``` r
(x <- as.list(1:5))
```

    ## [[1]]
    ## [1] 1
    ## 
    ## [[2]]
    ## [1] 2
    ## 
    ## [[3]]
    ## [1] 3
    ## 
    ## [[4]]
    ## [1] 4
    ## 
    ## [[5]]
    ## [1] 5

``` r
lapply(x, FUN = sqrt)
```

    ## [[1]]
    ## [1] 1
    ## 
    ## [[2]]
    ## [1] 1.414214
    ## 
    ## [[3]]
    ## [1] 1.732051
    ## 
    ## [[4]]
    ## [1] 2
    ## 
    ## [[5]]
    ## [1] 2.236068

``` r
(d <- data.frame(x = 1:5, y = 6:10))
```

    ##   x  y
    ## 1 1  6
    ## 2 2  7
    ## 3 3  8
    ## 4 4  9
    ## 5 5 10

``` r
lapply(d, FUN = sqrt)
```

    ## $x
    ## [1] 1.000000 1.414214 1.732051 2.000000 2.236068
    ## 
    ## $y
    ## [1] 2.449490 2.645751 2.828427 3.000000 3.162278

``` r
lapply(d, FUN = max)
```

    ## $x
    ## [1] 5
    ## 
    ## $y
    ## [1] 10

The `sapply()` function
-----------------------

-   When you want to to get the output as a vector, matrix, or array
    instead of a list

``` r
sapply(x, FUN = sqrt)
```

    ## [1] 1.000000 1.414214 1.732051 2.000000 2.236068

``` r
sapply(d, FUN = sqrt)
```

    ##             x        y
    ## [1,] 1.000000 2.449490
    ## [2,] 1.414214 2.645751
    ## [3,] 1.732051 2.828427
    ## [4,] 2.000000 3.000000
    ## [5,] 2.236068 3.162278

Reading in external data files
==============================

the table format
----------------

-   Typically, these files have a .txt extension (highlighting the
    plain-text style) or .csv (for comma-separated values).
-   One key feature is that it usually has a header.
-   Delimiter is a character used to seperate enteries in each line.
-   Missing value or NA is used to denote a missing value.

``` r
(mydatafile <- read.table(file = "C:/Users/pravesh/Google Drive/Copy/R/Lecture Basics of R/8.2.1_mydatafile.txt",
                         header = T, sep = " ", na.strings = "*", stringsAsFactors = F))
```

    ##   person age sex funny age.mon
    ## 1  Peter  NA   M  High     504
    ## 2   Lois  40   F  <NA>     480
    ## 3    Meg  17   F   Low     204
    ## 4  Chris  14   M   Med     168
    ## 5 Stewie   1   M  High      NA
    ## 6  Brian  NA   M   Med      NA

-   Another alternative way of selecting the file is using the
    `file.choose()` command

``` r
mydatafile <- read.table(file = file.choose(), header = T, sep = " ", na.strings = "*", stringsAsFactors = F)
```

Spreadsheet workbooks
---------------------

-   Using the `read.csv()` function.

``` r
(dat <- read.csv(file = "C:/Users/pravesh/Google Drive/Copy/R/Lecture Basics of R/8.2.1_mydatafile.csv", header = FALSE,
         stringsAsFactors = TRUE))
```

    ##   V1  V2      V3
    ## 1 75 161 female 
    ## 2 89 185   male 
    ## 3 75 185 female 
    ## 4 42 132   male 
    ## 5 93 170 female 
    ## 6 63 185 female 
    ## 7 58 132   male

-   Using the `read_excel()` function in the Environment window.

Writing out data files
----------------------

-   The function for writing out table format files to your computer is
    `write.table()`.

``` r
write.table(dat, file = "C:/Users/pravesh/Google Drive/Copy/R/Lecture Basics of R/data.csv", sep=",")
```

writing out plots and graphic files
-----------------------------------

-   Use `?png` for details.

``` r
png(filename = "C:/Users/pravesh/Google Drive/Copy/R/Lecture Basics of R/p.png")
plot(iris); dev.off()
```

    ## png 
    ##   2

``` r
jpeg(filename = "C:/Users/pravesh/Google Drive/Copy/R/Lecture Basics of R/p1.jpeg")
plot(mtcars$hp); dev.off()
```

    ## png 
    ##   2

-   The default unit is pixels which can be changed to *cm* or *mm* as
    follows

``` r
jpeg(filename = "C:/Users/pravesh/Google Drive/Copy/R/Lecture Basics of R/myplot.jpeg", height = 6, width = 6, 
     units = "cm", res = 200)
x <- 1:20; y <- 21:40; plot(x,y); dev.off()
```

-   When you have finished plotting, the file deveice must be closed
    with a `dev.off()` call. If `dev.off()` is not called R shall
    continue printing all the subsequent plotting commands to the file
    and overwrite it.

printing in a pdf format
------------------------

``` r
pdf(file = "C:/Users/pravesh/Google Drive/Copy/R/Lecture Basics of R/myplot.pdf", height = 6, width = 6)
x <- 1:20; y <- 21:40; plot(x,y); dev.off()
```

    ## png 
    ##   2

Practice
========

1.  Create a vector **x** and assign a numerical value to it.
2.  Create another vector **y** and assign the numbers 1 to 5.
3.  Creater a longer vector that contains numbers 1 to 5 ten times.
4.  Assign some meaningful names to the following vectors:
    -   `c(2, 4, 6, 8, 10, 12, 14, 16, 20)`
    -   `0`
    -   `3.141593`
    -   `c(1, 10, 100, 1000, 10000, 100000)`
5.  Create vectors that correspond to the following variables names:
    -   BMI
    -   Age
    -   daysPerMonth
    -   firstFivePrimeNumbers
6.  Create three vectors that each contain just 1 element with variable
    names `p`, `q`, and `r`, and values 1, 2, and 3. Then, create a new
    vector that contains multiple elements, using the scalars we just
    created i.e., create a vector `u` of length 3, with the subsequent
    elements of `p`, `q` and `r`.
7.  Create a new vector u with length 96 that contains the elements of u
    as follows: 1, 2, 3, 1, 2, 3, …., 1, 2, 3.
8.  Suppose the surface area of a circle equals 25, what is the radius?
9.  What is the probability density at *x=0* of a normally distributed
    random variable *x* with mean (mu) equal to zero, and standard
    devation (sigma) equal to one?
10. Sort the numbers 10,50,12,63,74,1,89,5,3,6,4 in ascending order.
11. Generate a sequence of 100 numbers between -60 to 45 with a width of
    5, and find the mean value.
12. Use the functions `mean()` and `range()` to find the mean and range
    of:
    -   the numbers 1, 2, . . . , 21
    -   the sample of 50 random normal values, that can be generated
        from a normaL distribution with mean 0 and variance 1 using the
        assignment `y <- rnorm(50)`.
    -   the columns **height** and **weight** in the data frame
        **women**. \[The datasets package that has this data frame is by
        default attached when R is started.\]
13. What are the respective effects of the arguments `sep` and
    `collapse` in the `paste()` function?
14. Create a matrix as depicted in the following table. The row names
    are the roll numbers of the students in economics class, and the
    column names are the codes of the courses. The values represent the
    marks obtained out of 50, and are random. You can assume and assign
    marks.

<div style="border: 1px solid #ddd; padding: 0px; overflow-y: scroll; height:250px; ">
<table class="table table-striped table-hover" style="width: auto !important; margin-left: auto; margin-right: auto;">
<thead>
<tr>
<th style="text-align:left;position: sticky; top:0; background-color: #FFFFFF;">
Subject
</th>
<th style="text-align:right;position: sticky; top:0; background-color: #FFFFFF;">
ECON0101
</th>
<th style="text-align:right;position: sticky; top:0; background-color: #FFFFFF;">
ECON0102
</th>
<th style="text-align:right;position: sticky; top:0; background-color: #FFFFFF;">
ECON0201
</th>
<th style="text-align:right;position: sticky; top:0; background-color: #FFFFFF;">
ECON0791
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
ECON01
</td>
<td style="text-align:right;">
31
</td>
<td style="text-align:right;">
22
</td>
<td style="text-align:right;">
20
</td>
<td style="text-align:right;">
22
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON02
</td>
<td style="text-align:right;">
24
</td>
<td style="text-align:right;">
32
</td>
<td style="text-align:right;">
26
</td>
<td style="text-align:right;">
41
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON03
</td>
<td style="text-align:right;">
37
</td>
<td style="text-align:right;">
29
</td>
<td style="text-align:right;">
22
</td>
<td style="text-align:right;">
41
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON04
</td>
<td style="text-align:right;">
35
</td>
<td style="text-align:right;">
23
</td>
<td style="text-align:right;">
48
</td>
<td style="text-align:right;">
37
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON05
</td>
<td style="text-align:right;">
38
</td>
<td style="text-align:right;">
23
</td>
<td style="text-align:right;">
30
</td>
<td style="text-align:right;">
21
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON06
</td>
<td style="text-align:right;">
20
</td>
<td style="text-align:right;">
23
</td>
<td style="text-align:right;">
21
</td>
<td style="text-align:right;">
22
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON07
</td>
<td style="text-align:right;">
33
</td>
<td style="text-align:right;">
41
</td>
<td style="text-align:right;">
41
</td>
<td style="text-align:right;">
37
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON08
</td>
<td style="text-align:right;">
47
</td>
<td style="text-align:right;">
38
</td>
<td style="text-align:right;">
40
</td>
<td style="text-align:right;">
45
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON09
</td>
<td style="text-align:right;">
23
</td>
<td style="text-align:right;">
42
</td>
<td style="text-align:right;">
46
</td>
<td style="text-align:right;">
40
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON10
</td>
<td style="text-align:right;">
39
</td>
<td style="text-align:right;">
37
</td>
<td style="text-align:right;">
41
</td>
<td style="text-align:right;">
39
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON11
</td>
<td style="text-align:right;">
39
</td>
<td style="text-align:right;">
38
</td>
<td style="text-align:right;">
24
</td>
<td style="text-align:right;">
43
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON12
</td>
<td style="text-align:right;">
46
</td>
<td style="text-align:right;">
43
</td>
<td style="text-align:right;">
40
</td>
<td style="text-align:right;">
29
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON13
</td>
<td style="text-align:right;">
43
</td>
<td style="text-align:right;">
44
</td>
<td style="text-align:right;">
43
</td>
<td style="text-align:right;">
31
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON14
</td>
<td style="text-align:right;">
29
</td>
<td style="text-align:right;">
35
</td>
<td style="text-align:right;">
50
</td>
<td style="text-align:right;">
21
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON15
</td>
<td style="text-align:right;">
41
</td>
<td style="text-align:right;">
32
</td>
<td style="text-align:right;">
38
</td>
<td style="text-align:right;">
47
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON16
</td>
<td style="text-align:right;">
21
</td>
<td style="text-align:right;">
33
</td>
<td style="text-align:right;">
41
</td>
<td style="text-align:right;">
31
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON17
</td>
<td style="text-align:right;">
28
</td>
<td style="text-align:right;">
33
</td>
<td style="text-align:right;">
41
</td>
<td style="text-align:right;">
24
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON18
</td>
<td style="text-align:right;">
33
</td>
<td style="text-align:right;">
23
</td>
<td style="text-align:right;">
42
</td>
<td style="text-align:right;">
28
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON19
</td>
<td style="text-align:right;">
25
</td>
<td style="text-align:right;">
30
</td>
<td style="text-align:right;">
49
</td>
<td style="text-align:right;">
45
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON20
</td>
<td style="text-align:right;">
21
</td>
<td style="text-align:right;">
37
</td>
<td style="text-align:right;">
20
</td>
<td style="text-align:right;">
50
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON21
</td>
<td style="text-align:right;">
28
</td>
<td style="text-align:right;">
43
</td>
<td style="text-align:right;">
33
</td>
<td style="text-align:right;">
34
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON22
</td>
<td style="text-align:right;">
50
</td>
<td style="text-align:right;">
31
</td>
<td style="text-align:right;">
31
</td>
<td style="text-align:right;">
21
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON23
</td>
<td style="text-align:right;">
38
</td>
<td style="text-align:right;">
42
</td>
<td style="text-align:right;">
42
</td>
<td style="text-align:right;">
35
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON24
</td>
<td style="text-align:right;">
28
</td>
<td style="text-align:right;">
28
</td>
<td style="text-align:right;">
28
</td>
<td style="text-align:right;">
30
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON25
</td>
<td style="text-align:right;">
31
</td>
<td style="text-align:right;">
39
</td>
<td style="text-align:right;">
20
</td>
<td style="text-align:right;">
29
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON26
</td>
<td style="text-align:right;">
26
</td>
<td style="text-align:right;">
50
</td>
<td style="text-align:right;">
23
</td>
<td style="text-align:right;">
49
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON27
</td>
<td style="text-align:right;">
41
</td>
<td style="text-align:right;">
26
</td>
<td style="text-align:right;">
47
</td>
<td style="text-align:right;">
40
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON28
</td>
<td style="text-align:right;">
22
</td>
<td style="text-align:right;">
26
</td>
<td style="text-align:right;">
47
</td>
<td style="text-align:right;">
29
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON29
</td>
<td style="text-align:right;">
42
</td>
<td style="text-align:right;">
46
</td>
<td style="text-align:right;">
40
</td>
<td style="text-align:right;">
42
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON30
</td>
<td style="text-align:right;">
25
</td>
<td style="text-align:right;">
40
</td>
<td style="text-align:right;">
30
</td>
<td style="text-align:right;">
39
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON31
</td>
<td style="text-align:right;">
45
</td>
<td style="text-align:right;">
49
</td>
<td style="text-align:right;">
22
</td>
<td style="text-align:right;">
25
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON32
</td>
<td style="text-align:right;">
27
</td>
<td style="text-align:right;">
45
</td>
<td style="text-align:right;">
50
</td>
<td style="text-align:right;">
48
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON33
</td>
<td style="text-align:right;">
35
</td>
<td style="text-align:right;">
48
</td>
<td style="text-align:right;">
44
</td>
<td style="text-align:right;">
31
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON34
</td>
<td style="text-align:right;">
37
</td>
<td style="text-align:right;">
44
</td>
<td style="text-align:right;">
35
</td>
<td style="text-align:right;">
46
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON35
</td>
<td style="text-align:right;">
41
</td>
<td style="text-align:right;">
45
</td>
<td style="text-align:right;">
36
</td>
<td style="text-align:right;">
31
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON36
</td>
<td style="text-align:right;">
34
</td>
<td style="text-align:right;">
43
</td>
<td style="text-align:right;">
43
</td>
<td style="text-align:right;">
23
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON37
</td>
<td style="text-align:right;">
38
</td>
<td style="text-align:right;">
42
</td>
<td style="text-align:right;">
34
</td>
<td style="text-align:right;">
41
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON38
</td>
<td style="text-align:right;">
34
</td>
<td style="text-align:right;">
33
</td>
<td style="text-align:right;">
32
</td>
<td style="text-align:right;">
20
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON39
</td>
<td style="text-align:right;">
24
</td>
<td style="text-align:right;">
44
</td>
<td style="text-align:right;">
37
</td>
<td style="text-align:right;">
45
</td>
</tr>
<tr>
<td style="text-align:left;">
ECON40
</td>
<td style="text-align:right;">
24
</td>
<td style="text-align:right;">
37
</td>
<td style="text-align:right;">
39
</td>
<td style="text-align:right;">
41
</td>
</tr>
</tbody>
</table>
</div>

1.  Calculate the mean marks obtained by each student in Q14 and find
    out which students got the top and last 3 positions (hint: you can
    sort the data).
2.  What date and time shall your friend in Massachusetts Institute of
    Technology (MIT) be speaking with you online if you call him/her
    now?
3.  Create a 4X3 matrix with numbers between -30 and 30 (excluding 0).
    Extract the first and second elements from the fourth row. Extract
    the second and third elements from the second row. Replace all the
    negative elements in the matrix with 0.
4.  Extract all clips starting with either `http` or `https` from this
    vector

``` r
(c("www.dogman.com", "http://rotterdam.com", "https://facebook.com", "httpx://sims.com"))
```

1.  Extract the street address from: **Presidency University, 86/1,
    College Street, Kolkata - 700073.**
2.  Remove all the non-alphabetical characters from the following
    paragraph and add your name at the end;

> I think, sometimes, that my use of commas, and, occasionally,
> exclamation marks, can be excessive. Whenever I add a word or
> expression, not necessary, to the sentence, just like I did with the
> “not necessary” and like am doing right now, I always include these
> words, well maybe not always, usually include these inserts between
> commas; so, basically, I enjoy writing long sentences, joined with
> lots of commas and, frequently, semi-colons and, often, colons (and
> have been rather prone to using brackets, as well).

I am posting the solution to this question as you shall require another
package called `mgsub`. Do let me know if you have any queries.

``` r
## install.packages("mgsub")
library(mgsub)
k <- 'I think, sometimes, that my use of commas, and, occasionally, exclamation marks, can be excessive. Whenever I add a word or expression, not necessary, to the sentence, just like I did with the "not necessary" and like am doing right now, I always include these words, well maybe not always, usually include these inserts between commas; so, basically, I enjoy writing long sentences, joined with lots of commas and, frequently, semi-colons and, often, colons (and have been rather prone to using brackets, as well).'

p <- mgsub(pattern = c("\\,", "\\(", "\"", "\\.", "\\)", "\\;"), replacement = rep("", times = 6), k)
paste(p, "My Name", sep = " --- ")
```

    ## [1] "I think sometimes that my use of commas and occasionally exclamation marks can be excessive Whenever I add a word or expression not necessary to the sentence just like I did with the not necessary and like am doing right now I always include these words well maybe not always usually include these inserts between commas so basically I enjoy writing long sentences joined with lots of commas and frequently semi-colons and often colons and have been rather prone to using brackets as well --- My Name"

1.  Create an ordered vector as represented in the following table, and
    replicate the output table:
    <table class="table table-striped" style="width: auto !important; ">
    <thead>
    <tr>
    <th style="text-align:right;">
    Slow
    </th>
    <th style="text-align:right;">
    Fast
    </th>
    <th style="text-align:right;">
    Insane
    </th>
    </tr>
    </thead>
    <tbody>
    <tr>
    <td style="text-align:right;">
    5
    </td>
    <td style="text-align:right;">
    6
    </td>
    <td style="text-align:right;">
    3
    </td>
    </tr>
    </tbody>
    </table>
2.  1.  Construct and store a 4 x 2 matrix that’s filled row-wise with
        the values 4.3, 3.1, 8.2, 8.2, 3.2, 0.9, 1.6, and 6.5, in that
        order.
    2.  Confirm the dimensions of the matrix from (a) are 3 x 2 if you
        remove any one row.
    3.  Overwrite the second column of the matrix from (a) with that
        same column sorted from smallest to largest.
    4.  What does R return if you delete the fourth row and the first
        column from (c)? Use matrix to ensure the result is a
        single-column matrix, rather than a vector.
    5.  Store the bottom four elements of (c) as a new 2 x 2 matrix.
    6.  Overwrite, in this order, the elements of (c) at positions
        (4;2), (1;2), (4;1), and (1;1) with $-\\frac{1}{2}$ of the two
        values on the diagonal of (e).

3.  1.  Calculate the following:
        $$\\frac{2}{7}\\left( 
        \\begin{bmatrix}
        1 & 2 \\\\
        2 & 4\\\\
        7 & 6 \\\\ 
        \\end{bmatrix} - \\begin{bmatrix}
        10 & 20 \\\\
        30 & 40\\\\
        50 & 60 \\\\ 
        \\end{bmatrix}\\right)$$
    2.  Store these two matrices:
        $$ A = \\begin{bmatrix}
        1\\\\2\\\\7
        \\end{bmatrix}  B = \\begin{bmatrix}
        3\\\\4\\\\8
        \\end{bmatrix} 
        $$
        Which of the following multiplications are possible?
        1.  *A*.*B*
        2.  *A*<sup>⊺</sup>.*B*
        3.  *B*<sup>⊺</sup>.(*A*.*A*<sup>⊺</sup>)
        4.  (*A*.*A*<sup>⊺</sup>).*B*<sup>⊺</sup>
        5.  \[(*B*.*B*<sup>⊺</sup>)+(*A*.*A*<sup>⊺</sup>)−100*I*<sub>3</sub>\]<sup> − 1</sup>

4.  1.  Store the vector `c(7,1,7,10,5,9,10,3,10,8)` as `nums`. Print
        the elements greater than 5 OR equal to 2.

    2.  Store the vector `c(8,8,4,4,5,1,5,6,6,8)` and print the elements
        less than or equal to 6 AND not equal to 4.

5.  Re-create exactly the following output:

<!-- -->

    ## The quick brown fox
    ##   jumped over
    ##       the lazy dogs

1.  Suppose you’ve stored the values `num1 <- 4` and `num2 <- 0.75`.
    Write a line of R code that returns the following string:

<!-- -->

    ## [1] "The result of multiplying 4 by 0.75 is 3"

1.  On my local machine, the directory for my work on this book is
    specified in R as **“/Users/ptamang/Documents/RBook/”**. Imagine it
    is your machine - write a line of code that replaces **ptamang** in
    this string with your first initial and surname.
2.  Store the following string **“How much wood could a woodchuck
    chuck”** and glue it to **“if a woodchuck could chuck wood.”** Next
    replace all instances of **wood** with **metal** in the resulting
    string.
3.  The Indian government consists of the political parties **BJP**,
    **INC**, **CPI**, **TMC** and other parties grouped under **Others**
    category. Suppose you asked 20 Indians which of these they
    identified most with and obtained the following data:
    -   There were 12 males and 8 females; the individuals nnumbered 1,
        5-7, 12, and 14-16 were females.
    -   The individuals numbered 1,4,12,15,16 and 19 identified with
        BJP; no one identified with CPI, the individuals numbered 6,9
        and 11 identified with INC, 10 and 20 identified with Others,
        and the rest with TMC.

    1.  Use your knowledge of vectors (for example, subsetting and
        overwriting) to create two character vectors: **sex** with
        entries “M” (male) and “F” (female) and **party** with entries
        “BJP”, “INC”, “CPI”, “TMC”, and “Others”. Make sure the entries
        are placed in the correct positions as outlined earlier.

<!-- -->

1.  Create two different factor vectors based on **sex** and **party**.
    Does it make any sense to use `ordered=TRUE` in either case? How has
    R appeared to arrange the levels?

2.  Use factor subsetting to do the following:

    1.  Return the factor vector of chosen parties for only the male
        participants.
    2.  Return the factor vector of genders for those who chose BJP.

3.  Another six people joined the survey, with the results
    **c(“BJP”,“INC”,“INC”,“CPM”,“TMC”,“BJP”)** for the preferred party
    and **c(“M”,“M”,“F”,“F”,“F”,“M”)** as their gender. Combine these
    results with the original factors from (b).

Suppose you also asked all individuals to state how confident they were
that BJP will win more seats in West Bengal than TMC in the next
election and to attach a subjective percentage to that confidence. The
following 26 results were obtained: 93, 55, 29, 100, 52, 84, 56, 0, 33,
52, 35, 53, 55, 46, 40, 40, 56, 45, 64, 31, 10, 29, 40, 95, 18, 61. e.
Create a factor with levels of confidence as follows: Low for
percentages \[0,30\]; Moderate for percentages (30,70\]; and High for
percentages (70,100\].

1.  From (e), extract the levels corresponding to those individuals who
    originally said they identified with BJP. Do this also for TMC. What
    do you notice?

<!-- -->

1.  1.  Create a list that contains, in this order, a sequence of 20
        evenly spaced numbers between -4 and 4; a 3 x 3 matrix of the
        logical vector c(F,T,T,T,F,T,T,F,F) filled column-wise; a
        character vector with the two strings “don” and “quixote”; and a
        factor vector containing the observations
        c(“LOW”,“MED”,“LOW”,“MED”,“MED”,“HIGH”). Then, do the following:
        1.  Extract row elements 2 and 1 of columns 2 and 3, in that
            order, of the logical matrix.
        2.  Obtain all values from the sequence between -4 and 4 that
            are greater than 1.
        3.  Using `which()` determine which indices in the factor vector
            are assigned the “MED” level.

2.  1.  Create and store this data frame as **dframe** in your R
        workspace:
        <table class="table table-striped table-hover" style="width: auto !important; ">
        <thead>
        <tr>
        <th style="text-align:left;">
        person
        </th>
        <th style="text-align:left;">
        gender
        </th>
        <th style="text-align:left;">
        funny
        </th>
        </tr>
        </thead>
        <tbody>
        <tr>
        <td style="text-align:left;">
        Bumrah
        </td>
        <td style="text-align:left;">
        M
        </td>
        <td style="text-align:left;">
        High
        </td>
        </tr>
        <tr>
        <td style="text-align:left;">
        Kom
        </td>
        <td style="text-align:left;">
        F
        </td>
        <td style="text-align:left;">
        Med
        </td>
        </tr>
        <tr>
        <td style="text-align:left;">
        Phogat
        </td>
        <td style="text-align:left;">
        M
        </td>
        <td style="text-align:left;">
        Low
        </td>
        </tr>
        <tr>
        <td style="text-align:left;">
        Bhutia
        </td>
        <td style="text-align:left;">
        M
        </td>
        <td style="text-align:left;">
        High
        </td>
        </tr>
        <tr>
        <td style="text-align:left;">
        Sindhu
        </td>
        <td style="text-align:left;">
        F
        </td>
        <td style="text-align:left;">
        Med
        </td>
        </tr>
        <tr>
        <td style="text-align:left;">
        Khan
        </td>
        <td style="text-align:left;">
        F
        </td>
        <td style="text-align:left;">
        Med
        </td>
        </tr>
        </tbody>
        </table>
        The variables **person**, **gender**, and **funny** should be of
        character, factor (with levels **F** and **M**), and factor
        (with levels **Low**, **Med**, and **High**) respectively.
        1.  Create another dataframe contatining information on 4 more
            people. Append this data frame to the one you created in
            (a).
        2.  Add a new column (name it **age**) containing information on
            age to the appended data frame in (b).
        3.  Reorder the column variables of the data frame in (c) such
            that the **age** column is after the **gender** column.
        4.  Use your knowledge of handling character strings and write a
            single line of code that will extract from the reordered
            data frame in (d), all the records of persons whose name
            starts with **B**. For example if you were to do the same
            with **dframe**, the oputput shoud look exactly as given
            below:
            <table class="table table-striped table-hover" style="width: auto !important; ">
            <thead>
            <tr>
            <th style="text-align:left;">
            </th>
            <th style="text-align:left;">
            person
            </th>
            <th style="text-align:left;">
            gender
            </th>
            <th style="text-align:left;">
            funny
            </th>
            </tr>
            </thead>
            <tbody>
            <tr>
            <td style="text-align:left;">
            1
            </td>
            <td style="text-align:left;">
            Bumrah
            </td>
            <td style="text-align:left;">
            M
            </td>
            <td style="text-align:left;">
            High
            </td>
            </tr>
            <tr>
            <td style="text-align:left;">
            4
            </td>
            <td style="text-align:left;">
            Bhutia
            </td>
            <td style="text-align:left;">
            M
            </td>
            <td style="text-align:left;">
            High
            </td>
            </tr>
            </tbody>
            </table>

3.  Store the following matrix
    $$\\begin{bmatrix}
    34 & 0 & 1\\\\
    23 & 1 &2 \\\\
    33 & 1& 1\\\\
    42 & 0 & 1 \\\\
    41 & 0 & 2
    \\end{bmatrix}$$
    Then do the following:

    1.  Coerce the matrix to a data frame.
    2.  As a data frame, coerce the second column to be logical valued.
    3.  As as data frame, coerce the third column to be factor valued.

4.  Use the code given below to download the United States real GDP
    rates from 1929.
    `t <- htmltab("https://www.thebalance.com/us-gdp-by-year-3305543", 1)`
    The table is stored in `t`. you can check the class of `t` and
    confirm that its a data frame. You can additionally visit the
    website to know more about the data structure.

    1.  Install `htmltab` package and load it in the current session.
    2.  All you need to do is to find the average the real gdp growth
        during 1950 - 1964.
    3.  You can plot the growth rates since the period 1929.

5.  As closely as you can, recreate the following plot:
    ![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-172-1.png)

6.  Use the `quakes` data set and the `mag` column to create the
    following boxplot: Use `?quakes` to read the description of the data
    set. You can use the `shape` package if you want to.
    ![](basicsofR2019_files/figure-markdown_github/unnamed-chunk-173-1.png)

7.  Us the built-in `InsectSprays` data frame, containing counts of
    insects on various agricultural units treated with one of six
    sprays:

    1.  Produce a histogram of the counts of insects using base R
        graphics.
    2.  Obtain the total number of insects found according to each
        spray. Then produce a vertical barplot and pie chart of these
        totals, labeling each plot appropriately.
    3.  Generate side-by-side boxplots of the counts of insects
        according to each spray type and include appropriate axis labels
        and a title.

8.  Yet another of R’s useful ready-to-use data sets is `USArrests`,
    containing data on the number of arrests for murder, rape, and
    assault per 100,000 individuals in each of the 50 states of the
    United States, recorded in 1973 (see, for example, McNeil, 1977). It
    also includes a variable giving the percentage of urban-based
    population in each state. Briefly inspect the data frame object and
    the accompanying documentation `?USArrests`. Then complete the
    following:

    1.  Generate a histogram of the proportion of urban population for
        the states. Set your breaks to be 10 units each, between 0
        and 100. Have the histogram show the first quartile, the median,
        and the third quartile; then provide a matching legend. Use
        colors as you like and include appropriate axis annotation.
    2.  The code `t(as.matrix(USArrests[,-3]))` creates a matrix of the
        `USArrests` data without the urban population column, and the
        built-in R object `state.abb` provides the two-letter state
        abbreviations, in alphabetical order, as a character vector. Use
        these two structures and base R graphics to produce a
        horizontal, stacked barplot with the horizontal bars labeled
        with state abbreviations and with each bar split according to
        the type of crime (murder, rape, and assault). Include a legend.
    3.  Define a new factor vector `urbancat` that is set to 1 if the
        corresponding state has an urban population percentage greater
        than the median percentage and is set to 0 otherwise.
    4.  Create a new copy of `USArrests` in your workspace, after
        deleting the `UrbanPop` column, leaving just the three crime
        rate variables. Then insert a new, fourth column in this object
        with `urbancat`.
    5.  Use the data frame from (iv) to produce a scatterplot matrix and
        other associated plots of the three crime rates against one
        another. Use `color` to split the crime rates according to the
        two levels of `urbancat`.

9.  Install the package `titanic`. Read the description of the dataset
    by `?titanic`.

    1.  Load the `titanic_test` and `titanic_train` datasets from the
        package.
    2.  Upon careful inspection you will find that the `titanic_test`
        dataset is a continuation of the `titanic_train` dataset.
        However, one column in `titanic_test` is missing. Identify the
        missing column and add the column to the `titanic_test` dataset
        with hypothetical column values similar to the one in the
        `titanic_train` dataset.
    3.  After completing i. and ii. combine the datasets into a single
        one and name it. Check the dimensions of the resulting dataset
        to confirm that you have all the data.
    4.  How many males did survie in iii? What was their most common
        age?
    5.  What kind of relationship can you infer between `Age` and
        `Class` in iii? (Use a box-plot.)
    6.  How is the fare distribution skewed in iii? Positive or
        negative?
    7.  Is there a correlation between fare and survival in iii?
