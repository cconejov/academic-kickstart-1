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
  url: https://github.com/cconejov/Surv_Analysis_HDD
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
# Abstract

The branch of statistics that study the expected duration of time for an event to occur is called survival analysis. The number of events can be one or more.  This project reviews nonparametric methods like Kaplan-Meier, Nelson-Aalen, and Cox proportional hazards model. These techniques are applied to the Hard Drive data sets of [Backblaze](https://www.backblaze.com/). This application of survival analysis is called _failure-time analysis_.  In this way, the goal is to find the survival probabilities of the hard disks using the data collected by [Backblaze](https://www.backblaze.com/b2/hard-drive-test-data.html) in 2019.  With the raw data, we create new variables for applying survival models. The major package used for this exercise is [survival](https://cran.r-project.org/web/packages/survival/index.html). For the number of files, it also uses [data.table](https://cran.r-project.org/web/packages/data.table/index.html) package.

# Summary

 The global number of hard disks observed during 2019 was 131 448 observations and the number of hard disks with failure was 2 211.

The observations are left truncated and right censored. The distribution of age and study time by fail is:
{{< figure src="1_age_fail_hd.png" title="" lightbox="true" >}}

We can perceive how the density of fail increases until reaching the first year of operations. We can also appreciate the few values from the end of the expected life of hard drives.

We applied the techniques for measuring the survival probabilities:

* Kaplan Meier

* Nelson Aalen

Both methods gives similar values, as you can see in the following figure:
{{< figure src="3_plot_diff_na_ka.png" title="" lightbox="true" >}}

As a result, the survival probabilities are:
{{< figure src="2_plot_na_km.png" title="" lightbox="true" >}}

Therefore, we can conclude that there is more than a 90% probability that a hard disk will reach its estimated useful life of 1825 days.

On the other hand, using the package [simPH](https://cran.r-project.org/web/packages/simPH/index.html), we can build a simulation of the relative hazard based on a comparison with a median age of 497 in hard disk using Cox regression.

{{< figure src="4_simPH_Age.png" title="" lightbox="true" >}}

As a result, there are more probabilities to fail during the first 497 days. In conclusion, the simulated relative hazards for ages below the median are more than one. This means that hard disks are more likely to fail at a given point in time than hard disks that have worked for 497 days.
