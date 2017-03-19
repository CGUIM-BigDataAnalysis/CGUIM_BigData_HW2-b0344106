長庚大學 大數據分析方法 作業二
================

數值變數運算
------------

``` r
num1<-3561
num2<-5815
num1+num2
```

    ## [1] 9376

``` r
num1-num2
```

    ## [1] -2254

``` r
num1*num2
```

    ## [1] 20707215

``` r
num1/num2
```

    ## [1] 0.6123818

檢查總覽資料
------------

``` r
str(iris)
```

    ## 'data.frame':    150 obs. of  5 variables:
    ##  $ Sepal.Length: num  5.1 4.9 4.7 4.6 5 5.4 4.6 5 4.4 4.9 ...
    ##  $ Sepal.Width : num  3.5 3 3.2 3.1 3.6 3.9 3.4 3.4 2.9 3.1 ...
    ##  $ Petal.Length: num  1.4 1.4 1.3 1.5 1.4 1.7 1.4 1.5 1.4 1.5 ...
    ##  $ Petal.Width : num  0.2 0.2 0.2 0.2 0.2 0.4 0.3 0.2 0.2 0.1 ...
    ##  $ Species     : Factor w/ 3 levels "setosa","versicolor",..: 1 1 1 1 1 1 1 1 1 1 ...

輸出系統現在日期
----------------

``` r
Sys.Date()
```

    ## [1] "2017-03-19"

字串比大小
----------

``` r
"A">"a"
```

    ## [1] TRUE

``` r
"b">"A"
```

    ## [1] TRUE

運作環境資訊擷取
----------------

``` r
sessionInfo()
```

    ## R version 3.3.2 (2016-10-31)
    ## Platform: x86_64-w64-mingw32/x64 (64-bit)
    ## Running under: Windows 10 x64 (build 14393)
    ## 
    ## locale:
    ## [1] LC_COLLATE=Chinese (Traditional)_Taiwan.950 
    ## [2] LC_CTYPE=Chinese (Traditional)_Taiwan.950   
    ## [3] LC_MONETARY=Chinese (Traditional)_Taiwan.950
    ## [4] LC_NUMERIC=C                                
    ## [5] LC_TIME=Chinese (Traditional)_Taiwan.950    
    ## 
    ## attached base packages:
    ## [1] stats     graphics  grDevices utils     datasets  methods   base     
    ## 
    ## loaded via a namespace (and not attached):
    ##  [1] backports_1.0.5 magrittr_1.5    rprojroot_1.2   tools_3.3.2    
    ##  [5] htmltools_0.3.5 yaml_2.1.14     Rcpp_0.12.9     stringi_1.1.2  
    ##  [9] rmarkdown_1.3   knitr_1.15.1    stringr_1.2.0   digest_0.6.12  
    ## [13] evaluate_0.10

