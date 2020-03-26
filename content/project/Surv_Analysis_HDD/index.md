---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Survival Analysis: Hard Drive Reliability Sample"
summary: "Nonparametric methods such as Kaplan-Meier and Nelson-Aalen is applied to the Hard Drive Data of Backblaze."
authors: []
tags:
- Survival Analysis
- Nonparametric Modeling
- Other
categories: []
date: 2020-03-25T17:17:04-06:00

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
  url: https://github.com/cconejov/purchased_Bike
url_code: ""
url_pdf: "files/Report_Surv_Analysis_HDD.pdf"
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
The branch of statistics that study the expected duration of time for an event to occur is called survival analysis. The number of events can be one or more.  This project reviews nonparametric methods like Kaplan-Meier, Nelson-Aalen, and Cox proportional hazards model is applied to the Hard Drive of [Backblaze](https://www.backblaze.com/) in the context of _failure-time analysis_. In this way, the goal is to find the probabilities that the hard disk works well for 1 year using the data collected in 2019. The package used for this exercise is [survival](https://cran.r-project.org/web/packages/survival/index.html). For the number of files, it also uses [data.table](https://cran.r-project.org/web/packages/data.table/index.html) package.

Work in Progress.
