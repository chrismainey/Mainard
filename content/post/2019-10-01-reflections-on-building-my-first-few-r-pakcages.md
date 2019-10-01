---
title: Reflections on building my first few R pakcages
author: ''
date: '2019-10-01'
slug: reflections-on-building-my-first-few-r-pakcages
categories:
  - R
tags:
  - R
  - package
summary: "HEDfunctions, FunnelPlotR and NHSRdatasets reflections"
image:
  caption: ''
  focal_point: ''
output:
  blogdown::html_page:
    toc: true
    number_sections: true
    toc_depth: 1
draft: false
---

# Package development

I've spent much of the last six months building several `R` packages.  It's the first time that I'd built packages, and I hope the released versions are much better now that they were at initial release!  This post is not a tutorial on how to build packages, but will summarise some parts I've had to learn, and aims to whos you that pakcages building is not magic.  It's particuarlrly accessible now with RStudio, `devtools`, `usethis` and `git` in combination.

## Packages

I've build or collaboraed on three packages recently:

+ `FunnelPlotR`: `ggplot2` methods for producting funnel plots of indirectly standardised ratios with overdispersion adjustment
+ `NHSRdatasets`: a free, collaborative datasets package with examples of health related data, to provide in-context examples for NHS-R community and others learning `in health`R`.
+ `HEDfunctions`: an HED internal package that contains methods for some of the models build in HED production, and several utility functions like confidence intervals etc.

I first went about htis b watching a couple of YouTube videos aon package build.  These videos used the RStudio wizards to set up the package, as well as `roxygen2` to generate documentation.

## Git and GitHub


## Vignettes

Vignette are the term used for 'worked examples.' They range from a few lines to show you how to use a function, to long tutorials on package use.  Some cotian several vignettes, demosntrating special cases or variants of use. I think they are helpful for demonstrating the motivation and application of a package, and I believe all packages released on CRAN should include at least one.

You can use `rmarkdown` to create vignettes.  In doing so, you need to include a few things:

1. Specificy YAML to tell the package build what it is and how to process it
1. Add `rmarkdown` and `knitr` to the Description, in `Suggests` (and the namespace).
1. Consider where image for plots are being store

The easiest way to solve all three is to call `usethis::use_vignette()`.  This sets up the YAML, picture location and the requiredd packages.  I didn't relaise this at first, and had copied the YAML in.  If you don't specify the right picture location, you can get warnings a build time about unexpected files because they are int he wrong location.  The other issue with this is that, if you use 'pkgdown' to build a package documentatino website, it won't pick up the pictures properly (see next section).

## README file

Include a README.md file in the top level of your package

## Unit testing and Code coverage

## Checking you `R` package

## Process for release

## Licencing