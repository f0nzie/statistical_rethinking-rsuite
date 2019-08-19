# statistical_rethinking-rsuite

<!-- badges: start -->
<!-- badges: end -->


## Statistical Rethinking ebook built with rsuite

### How is this different

This ebook, [Statistical Rethinking with brms, ggplot2, and the tidyverse](https://bookdown.org/ajkurz/Statistical_Rethinking_recoded/), was created with `bookdown`. It is different in the way it has been built, and can be rebuilt, helping with **reproducibility**. 

I have used [rsuite](https://rsuite.io/) to make this ebook fully reproducible. This ebook is one of the most difficult that I have found in matching all the dependencies. In addition, it uses `stan`. After all it is about Bayesian statistics using `Stan` and `rstan`. I love this book but, unfortunately, after a R package upgrade it will stop building.

So, what I did is creating an isolated environment for the book, one where all the packages are spelled out in advance so the ebook can be rebuilt after an R re-installation, a new R version, or a full package upgrade. The book will be able to be regenerated to the CRAN snapshot at the time it was first built.

Because `rsuite` allows a supervising project on top of other projects or packages, you can control the date of the snapshot; the R version under you want the book to be built; the names of all the packages that satisfy the dependencies for the book to work; place the source code of the package if the package is not in CRAN; along with a master project and a master package that takes care of reproducing the whole book, again and again, even after changing the operating system.

## How to reproduce this ebook yourself
1. Download and install the RSuite client. Available for Linux, Mac and Windows.
2. Install the `rsuite` package with `rsuite install`
3. Clone or download this repository.
4. Change to this repo folder and install the dependencies on its own isolated reproducible environment. Use `rsuite proj depsinst`
5. Build the project with `rsuite proj build`
6. Go to the folder `/work/book` and open the project `Statistical Rethinking with brms, ggplot2, and the tidyverse.Rproj`.
7. Click on the RStudio `Build book`
8. Enjoy


## References

* [McElreath, R. (2016). Statistical rethinking: A Bayesian course with examples in R and Stan. Chapman & Hall/CRC Press.](https://xcelab.net/rm/statistical-rethinking/)

* [Statistical Rethinking with brms, ggplot2, and the tidyverse](https://bookdown.org/ajkurz/Statistical_Rethinking_recoded/)

* [Bookdown](https://bookdown.org/)

* [Rsuite](https://rsuite.io/)

* [Stan](https://mc-stan.org/)

* [rstan](https://github.com/stan-dev/rstan)

