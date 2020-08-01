---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Ovintiv"
summary: "In March 2020, the WTI futures contract settled below zero for the
first time in the contract's history.  Many market participants apply the Black
76 model or a variation of this model to calculate the value of the options on
this futures contract.  However, Black 76 requires positive underlying market
prices.  The goal of this project is to identify alternative models which can
accept negative underlying pricing, and assess the suitability of the
alternatives. People interested in quantitative finance, commodity training and
marketing, and bridging the gap between quantitative experts and non-experts
would be excellent team members for this project."
authors: []
tags: []
categories: []
date: 2020-07-23T16:58:02-07:00

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

# Practical Option Valuation with Negative Underlying Prices

### Industry Mentor: Scott Dalton, Director of Risk Management, Ovintiv

In March 2020, the prompt month [WTI futures contract](https://www.cmegroup.com/trading/energy/crude-oil/light-sweet-crude_contract_specifications.html)
settled below zero for the first time in the contract's history. Many
market participants apply the [Black 76 model](https://en.wikipedia.org/wiki/Black_model)
model or some variation when calculating the value of the options on
this futures contract as a relatively straightforward, parametric
valuation method. This calculation model is hard wired into many
[Commodity Trading and Risk Management Systems](https://iongroup.com/ion-commodities/products/). Traders and
risk managers rely on its straightforward and reproducible output.

However, Black 76 requires positive underlying market prices. The
negative prompt month settlement price caused considerable consternation
among energy traders and risk managers.

More generally, OTC options are also available on basis or differential
prices. These transactions are options on the difference between two
published indexes such as NYMEX Henry Hub and AECO (for natural gas) or
Cushing WTI and Houston (for crude oil). As such, these instruments
frequently have negative underlying market prices.

While commodity producers, processors, transporters and consumers
frequently use derivatives to hedge their underlying physical exposures,
many of these organizations do not maintain significant quantitative
expertise in-house. Being able to perform this type of analysis and then
explain the approach and results to non-quant specialists is a useful
and valuable skillset.

#### The task

-   Review available alternatives to Black 76 for valuing
    commodity-based European options.

-   Identify alternatives that can accept negative underlying pricing
    (Bachelier is one example).

-   Assess the suitability of alternatives in terms of:

    -   Ease of use

    -   Validity of assumptions

    -   Reasonableness of results

    -   Proximity of results to Black 76 when underlying market prices
        are positive

-   Identify recommended alternative(s)

#### Student background

People interested in applied quantitative finance, commodity trading and
marketing, and bridging the gap between quantitative experts and
non-experts.

A sample market data set will be available that includes historical
forward market prices, implied volatilities or option premiums, risk
free interest rates
