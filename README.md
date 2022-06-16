# SICSS-Howard/Mathematica 2022

- Saturday June 18 from 2:30-5:30PM EST on Zoom
- Sunday June 19 from 2:00-5:00PM EST on Zoom

Author and instructor: [Evan Muzzall, Stanford University](https://library.stanford.edu/people/muzzall) muzzall {at} stanford {dot} edu

Assistant: [Jose Aveldanes, UC Berkeley](https://dlab.berkeley.edu/people/jose-aveldanes)

These are the R workshop materials for [SICSS-HOWARD/Mathematica Summer Institute in Computational Social Science 2022](https://sicss.io/2021/howard-mathematica/) at [Howard University](https://howard.edu/). 

They are inspired by and borrow from [Jae Yeon Kim's]() version from [2021](https://github.com/jaeyk/sicss-howard-r-boot-camp). 

# Workshop goals

This workshop will introduce you to a variety of computational methods in R that can be applied to your own research and give you the confidence to approach old and new projects as an independent learner. Each section will build on the previous one in some way, so be sure to start thinking about the connections in a way that makes sense to you! Also, try to keep a list of questions of things that do not make sense. 

If you are a beginner, you will learn how the computational aspect fits into a basic social science research workflow using the R programming language and RStudio programming environment. 

If you are already an R user this will be a good opportunity to refresh and structure your existing knowledge, while building confidence with the tidyverse to accomplish more complex tasks in easier ways. I encourage you to contribute your perspectives to the topics being covered, strengths and weaknesses, potential pitfalls, and more efficient ways of doing things. 

There are many more topics we cannot get to due to time constraints, such as accessing the American Community Survey through the `tidycensus` package, webscraping, text analysis, machine learning, and more! Contact me if you want to talk more. 

## Datasets

We will use data from the [The Stanford Open Policing Project](https://openpolicing.stanford.edu/), the [Gapminder Foundation](https://www.gapminder.org/), the Midwest demographics dataset, and numerous other toy examples throughout to keep you thinking on your feet.

# Organization of these materials
- Part1.Rmd and Part2.Rmd - R Markdown files that contain the coding walkthroughs for this workshop
- README.md - markdown file that contains the the information you are currently reading
- runtime.txt - text file that defines the R version to be loaded by Binder (cloud-based version of RStudio)
- install.R - R script that contains packages to be loaded by Binder
- solutions.Rmd - R Markdown file that contains challenge question solutions
- sicss_howard_mathematica_2022.Rproj - R Project file that bundles all of these materials
- data/ - folder containing the raw and preprocessed data
- html/ - folder with the hypertext markup language (html) versions of the code scripts you can open in your web browser
- img/ - folder with the images used in these workshop materials

# Schedule

After the lecture-heavy first half of Part 1, each section will be divided into a coding walkthrough demonstration followed by a challenge question for you to apply what you have learned. 

## Saturday June 18 - Overview of the research process

- 2:30-3:15: Introductions and installations
  - Computational Social Science (CSS) example research workflow
  - R (programming language)
  - RStudio (programming environment)
    - Source files: 
      - Script
      - R Markdown
    - Navigating RStudio
  - R projects
- 3:15-4:00: Basic building blocks of R programming
  - Objects, functions, and arguments
  - Variable assignment
  - Data types: numeric, character, logical, integer, factor
  - Data structures: vector, data frame
  - Indexing
  - Subsetting single columns with `$`
  - Subsetting rows and columns with bracket notation `[,]`
  - Getting help
- 4:00-4:15: Break
- 4:15-5:15: Putting it all together: CSS research workflow example
  - Package installation
  - Import data
  - Wrangle
  - Summarize
  - Visualize
  - Interpret
- 5:15-5:30: Save your work
  - A note on computational reproducibility

## Sunday June 19 - Deep dives into data reshaping, wrangling, visualization, and modeling

- 2:00-2:30: The tidyverse approach: Reshaping data with `tidyr` functions
  - pipes `>%>`
  - `pivot_longer()`
  - `pivot_wider()`
  - Missing values
- 2:30-3:15: Wrangling data with `dplyr` 
  - `arrange()` 
  - `rename()`
  - `filter()`
  - `select()`
  - `count()`
  - `group_by()`
  - `summarize()`
  - `mutate()`
  - Create publishable ready tables
- 3:15-3:30: Break
- 3:30-4:15: Data visualization with `ggplot2`
  - Anscombe's quartet motivating example
  - The grammar of graphics 
  - Mapping with `aes()`, and `geom_`
  - `geom_histogram()` 
  - Size, color, coordinates, scales, labels, guides
  - Saving/exporting figures
  - Multiple plots: Facetting and compound figures
  - Plotting text
  - Plotting models
- 4:15-5:00: Statistical modeling with `broom` 
  - `nest()` and `unnest()`
  - `glance()`, `tidy()`, and `augment()`

# Setup - R and RStudio Installations

Install both R and RStudio. While they are often referred to synonymously, they are actually two different things: 

- R is the programming language we will use to give instructions to our computer to perform data-related tasks. 
- RStudio is the environment that we will program R in. 

## R

- [Mac users click here to install R](https://cloud.r-project.org/bin/macosx/base/R-4.2.0.pkg)
- [Windows users click here to install R](https://cloud.r-project.org/bin/windows/base/R-4.2.0-win.exe)

## RStudio

- [Mac and Windows users click here to install RStudio. Click the blue button that says "Recommended for your system:"](https://www.rstudio.com/products/rstudio/download/#download)

## Binder

Please try and install R and RStudio before the workshop start time. If you cannot, simply click the Binder button below to launch a version of these workshop materials in RStudio in your preferred web browser. This will take a few minutes to load, so be sure to do so before the workshop start time. 

Click this button [[![Binder]https://mybinder.org/v2/gh/EastBayEv/sicss-howard-mathematica-R-2022/HEAD?urlpath=rstudio]](https://mybinder.org/v2/gh/EastBayEv/sicss-howard-mathematica-R-2022/HEAD?urlpath=rstudio) to launch Binder.

# Download these workshop materials

If you plan to use these materials locally on your personal computer, download these materials by following the below steps: 
  1. Visit: https://github.com/EastBayEv/sicss-howard-mathematica-R-2022
  2. Click the green "Code" button
  3. Click "Download Zip"
  4. Extract the archive someplace familiar (e.g., Desktop)

> Git users can simply `git clone https://github.com/EastBayEv/sicss-howard-mathematica-R-2022.git`

# Get started

Open the file `Part1.Rmd` to get started. 

# Resources 

- Kim JY. 2022. [Computational Thinking for Social Scientists](https://jaeyk.github.io/comp_thinking_social_science/)
- Kerns GJ. 2010. [Introduction to Probability and Statistics Using R](http://ipsur.r-forge.r-project.org/book/download/IPSUR.pdf)
- Wilke CO. 2022. [Fundamentals of Data Visualization](https://clauswilke.com/dataviz/)
- Wickham H. 2022. [Advanced R](https://adv-r.hadley.nz/)
- Wickham H, Grolemund G. 20[R for Data Science (learn the tidyverse)](https://r4ds.had.co.nz/)
- Silge J, Robinson D. 2022. [Text Mining with R - A tidy Approach](https://www.tidytextmining.com/)
- James G, Witten D, Hastie T, Tibshirani R. 2021. [An Introduction to Statistical Learning - with Applications in R](https://www.statlearning.com/)
- [RStudio cheatsheets](https://www.rstudio.com/resources/cheatsheets/)
- Mangiafico SS. 2022. [R Companion - Introduction to Parametric and Non-Parametric Tests](https://rcompanion.org/handbook/I_01.html)
- du Prel JB, Hommel G, Röhrig B, Blettner M. 2009. [Confidence Interval or P-Value?](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2689604/)
- Mensh B, Kording K. 2017. [Ten simple rules for structuring papers](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005619)
- tidyverse: https://www.tidyverse.org/
- tidyr: https://www.tidyverse.org/blog/2019/09/tidyr-1-0-0/
- dplyr: https://cran.r-project.org/web/packages/dplyr/vignettes/dplyr.html
- ggplot2: https://ggplot2-book.org/
- broom: https://cran.r-project.org/web/packages/broom/vignettes/broom.html
- tidycensus: https://csde-uw.github.io/tidycensus-tutorial/

![](https://i.creativecommons.org/l/by/4.0/88x31.png) This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).
