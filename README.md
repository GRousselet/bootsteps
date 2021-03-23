Reproducibility package for the article:

**The percentile bootstrap: a primer with step-by-step instructions in R**  
Rousselet G.A., Pernet C.R., Wilcox R.R. (2020)  
*Advances in Methods and Practices in Psychological Science*  

[[Article](https://journals.sagepub.com/doi/10.1177/2515245920911881)]

[[GitHub repository](https://github.com/GRousselet/bootsteps)]

[[OSF repository](https://osf.io/dvuze/)]

This tutorial provides a very short and lightweight introduction to the percentile bootstrap. For a more substantial tutorial, see [here](https://osf.io/8b4t5/).

The repository contains the [R](https://www.r-project.org/) code  used in the article. The code is best seen by running the RMarkdown notebook in [RStudio](https://www.rstudio.com/).

The code is released under the [MIT license](https://opensource.org/licenses/MIT). Copyright 2019-2020, Guillaume A. Rousselet.

The figures are released under the [CC-BY 4.0 license](https://creativecommons.org/licenses/by/4.0/legalcode). Copyright 2019-2020, Rousselet, Pernet & Wilcox.

# Content
|folder|description|location|
|-----|-----|-----|
|`bootsteps.Rmd`|RMarkdown file to create figures and run the simulation|OSF + GitHub|
|`bootsteps.pdf`|pdf versions of the code, with embedded figures|OSF|
|`data`|simulation results needed to run the code|OSF + GitHub|
|`figures`|all the figures used in the article, in pdf format|OSF|
|`functions`|extra R functions defined in text files|OSF + GitHub|

# R packages needed
If you want to run the code in RStudio and reproduce the figures, you will need to install three packages, which you can do by typing this in the console:

`install.packages(c("ggplot2", "tibble", "boot", "simpleboot", "SimJoint"))`

Or you can navigate in the GUI to Tools > Install Packages...

## Robust estimation and hypothesis testing
To get all the statistical functions from Rand Wilcox, select the `Rallfun-v35.txt` file in the `functions` folder. See details on this [webpage](https://dornsife.usc.edu/labs/rwilcox/software/). The full description of the functions is available in the book [Introduction to Robust Estimation and Hypothesis Testing](https://books.google.co.uk/books/about/Introduction_to_Robust_Estimation_and_Hy.html?id=8f8nBb4__EYC&printsec=frontcover&source=kp_read_button&redir_esc=y#v=onepage&q&f=false).

The notebook `bootsteps.Rmd` will install the appropriate functions for you; otherwise, in the console you can type `source(file.choose())` and select the relevant `.txt` file.

## Other function
The file [theme_gar.txt](https://github.com/GRousselet/articles/blob/master/bootstrap/functions/theme_gar.txt) contains custom code to set some `ggplot2` parameters.

# Extra resources

## R packages for bootstrap inferences

For packages not focused on bootstrap methods, example functions are provided in brackets. The full references are available in the article.

- [`bootstrap`](https://cran.r-project.org/web/packages/bootstrap/) (Efron & Tibshirani, 1994; Tibshirani & Leisch, 2019)

- [`boot`](https://cran.r-project.org/web/packages/boot/) (Canty & Ripley, 2017; Davison & Hinkley, 1997)

- [`simpleboot`](https://cran.r-project.org/web/packages/simpleboot/) (Peng, 2019)

- [`WRS2`](https://cran.r-project.org/web/packages/WRS2/) (Mair & Wilcox, 2019)

- [`resample`](https://cran.r-project.org/web/packages/resample/) (Hesterberg, 2015a)

- [`car` (`Boot`)](https://cran.r-project.org/web/packages/car/) (Fox & Weisberg, 2019)

- [`nlstools` (`nlsBoot`)](https://cran.r-project.org/web/packages/nlstools/) (Baty et al., 2015)

- [`dabestr`](https://cran.r-project.org/web/packages/dabestr/) (Ho, Tumkaya, Aryal, Choi, & Claridge-Chang, 2019)

- [`rogme`](https://github.com/GRousselet/rogme) (Rousselet, Pernet, & Wilcox, 2017)

## Interactive demo
[Frequentist inference: confidence interval & bootstrap](https://seeing-theory.brown.edu/frequentist-inference/index.html#section2)

## Books
Suggested books on bootstrap methods, robust statistics and simulations.

[An Introduction to the Bootstrap](https://books.google.co.uk/books?id=gLlpIUxRntoC&printsec=frontcover&dq=bootstrap+efron&hl=en&sa=X&ved=0ahUKEwjiv676orHiAhVIRxUIHYkgAckQ6AEIKDAA#v=onepage&q=bootstrap%20efron&f=false)

[Robust Statistics](https://books.google.co.uk/books?id=yAmZsxWSEWgC&dq=mathematical+foundations+of+robust+statistics&hl=en&sa=X&ved=0ahUKEwj3tP6Oo7HiAhU_UhUIHftBCnQQ6AEILjAB)

[Introduction to Robust Estimation and Hypothesis Testing](https://books.google.co.uk/books/about/Introduction_to_Robust_Estimation_and_Hy.html?id=8f8nBb4__EYC&printsec=frontcover&source=kp_read_button&redir_esc=y#v=onepage&q&f=false)

[Computer Age Statistical Inference](https://books.google.co.uk/books?id=Sj1yDAAAQBAJ&printsec=frontcover&dq=computer+inference+efron&hl=en&sa=X&ved=0ahUKEwiXy7vjorHiAhU4SxUIHUm7A3kQ6AEIKDAA#v=onepage&q=computer%20inference%20efron&f=false)

[Statistics: Unlocking the Power of Data](https://books.google.co.uk/books?id=EpBEDwAAQBAJ&printsec=frontcover&dq=Statistics:+Unlocking+the+Power+of+Data&hl=en&sa=X&ved=0ahUKEwil1unSorHiAhUPTxUIHfCwBjEQ6AEIKDAA#v=onepage&q=Statistics%3A%20Unlocking%20the%20Power%20of%20Data&f=false)

[Introduction to Statistical Investigations](https://books.google.co.uk/books?id=FsvVwQEACAAJ&dq=Introduction+to+Statistical+Investigations&hl=en&sa=X&ved=0ahUKEwigt_2worHiAhUySBUIHcZqCnAQ6AEIKDAA)

[Mathematical Statistics with Resampling and R](https://books.google.co.uk/books?id=_2hvDwAAQBAJ&printsec=frontcover&dq=Mathematical+Statistics+with+Resampling+and+R&hl=en&sa=X&ved=0ahUKEwiEj_-gorHiAhXkQhUIHRauC-IQ6AEILzAB#v=onepage&q=Mathematical%20Statistics%20with%20Resampling%20and%20R&f=false)
