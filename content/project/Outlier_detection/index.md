---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Anomaly Detection in Time Series using R"
summary: "Identifying and predicting anomalies in time series is crucial for decision making. So, we are going to use an option in R for doing the work."
authors: []
tags:
- Anomaly Detection
- Unsupervised Algorithms
- Time Series
categories: []
date: 2020-03-17T16:53:01-06:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
links:
- icon: github
  icon_pack: fab
  name: Repository
  url: https://github.com/cconejov/Anomaly_Detection_TS

url_code: ""
url_pdf: "files/Report_Anomaly_detection_TS.pdf"
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
Currently, a lot of processes cause information that can be gathered as time series. Predict anomalies in the observations also is crucial for determining changes in business patterns and decision making. Identifying those events in time series is usually complicated, so package like [anomalize](https://cran.r-project.org/web/packages/anomalize/index.html) in [R](https://cran.r-project.org/) brings effective
solutions for identifying outliers observations. In this exercise, we use this package for detecting anomalies in the price of [Tesla](https://www.tesla.com/) shares from January 2019 to March 2020.
