---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Cenovus Energy"
summary: ""
authors: []
tags: []
categories: []
date: 2020-07-23T17:00:55-07:00

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

# Modelling Canadian Heavy Crude Congestion pricing using Capacitated Transport networks

## apacitated Transport networks

#### Problem Proposal:

Alberta produces \~4MM bbls/d of crude oil of which \~3 MMbbls/d is
considered "heavy oil". Majority or 2/3 of Canadian heavy oil is
consumed in PADD II and 1/3 in USGC refining center. The PADD III or
USGC is considered a marginal consumption point for Canadian crude where
the "last barrel" or marginal barrel is being consumed. Canadian crude
can reach USGC through number of pipe options: Enbridge mainline,
Express, and Keystone, or rail from either Edmonton or Hardisty. The
cost of transport of the last barrel from Alberta to USGC is going to
set the price of Canadian heavy benchmark (WCS) in Alberta.

Pipe is considered a cheapest mode of transport of Canadian crude to the
demand markets. The total offtake capacity from Alberta is on average
less than the total available production. This leads often to the
requirement of "call on rail" or shut-ins to balance the market which in
turn leads to significant price response.

Prices are generally integrated if they respond to same price shock. In
reality looking at USGC-Alberta spread pricing we see a regular
breakdown of the price relationship or "congestion pricing". This is due
to the fact that transient "sub-markets" can be form in a capitated
transport system.

The question is using stochastic transport optimization (following
similar method as reference [^1] and [^2]) can we model and answer the
following questions:

1.  When there are documented disruptions in the transport system can we
    predict how large the congestion surcharge was and how did prices
    respond to the disruption?

2.  Can we predict the occurrence of congestion by perturbing input
    factors in the system?

3.  How does shape and connections in the transport network contribute
    to the propensity for frequency of the congestion and magnitude of
    congestion surcharge?

There is a fantastic work performed looking at US gasoline market that
can be used as a guide and starting point to look at the Canadian crude
oil transport network.

The majority of the data: (1) Pipe Tolls and Tariffs (2) Capacities (3)
Supply and Demand factors are publicly available. (4) Pricing data and
some of the historical flow data that is used for benchmarking and
testing the models can be made available with some degree of
modifications and can be anonymized.

#### References

[^1]: Price Integration in Competitive Markets with Capacitated Transport Networks [PDF]

[^2]: Spatial Price Integration in Competitive Markets with Capacitated Transport Networks Master Thesis [PDF]

