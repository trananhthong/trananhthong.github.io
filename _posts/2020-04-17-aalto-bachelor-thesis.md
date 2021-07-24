---
title: A Study on Approximate Bayesian Computation
author: Thong Tran
date: 2020-04-17 12:00:01 +0200
categories: [Project, Aalto]
tags: [abc, likelihood-free inference, python, data science]
math: true
image:
  src: /assets/img/projects/aalto_thesis.png
  width: 900
  height: 700
---

Approximate Bayesian computation (ABC) is a framework for inference that utilize simulations to bypass the need to explicitly calculate likelihoods. The project investigated the effects of factors such as summary statistics, distance measures, and dimension reduction on the performance of ABC. This was done by calculating the Wasserstein distance between the approximate posteriors produced by ABC and the true theoretical posterior. The experiments were implemented with Python [here](https://github.com/trananhthong/ABC), and more details of the experiments and the results can be found in the [final report](/assets/doc/Thesis_Aalto.pdf).
