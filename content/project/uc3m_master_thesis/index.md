---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Master's thesis: Application of Convolutional networks in the Multiple Hypothesis Testing"
summary: "Site with the official pdf document and Python code of my thesis project for the master's degree in Statistics for Data Science. My thesis applies Convolutional Neural Networks (CNNs), a popular Deep Learning framework used for detecting patterns, especially in images and photos. But, instead of analyzing pictures, I am applying the CNNs in the context of statistical inference on high-dimensional data and Multiple Hypothesis testing."
authors: []
tags:
- UC3M
categories: []
date: 2021-09-21

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "UC3M master thesis in Statistics for Data Science"
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
links:
- icon: github
  icon_pack: fab
  name: Repository
  url: https://github.com/cconejov/Application_CNN_MHT_problems

url_code: ""
url_pdf: "files/TFM_Cesar_Conejo_Application_CNN_MHT.pdf"
url_slides: "files/TFM_PPT_Cesar_Conejo_Application_CNNs_MHT.pdf"
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

**Abstract**

Multiple Hypothesis testing consists of a series of statistical procedures for solving hypothesis tests on high-dimensional data marginally.  Several approaches have been developed for dealing with this statistical problem. Classical methods consist of defining and controlling a specific error rate. These methods usually rely on the p-values for collecting the evidence against the null hypothesis. Other alternatives have also been developed under a semi-supervised approach. In this case, we solve the large-scale testing using a null train sampling collected via endogenous or exogenous mechanisms.  In this project, we combine both approaches. Employing simulations, we explore the possibility of handling cases where the user knows and controls the ground truth for solving multiple hypothesis testing problems in a supervised framework. Starting with calibrated p-values under the null hypothesis, we represent the p-values in terms of odds, converting them into lower bounds of Bayes Factors.
Additionally, we take a step further, creating a matrix of the relative evidence among tests as the previously ordered minimum bounds quotients. This matrix representation is considered analogous to an image. With these ingredients, we train Convolutional Neural Networks to determine if this framework can detect the cases where the null hypothesis is rejected. We explore the ability of the CNNs to correctly classifying the hypothesis based on two primary examples. First, we study the efficiency of a diet applied to a female mice sample under several scenarios. Then, we explore the mean difference of two independent populations sampling from the normal distribution.