``` r
installed.packages()
```

    ##              Package        LibPath                Version   Priority     
    ## backports    "backports"    "E:/R/R-3.3.2/library" "1.0.5"   NA           
    ## base         "base"         "E:/R/R-3.3.2/library" "3.3.2"   "base"       
    ## base64enc    "base64enc"    "E:/R/R-3.3.2/library" "0.1-3"   NA           
    ## bitops       "bitops"       "E:/R/R-3.3.2/library" "1.0-6"   NA           
    ## boot         "boot"         "E:/R/R-3.3.2/library" "1.3-18"  "recommended"
    ## caTools      "caTools"      "E:/R/R-3.3.2/library" "1.17.1"  NA           
    ## class        "class"        "E:/R/R-3.3.2/library" "7.3-14"  "recommended"
    ## cluster      "cluster"      "E:/R/R-3.3.2/library" "2.0.5"   "recommended"
    ## codetools    "codetools"    "E:/R/R-3.3.2/library" "0.2-15"  "recommended"
    ## compiler     "compiler"     "E:/R/R-3.3.2/library" "3.3.2"   "base"       
    ## datasets     "datasets"     "E:/R/R-3.3.2/library" "3.3.2"   "base"       
    ## digest       "digest"       "E:/R/R-3.3.2/library" "0.6.12"  NA           
    ## evaluate     "evaluate"     "E:/R/R-3.3.2/library" "0.10"    NA           
    ## foreign      "foreign"      "E:/R/R-3.3.2/library" "0.8-67"  "recommended"
    ## formatR      "formatR"      "E:/R/R-3.3.2/library" "1.4"     NA           
    ## graphics     "graphics"     "E:/R/R-3.3.2/library" "3.3.2"   "base"       
    ## grDevices    "grDevices"    "E:/R/R-3.3.2/library" "3.3.2"   "base"       
    ## grid         "grid"         "E:/R/R-3.3.2/library" "3.3.2"   "base"       
    ## highr        "highr"        "E:/R/R-3.3.2/library" "0.6"     NA           
    ## htmltools    "htmltools"    "E:/R/R-3.3.2/library" "0.3.5"   NA           
    ## jsonlite     "jsonlite"     "E:/R/R-3.3.2/library" "1.3"     NA           
    ## KernSmooth   "KernSmooth"   "E:/R/R-3.3.2/library" "2.23-15" "recommended"
    ## knitr        "knitr"        "E:/R/R-3.3.2/library" "1.15.1"  NA           
    ## lattice      "lattice"      "E:/R/R-3.3.2/library" "0.20-34" "recommended"
    ## magrittr     "magrittr"     "E:/R/R-3.3.2/library" "1.5"     NA           
    ## markdown     "markdown"     "E:/R/R-3.3.2/library" "0.7.7"   NA           
    ## MASS         "MASS"         "E:/R/R-3.3.2/library" "7.3-45"  "recommended"
    ## Matrix       "Matrix"       "E:/R/R-3.3.2/library" "1.2-7.1" "recommended"
    ## methods      "methods"      "E:/R/R-3.3.2/library" "3.3.2"   "base"       
    ## mgcv         "mgcv"         "E:/R/R-3.3.2/library" "1.8-15"  "recommended"
    ## mime         "mime"         "E:/R/R-3.3.2/library" "0.5"     NA           
    ## nlme         "nlme"         "E:/R/R-3.3.2/library" "3.1-128" "recommended"
    ## nnet         "nnet"         "E:/R/R-3.3.2/library" "7.3-12"  "recommended"
    ## parallel     "parallel"     "E:/R/R-3.3.2/library" "3.3.2"   "base"       
    ## Rcpp         "Rcpp"         "E:/R/R-3.3.2/library" "0.12.9"  NA           
    ## rmarkdown    "rmarkdown"    "E:/R/R-3.3.2/library" "1.3"     NA           
    ## rpart        "rpart"        "E:/R/R-3.3.2/library" "4.1-10"  "recommended"
    ## rprojroot    "rprojroot"    "E:/R/R-3.3.2/library" "1.2"     NA           
    ## spatial      "spatial"      "E:/R/R-3.3.2/library" "7.3-11"  "recommended"
    ## splines      "splines"      "E:/R/R-3.3.2/library" "3.3.2"   "base"       
    ## stats        "stats"        "E:/R/R-3.3.2/library" "3.3.2"   "base"       
    ## stats4       "stats4"       "E:/R/R-3.3.2/library" "3.3.2"   "base"       
    ## stringi      "stringi"      "E:/R/R-3.3.2/library" "1.1.2"   NA           
    ## stringr      "stringr"      "E:/R/R-3.3.2/library" "1.2.0"   NA           
    ## survival     "survival"     "E:/R/R-3.3.2/library" "2.39-5"  "recommended"
    ## tcltk        "tcltk"        "E:/R/R-3.3.2/library" "3.3.2"   "base"       
    ## tools        "tools"        "E:/R/R-3.3.2/library" "3.3.2"   "base"       
    ## translations "translations" "E:/R/R-3.3.2/library" "3.3.2"   NA           
    ## utils        "utils"        "E:/R/R-3.3.2/library" "3.3.2"   "base"       
    ## yaml         "yaml"         "E:/R/R-3.3.2/library" "2.1.14"  NA           
    ##              Depends                                          
    ## backports    "R (>= 3.0.0)"                                   
    ## base         NA                                               
    ## base64enc    "R (>= 2.9.0)"                                   
    ## bitops       NA                                               
    ## boot         "R (>= 3.0.0), graphics, stats"                  
    ## caTools      "R (>= 2.2.0)"                                   
    ## class        "R (>= 3.0.0), stats, utils"                     
    ## cluster      "R (>= 3.0.1)"                                   
    ## codetools    "R (>= 2.1)"                                     
    ## compiler     NA                                               
    ## datasets     NA                                               
    ## digest       "R (>= 2.4.1)"                                   
    ## evaluate     "R (>= 3.0.2)"                                   
    ## foreign      "R (>= 3.0.0)"                                   
    ## formatR      "R (>= 3.0.2)"                                   
    ## graphics     NA                                               
    ## grDevices    NA                                               
    ## grid         NA                                               
    ## highr        "R (>= 3.0.2)"                                   
    ## htmltools    "R (>= 2.14.1)"                                  
    ## jsonlite     "methods"                                        
    ## KernSmooth   "R (>= 2.5.0), stats"                            
    ## knitr        "R (>= 3.1.0)"                                   
    ## lattice      "R (>= 3.0.0)"                                   
    ## magrittr     NA                                               
    ## markdown     "R (>= 2.11.1)"                                  
    ## MASS         "R (>= 3.1.0), grDevices, graphics, stats, utils"
    ## Matrix       "R (>= 3.0.1)"                                   
    ## methods      NA                                               
    ## mgcv         "R (>= 2.14.0), nlme (>= 3.1-64)"                
    ## mime         NA                                               
    ## nlme         "R (>= 3.0.2)"                                   
    ## nnet         "R (>= 2.14.0), stats, utils"                    
    ## parallel     NA                                               
    ## Rcpp         "R (>= 3.0.0)"                                   
    ## rmarkdown    "R (>= 3.0)"                                     
    ## rpart        "R (>= 2.15.0), graphics, stats, grDevices"      
    ## rprojroot    "R (>= 3.0.0)"                                   
    ## spatial      "R (>= 3.0.0), graphics, stats, utils"           
    ## splines      NA                                               
    ## stats        NA                                               
    ## stats4       NA                                               
    ## stringi      "R (>= 2.13.1)"                                  
    ## stringr      "R (>= 2.14)"                                    
    ## survival     "R (>= 2.13.0)"                                  
    ## tcltk        NA                                               
    ## tools        NA                                               
    ## translations NA                                               
    ## utils        NA                                               
    ## yaml         NA                                               
    ##              Imports                                                                                                                                      
    ## backports    "utils"                                                                                                                                      
    ## base         NA                                                                                                                                           
    ## base64enc    NA                                                                                                                                           
    ## bitops       NA                                                                                                                                           
    ## boot         NA                                                                                                                                           
    ## caTools      "bitops"                                                                                                                                     
    ## class        "MASS"                                                                                                                                       
    ## cluster      "graphics, grDevices, stats, utils"                                                                                                          
    ## codetools    NA                                                                                                                                           
    ## compiler     NA                                                                                                                                           
    ## datasets     NA                                                                                                                                           
    ## digest       NA                                                                                                                                           
    ## evaluate     "methods, stringr (>= 0.6.2)"                                                                                                                
    ## foreign      "methods, utils, stats"                                                                                                                      
    ## formatR      NA                                                                                                                                           
    ## graphics     "grDevices"                                                                                                                                  
    ## grDevices    NA                                                                                                                                           
    ## grid         "grDevices, utils"                                                                                                                           
    ## highr        NA                                                                                                                                           
    ## htmltools    "utils, digest, Rcpp"                                                                                                                        
    ## jsonlite     NA                                                                                                                                           
    ## KernSmooth   NA                                                                                                                                           
    ## knitr        "evaluate (>= 0.10), digest, highr, markdown, stringr (>= 0.6),\nyaml, methods, tools"                                                       
    ## lattice      "grid, grDevices, graphics, stats, utils"                                                                                                    
    ## magrittr     NA                                                                                                                                           
    ## markdown     "mime (>= 0.3)"                                                                                                                              
    ## MASS         "methods"                                                                                                                                    
    ## Matrix       "methods, graphics, grid, stats, utils, lattice"                                                                                             
    ## methods      "utils, stats"                                                                                                                               
    ## mgcv         "methods, stats, graphics, Matrix"                                                                                                           
    ## mime         "tools"                                                                                                                                      
    ## nlme         "graphics, stats, utils, lattice"                                                                                                            
    ## nnet         NA                                                                                                                                           
    ## parallel     "tools"                                                                                                                                      
    ## Rcpp         "methods, utils"                                                                                                                             
    ## rmarkdown    "tools, utils, knitr (>= 1.14), yaml (>= 2.1.5), htmltools (>=\n0.3.5), caTools, evaluate (>= 0.8), base64enc, jsonlite,\nrprojroot, methods"
    ## rpart        NA                                                                                                                                           
    ## rprojroot    "backports"                                                                                                                                  
    ## spatial      NA                                                                                                                                           
    ## splines      "graphics, stats"                                                                                                                            
    ## stats        "utils, grDevices, graphics"                                                                                                                 
    ## stats4       "graphics, methods, stats"                                                                                                                   
    ## stringi      "tools, utils, stats"                                                                                                                        
    ## stringr      "stringi (>= 0.4.1), magrittr"                                                                                                               
    ## survival     "graphics, Matrix, methods, splines, stats, utils"                                                                                           
    ## tcltk        "utils"                                                                                                                                      
    ## tools        NA                                                                                                                                           
    ## translations NA                                                                                                                                           
    ## utils        NA                                                                                                                                           
    ## yaml         NA                                                                                                                                           
    ##              LinkingTo
    ## backports    NA       
    ## base         NA       
    ## base64enc    NA       
    ## bitops       NA       
    ## boot         NA       
    ## caTools      NA       
    ## class        NA       
    ## cluster      NA       
    ## codetools    NA       
    ## compiler     NA       
    ## datasets     NA       
    ## digest       NA       
    ## evaluate     NA       
    ## foreign      NA       
    ## formatR      NA       
    ## graphics     NA       
    ## grDevices    NA       
    ## grid         NA       
    ## highr        NA       
    ## htmltools    "Rcpp"   
    ## jsonlite     NA       
    ## KernSmooth   NA       
    ## knitr        NA       
    ## lattice      NA       
    ## magrittr     NA       
    ## markdown     NA       
    ## MASS         NA       
    ## Matrix       NA       
    ## methods      NA       
    ## mgcv         NA       
    ## mime         NA       
    ## nlme         NA       
    ## nnet         NA       
    ## parallel     NA       
    ## Rcpp         NA       
    ## rmarkdown    NA       
    ## rpart        NA       
    ## rprojroot    NA       
    ## spatial      NA       
    ## splines      NA       
    ## stats        NA       
    ## stats4       NA       
    ## stringi      NA       
    ## stringr      NA       
    ## survival     NA       
    ## tcltk        NA       
    ## tools        NA       
    ## translations NA       
    ## utils        NA       
    ## yaml         NA       
    ##              Suggests                                                                                                                                                         
    ## backports    NA                                                                                                                                                               
    ## base         "methods"                                                                                                                                                        
    ## base64enc    NA                                                                                                                                                               
    ## bitops       NA                                                                                                                                                               
    ## boot         "MASS, survival"                                                                                                                                                 
    ## caTools      "MASS, rpart"                                                                                                                                                    
    ## class        NA                                                                                                                                                               
    ## cluster      "MASS"                                                                                                                                                           
    ## codetools    NA                                                                                                                                                               
    ## compiler     NA                                                                                                                                                               
    ## datasets     NA                                                                                                                                                               
    ## digest       "knitr, rmarkdown"                                                                                                                                               
    ## evaluate     "testthat, lattice, ggplot2"                                                                                                                                     
    ## foreign      NA                                                                                                                                                               
    ## formatR      "codetools, shiny, testit, knitr"                                                                                                                                
    ## graphics     NA                                                                                                                                                               
    ## grDevices    "KernSmooth"                                                                                                                                                     
    ## grid         "lattice"                                                                                                                                                        
    ## highr        "knitr, testit"                                                                                                                                                  
    ## htmltools    "markdown, testthat"                                                                                                                                             
    ## jsonlite     "httr, curl, plyr, testthat, knitr, rmarkdown, R.rsp"                                                                                                            
    ## KernSmooth   "MASS"                                                                                                                                                           
    ## knitr        "formatR, testit, rgl (>= 0.95.1201), codetools, rmarkdown,\nhtmlwidgets (>= 0.7), webshot, tikzDevice (>= 0.10), png, jpeg,\nXML, RCurl, DBI (>= 0.4-1), tibble"
    ## lattice      "KernSmooth, MASS"                                                                                                                                               
    ## magrittr     "testthat, knitr"                                                                                                                                                
    ## markdown     "knitr, RCurl"                                                                                                                                                   
    ## MASS         "lattice, nlme, nnet, survival"                                                                                                                                  
    ## Matrix       "expm, MASS"                                                                                                                                                     
    ## methods      "codetools"                                                                                                                                                      
    ## mgcv         "splines, parallel, survival, MASS"                                                                                                                              
    ## mime         NA                                                                                                                                                               
    ## nlme         "Hmisc, MASS"                                                                                                                                                    
    ## nnet         "MASS"                                                                                                                                                           
    ## parallel     "methods"                                                                                                                                                        
    ## Rcpp         "RUnit, inline, rbenchmark, highlight, pkgKitten (>= 0.1.2)"                                                                                                     
    ## rmarkdown    "shiny (>= 0.11), tufte, testthat, digest, tibble"                                                                                                               
    ## rpart        "survival"                                                                                                                                                       
    ## rprojroot    "testthat, knitr, withr, rmarkdown"                                                                                                                              
    ## spatial      "MASS"                                                                                                                                                           
    ## splines      "Matrix, methods"                                                                                                                                                
    ## stats        "MASS, Matrix, SuppDists, methods, stats4"                                                                                                                       
    ## stats4       NA                                                                                                                                                               
    ## stringi      NA                                                                                                                                                               
    ## stringr      "testthat, knitr, htmltools, htmlwidgets, rmarkdown, covr"                                                                                                       
    ## survival     NA                                                                                                                                                               
    ## tcltk        NA                                                                                                                                                               
    ## tools        "codetools, methods, xml2"                                                                                                                                       
    ## translations NA                                                                                                                                                               
    ## utils        "methods, XML"                                                                                                                                                   
    ## yaml         "testthat"                                                                                                                                                       
    ##              Enhances                               
    ## backports    NA                                     
    ## base         NA                                     
    ## base64enc    "png"                                  
    ## bitops       NA                                     
    ## boot         NA                                     
    ## caTools      NA                                     
    ## class        NA                                     
    ## cluster      NA                                     
    ## codetools    NA                                     
    ## compiler     NA                                     
    ## datasets     NA                                     
    ## digest       NA                                     
    ## evaluate     NA                                     
    ## foreign      NA                                     
    ## formatR      NA                                     
    ## graphics     NA                                     
    ## grDevices    NA                                     
    ## grid         NA                                     
    ## highr        NA                                     
    ## htmltools    "knitr"                                
    ## jsonlite     NA                                     
    ## KernSmooth   NA                                     
    ## knitr        NA                                     
    ## lattice      "chron"                                
    ## magrittr     NA                                     
    ## markdown     NA                                     
    ## MASS         NA                                     
    ## Matrix       "MatrixModels, graph, SparseM, sfsmisc"
    ## methods      NA                                     
    ## mgcv         NA                                     
    ## mime         NA                                     
    ## nlme         NA                                     
    ## nnet         NA                                     
    ## parallel     "snow, nws, Rmpi"                      
    ## Rcpp         NA                                     
    ## rmarkdown    NA                                     
    ## rpart        NA                                     
    ## rprojroot    NA                                     
    ## spatial      NA                                     
    ## splines      NA                                     
    ## stats        NA                                     
    ## stats4       NA                                     
    ## stringi      NA                                     
    ## stringr      NA                                     
    ## survival     NA                                     
    ## tcltk        NA                                     
    ## tools        NA                                     
    ## translations NA                                     
    ## utils        NA                                     
    ## yaml         NA                                     
    ##              License                       License_is_FOSS
    ## backports    "GPL-2"                       NA             
    ## base         "Part of R 3.3.2"             NA             
    ## base64enc    "GPL-2 | GPL-3"               NA             
    ## bitops       "GPL (>= 2)"                  NA             
    ## boot         "Unlimited"                   NA             
    ## caTools      "GPL-3"                       NA             
    ## class        "GPL-2 | GPL-3"               NA             
    ## cluster      "GPL (>= 2)"                  NA             
    ## codetools    "GPL"                         NA             
    ## compiler     "Part of R 3.3.2"             NA             
    ## datasets     "Part of R 3.3.2"             NA             
    ## digest       "GPL (>= 2)"                  NA             
    ## evaluate     "MIT + file LICENSE"          NA             
    ## foreign      "GPL (>= 2)"                  NA             
    ## formatR      "GPL"                         NA             
    ## graphics     "Part of R 3.3.2"             NA             
    ## grDevices    "Part of R 3.3.2"             NA             
    ## grid         "Part of R 3.3.2"             NA             
    ## highr        "GPL"                         NA             
    ## htmltools    "GPL (>= 2)"                  NA             
    ## jsonlite     "MIT + file LICENSE"          NA             
    ## KernSmooth   "Unlimited"                   NA             
    ## knitr        "GPL"                         NA             
    ## lattice      "GPL (>= 2)"                  NA             
    ## magrittr     "MIT + file LICENSE"          NA             
    ## markdown     "GPL-2"                       NA             
    ## MASS         "GPL-2 | GPL-3"               NA             
    ## Matrix       "GPL (>= 2) | file LICENCE"   NA             
    ## methods      "Part of R 3.3.2"             NA             
    ## mgcv         "GPL (>= 2)"                  NA             
    ## mime         "GPL"                         NA             
    ## nlme         "GPL (>= 2) | file LICENCE"   NA             
    ## nnet         "GPL-2 | GPL-3"               NA             
    ## parallel     "Part of R 3.3.2"             NA             
    ## Rcpp         "GPL (>= 2)"                  NA             
    ## rmarkdown    "GPL-3"                       NA             
    ## rpart        "GPL-2 | GPL-3"               NA             
    ## rprojroot    "GPL-3"                       NA             
    ## spatial      "GPL-2 | GPL-3"               NA             
    ## splines      "Part of R 3.3.2"             NA             
    ## stats        "Part of R 3.3.2"             NA             
    ## stats4       "Part of R 3.3.2"             NA             
    ## stringi      "file LICENSE"                "yes"          
    ## stringr      "GPL-2 | file LICENSE"        NA             
    ## survival     "LGPL (>= 2)"                 NA             
    ## tcltk        "Part of R 3.3.2"             NA             
    ## tools        "Part of R 3.3.2"             NA             
    ## translations "Part of R 3.3.2"             NA             
    ## utils        "Part of R 3.3.2"             NA             
    ## yaml         "BSD_3_clause + file LICENSE" NA             
    ##              License_restricts_use OS_type MD5sum NeedsCompilation Built  
    ## backports    NA                    NA      NA     "no"             "3.3.2"
    ## base         NA                    NA      NA     NA               "3.3.2"
    ## base64enc    NA                    NA      NA     "yes"            "3.3.2"
    ## bitops       NA                    NA      NA     "yes"            "3.3.2"
    ## boot         NA                    NA      NA     "no"             "3.3.2"
    ## caTools      NA                    NA      NA     "yes"            "3.3.2"
    ## class        NA                    NA      NA     "yes"            "3.3.2"
    ## cluster      NA                    NA      NA     "yes"            "3.3.2"
    ## codetools    NA                    NA      NA     "no"             "3.3.2"
    ## compiler     NA                    NA      NA     NA               "3.3.2"
    ## datasets     NA                    NA      NA     NA               "3.3.2"
    ## digest       NA                    NA      NA     "yes"            "3.3.2"
    ## evaluate     NA                    NA      NA     "no"             "3.3.2"
    ## foreign      NA                    NA      NA     "yes"            "3.3.2"
    ## formatR      NA                    NA      NA     "no"             "3.3.2"
    ## graphics     NA                    NA      NA     "yes"            "3.3.2"
    ## grDevices    NA                    NA      NA     "yes"            "3.3.2"
    ## grid         NA                    NA      NA     "yes"            "3.3.2"
    ## highr        NA                    NA      NA     "no"             "3.3.2"
    ## htmltools    NA                    NA      NA     "yes"            "3.3.2"
    ## jsonlite     NA                    NA      NA     "yes"            "3.3.2"
    ## KernSmooth   NA                    NA      NA     "yes"            "3.3.2"
    ## knitr        NA                    NA      NA     "no"             "3.3.2"
    ## lattice      NA                    NA      NA     "yes"            "3.3.2"
    ## magrittr     NA                    NA      NA     "no"             "3.3.2"
    ## markdown     NA                    NA      NA     "yes"            "3.3.2"
    ## MASS         NA                    NA      NA     "yes"            "3.3.2"
    ## Matrix       NA                    NA      NA     "yes"            "3.3.2"
    ## methods      NA                    NA      NA     "yes"            "3.3.2"
    ## mgcv         NA                    NA      NA     "yes"            "3.3.2"
    ## mime         NA                    NA      NA     "yes"            "3.3.2"
    ## nlme         NA                    NA      NA     "yes"            "3.3.2"
    ## nnet         NA                    NA      NA     "yes"            "3.3.2"
    ## parallel     NA                    NA      NA     "yes"            "3.3.2"
    ## Rcpp         NA                    NA      NA     "yes"            "3.3.2"
    ## rmarkdown    NA                    NA      NA     "no"             "3.3.2"
    ## rpart        NA                    NA      NA     "yes"            "3.3.2"
    ## rprojroot    NA                    NA      NA     "no"             "3.3.2"
    ## spatial      NA                    NA      NA     "yes"            "3.3.2"
    ## splines      NA                    NA      NA     "yes"            "3.3.2"
    ## stats        NA                    NA      NA     "yes"            "3.3.2"
    ## stats4       NA                    NA      NA     NA               "3.3.2"
    ## stringi      NA                    NA      NA     "yes"            "3.3.2"
    ## stringr      NA                    NA      NA     "no"             "3.3.2"
    ## survival     NA                    NA      NA     "yes"            "3.3.2"
    ## tcltk        NA                    NA      NA     "yes"            "3.3.2"
    ## tools        NA                    NA      NA     "yes"            "3.3.2"
    ## translations NA                    NA      NA     NA               "3.3.2"
    ## utils        NA                    NA      NA     "yes"            "3.3.2"
    ## yaml         NA                    NA      NA     "yes"            "3.3.2"
