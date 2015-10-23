---
title       : Ordinary Least Squares
subtitle    : Simulation App
author      : Cristian Santa
job         : statistician
framework   : io2012      # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow
widgets     : [mathjax]     # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
github      :
   user:cdsantae
   repo:OLSAppPresentation
---

## OLS

[Ordinary Least Squares](https://en.wikipedia.org/wiki/Ordinary_least_squares) is a method for estimating the unknown parameters in a linear regression model, with the goal of minimizing the differences between the observed responses in some arbitrary dataset and the responses predicted by the linear approximation of the data.

<style type='text/css'>
img {
    max-height: 400px;
    max-width: 600px;
}
</style>

![](App.png)
<script type='text/javascript'>
$(function() {
    $("p:has(img)").addClass('centered');
});
</script>

--- .class #id

## The App

In this App you will manipulate the dataset and fit model, change the options of the plot, as well as on/off the intercept of the model, change the proportional scheme, and Set Seed for randomly data.

The data is generating by two normal random variables like this.

<script type="text/x-mathjax-config">
   MathJax.Hub.Config({  "HTML-CSS": { minScaleAdjust: 120, availableFonts: [] }  });
</script>
<br>
$$x\sim N(0,\sigma_{x}+2)$$
<br>
$$u\sim N(0,\sigma_{u})$$

--- &twocol

## Models & Data Generating Process

*** =left
### Data Generating Process
$y=2+3x+u$
<br>
<br>
$y=2+3x-0.5x^2+u$
<br>
<br>
$y=-10-1.5x+x^2+u$
<br>
<br>
$y=-2x-0.5x^2+u$
<br>
<br>
$y=5+x-0.1e^{x}+u$
<br>
<br>
$y=0.2e^{x}+u10$
<br>
<br>
$y=-4-2x^2+0.4e^{x}-x^2+u^5$
<br>
<br>
$y=-1-2x+1.5x^2-1.5x^3-0.05x^4+10^{-4}x^5+u^5$

*** =right
### Fit Models
$y\sim x$
<br>
$y\sim x^2$
<br>
$y\sim e^{x}$
<br>
$y\sim x+x^2$
<br>
$y\sim x+e^{x}$
<br>
$y\sim x+x^2+e^{x}$
<br>
$y\sim x+x^2+x^3+x^4+x^5$ 

--- &vcenter

## Run The App

### Simulation OLS Application

# [Click Here](https://cdsantae.shinyapps.io/OLS_App)
