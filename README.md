# cnn-stock-image-analysis

Prices contain subtle and complex patterns that are difficult to detect with the standard methods of empirical finance. This set of code consider price trend patterns from a machine learning perspective.

Replication from paper: (Re-)Imag(in)ing Price Trends, Journal of Finance

## Table of Contents
- [Background](#background)
- [Dataset](#dataset)
- [Requirement](#requirement)

## Background

Why do we use CNN? From a machine learning perspective that applies to find price trend pattern, there is two prevailing concerns (from paper (Re-)Imag(in)ing Price Trends):
- We want a method that is flexible in order to find potentially complex predictive patterns.
- We also want a method that is interpretable (means that it should be constrained enough).

That is why this set of repo tries to replicate the following:
1. Represent historical prices as an image: mainly use for CNN, also help the model to focus on relational attributes.
2. Model the predictive association between images and future returns using CNN: image smoothing, feature extraction automation.

## Dataset

Current dataset that applies for this repo: U.S. stock returns from 1993 to 2019, and the CNN model is trained to predict the direction (up or down) of future stock returns.

## Requirement
Image Width: 
- for 5 days, it should be 15
- for 20 days, it should be 60
- for 60 days, it should be 180

Image Height:
- for 5 days, it should be 32
- for 20 days, it should be 64
- for 60 days, it should be 96

More information can be found at: [Dacheng's Xiu Website](https://dachxiu.chicagobooth.edu/download/img_demo.html)

