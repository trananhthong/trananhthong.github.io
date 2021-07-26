---
title: COVID-19 Impact on Credit Loss Modelling
author: Thong Tran
date: 2021-06-07 12:00:01 +0200
categories: [Project, Aalto]
tags: [merton-vasicek, quasi moment matching, credit risk, covid-19, optimization, python, torch]
math: true
---

## Background

The COVID-19 pandemic and the measures from governments to alleviate its effects has created complicated economic conditions. As a result, conventional models such as the single-factor Merton-Vasicek (MV) model for estimating credit risk have failed to reliably predict the probability of default (PD) in the recent years. The project aimed to provide a more robust method for PD prediction that can account for complex condition such as those of during the pandemic. The project was done with data from [SEB](https://seb.se/) and [GCD](https://www.globalcreditdata.org/).

## Approach

The single-factor MV model only considers a single economic factor to predict the performance of a large and diverse portfolio. Therefore, it cannot fully account for the variations of the PDs of companies of different sectors and ratings under complicated conditions. To address those issues, the following was proposed:
- Employing the multi-factor MV model,
- Using a broader set of economic factors,
- Applying the MV model at rating and sector level.

## Implementation

As there were different data sources involved, a data pipeline was created to standardize the data from both SEB and GCD rating migration datasets and integrate economic data from open data sources. The multi-factor MV model was implemented and optimized using `PyTorch`. SEB data was used as the test portfolio to measure the performance of different combination of models and economic factors.

## Additional Resources

More details and final results of the experiments can found in the [final report](/assets/doc/sebcreditrisk.pdf). The source code of the project can be accessed [here](https://github.com/trananhthong/sebcreditrisk).
