---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Fotech Solutions"
summary: "Consider a distributed acoustic sensing (DAS) system monitoring a
fibre optic cable deployed along an active roadway. The goal of this project is
to use data collected from the DAS system to develop a detection and tracking
method capable of identifying individual vehicles and reporting their position
and velocity as they move along the road/fibre.  Once the position and velocity
are determined, various metrics for traffic flow could be determined, allowing
for prediction and optimization of traffic congestion."
authors: [fotech]
tags: []
categories: []
date: 2020-07-23T16:58:50-07:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Figure 1: DAS response showing multiple vehicles travelling along a fibre optic cable"
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
math: true
---

# Traffic monitoring with distributed acoustic sensing

### Industry Mentor: Matt McDonald, Chief Technology Officer, Fotech Solutions

#### Problem Description

Consider the application of distributed acoustic sensing (DAS) system monitoring
to a fibre optic cable deployed along an active roadway. Traffic on
the roadway causes mechanical deformation of the ground which strain the
fibre optic cable, causing phase shift in the backscattered light measured by
the DAS system. Figure 1 shows the system response as traffic moves along
the fibre optic cable.

Analysing a subset of the data in window in space-time allows individual
vehicles to be recognized. Transforming this data into the time-slowness
($\tau−p$) domain using a Radon transform then admits a representation suitable
for counting the number of vehicles present in the frame and identifying
individual velocities using standard peak-detection methods. Figure 2 shows
a subset of data with four vehicles travelling in the positive direction at
different velocities and the Radon transform of the data showing four peaks
isolated in the ($\tau − p$) domain, each labelled with its associated velocity.

{{< figure src="./fig2.png" title="Figure 2: (Top) Four vehicles travelling along a fibre optic cable at different speeds. (Bottom) $\tau − p$ domain representation of traffic response showing time offset and apparent slowness." >}}

The proposed problem, is to develop a detection and tracking method
capable of identifying individual vehicles and reporting their position and
velocity as they move along the road/fibre. Furthermore, once the position
and velocity is determined, various metrics for traffic flow could be
determined, allowing for prediction and optimization of traffic congestion.
