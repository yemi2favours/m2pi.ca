---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "BC Financial Services Authority"
summary: "The goal of this project is to develop a housing price
estimate/forecast using publicly available data to inform evidence-based
decision making for the benefit of government regulators, industry
practitioners, and concerned citizens.  

Students will be expected to use Python 3.X for data acquisition, cleaning,
organization, and manipulation.  Working experience with libraries such as
Pandas may be useful.  Previous experience with other programming languages such
as Matlab or R is useful but not required."
authors: [dong, moosvi, danieldibenedetto, yiwei, leimin23]
tags: ['2020']
categories: []
date: 2020-07-23T16:59:33-07:00

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

final_report: 'BCFSA-final.pdf'

---

# Housing price estimates/forecasts for BC real estate markets

### Industry Mentor: David Dong, Senior Analyst, BC Financial Services Authority

#### Disclaimer

The opinions as stated in this outline do not represent the opinions of
the organisations that I work for and/or with. In addition, all data
that is used in this project is open-sourced; no privileged data is used
in the project.

#### Expectation of outcome

It goes without saying that the Real Estate sector represents one of the
most important economic activities in the province of British Columbia.
In recent years, it has also attracted media spotlight and public
attentions as housing prices spike as well as the development of topical
issues such as Public Housing and Strata Insurance. All these have
generated a high demand for better understanding of the Industry's
operational mechanism and driving factors. This project can be
considered as a further step towards more evidence-based decision
making, for the benefits of government regulators, industry
practitioners, and concerned citizens.

Housing price estimate/forecast is not a new thing. Zillow's
Zestimate[^1] and Kaggle[^2] competitions on Housing Prices are two of
the better-known venues of such effort to address public concerns on
Housing issues by scientists/engineers' communities. All these estimates
have commonalities for practical reasons. For the end users of an
estimate, relevant information would include

1. Explanatory variables such as property-specific features (\# of
bedrooms and bathrooms for example) and other driving factors (e.g.,
demographic information, average household income in the area or
mortgage rates)

2. An interpretable model. Earlier models were mostly similar to
regression of some kind for this reason. Recent black-box machine
learning models can have interpretability issue.

3. Some form of estimate or forecast of property prices either in the
future or in areas with comparable driving factors.

It is to be noted that some of previous efforts have used Root Mean
Square Error (RMSE) as measurement for the accuracy of estimate. We can
use that as well.

**Why this is an interesting to public sector**

Consider a hypothetical scenario where there has been an economic
downturn in the Province. Unemployment is up and businesses are shut
down. A financial industry regulator would be concerned with where the
Housing market goes because real properties represent a significant
portion of Financial Institutions' business and therefore their risks.

Consider a hypothetical scenario where a minor Flood or Earthquake just
hit a populated municipality. The Mayor and city Councillors would want
to find out the indirect economic impact of the natural disaster.

#### Data

**Data Sources**

The first type of data to consider would be the geographic boundary data
in the Province. It can be found from the Statistics Canada API or
website.

The second source of data is the property valuation information. It
contains the valuation of land and improvement valuation of each parcel
in the studied area. Historical annual information can be sourced all
the way back to the year of 2006.

The third source of data is the demographic information from Statistics
Canada.

As the modeling goes deeper, the project team may find it interesting to
explore deeper. This is where information on school district, local
health care-related information, traffic surveillance, historical police
report can become worth studying.

#### Expectation of students

**Data skills**

Data can be acquired either through API requests or by downloading CSV
files. Students will be expected to learn to use Python for data
acquisition, cleaning, organization, and manipulation. If the project
continues beyond the length of the boot camp, it is reasonable for the
students to learn the basics of data integrity and data governance.

**Tools and programming languages**

Students are expected to program in Python 3.X. Working experiences with
libraries such as pandas can be useful. Previous experiences of other
programming languages such as Matlab or R can be useful but is not
required.

No previous knowledge of database management or operation Is expected.

[^1]: <https://www.zillow.com/blog/zestimate-updates-230614/>

[^2]: Such as here: <https://www.kaggle.com/c/boston-housing/overview>
