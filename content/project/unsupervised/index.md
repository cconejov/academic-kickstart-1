---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Unsupervised Algorithms"
summary: "In this project, we review two methods of unsupervised techniques: k-means and hierarchical clustering."
authors: []
tags:
- Machine Learning
- Unsupervised Algorithms
- Clustering
categories: []
date: 2020-03-08T21:44:22-06:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Image credit: [**quoracreative.com**](https://quoracreative.com/article/machine-learning-marketing-Sales)"

  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
links:
- icon: github
  icon_pack: fab
  name: Repository
  url: https://github.com/cconejov/clustering

url_code: ""
url_pdf: "files/Unsupervised_Algorithms.pdf"
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
This project provides some examples of unsupervised algorithms in machine learning. In these techniques, we need to infer the properties of the observations without the help of an output variable or _supervisor_. We review two methods: k-means and hierarchical clustering. Then we use
some data from [Kaggle](https://www.kaggle.com/arjunbhasin2013/ccdata)  for applying these techniques to produce a customer segmentation. The platform that we use is [R](https://cran.r-project.org/). Because of the number of observations, we are going to use a parallel process for improving the execution times using the [snow](https://cran.r-project.org/web/packages/snow/index.html) package.
