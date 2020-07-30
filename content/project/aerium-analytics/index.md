---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Aerium Analytics"
summary: ""
authors: [""]
tags: []
categories: []
date: 2020-07-23T16:57:49-07:00

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
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

#  Automated region of interest creation for training sets

### Industry Mentor: Heather Hardeman-Vooys, Machine Learning Developer, AERIUM Analytics



Standard procedure for building training sets for some machine learning models involves an individual going through hundreds of images and creating 2D binary matrices which reflects where the region of interest is in each image. Depending on the type of images, can we use RGB information or some other method to automate this process?  The goal of this project is to develop a method which creates a mask of an image depicting where monochromatic objects occur in an image automatically and with limited user input.
