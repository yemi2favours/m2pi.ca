---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Divi Project"
summary: "The main limitation of blockchains is storage requirements, which
would be alleviated if one could reversibly compress the data in a blockchain or
in its underlying transaction graph. Determine to what extent a transaction
graph can be compressed (for later decompression) or what obstructions exist to
its compression. What compression ratio can you achieve for an ordered sequence
of cryptographic hashes? Pure Mathematics skills and experience with
mathematical proof-writing are essential skills for this project.  Knowledge of
undergraduate-level cryptography or Python programming skills would be assets,
but are not required."
authors: ["pattiaroy","akcora"]
tags: []
categories: []
date: 2020-07-23T17:00:22-07:00

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

# Compressibility of the transaction graph for the proof-of-protocol in a blockchain

### German Luna Patiarroy, Lead Blockchain Developer, The Divi Project

Present-day societies are facing an ever-increasing adoption of
cryptography-based currencies (aka. crypto-currencies) developed atop the
concept of a blockchain - a collection of “blocks” each committing to other
“blocks” providing an immutable history of transactions that can be replicated
in a permissionless fashion. In spite of the importance of blockchain
technology, not a lot of work has been done on trying to improve the main
limitation of blockchains: storage requirements. Most work trying to address
this problem has focused on reducing the storage footprint of future data.
However, this doesn’t fundamentally solve the problem that ever-increasing
amounts of storage space will be required.

A blockchain consists conceptually of 6 systems:
* Data System (the shared data between the users of the blockchain)
* Communication System (the mechanisms of communicating data)
* Consensus System (the rules of the blockchain dictating what modifications of
  the data layer are and are not allowed)
* Incentive System (the incentives or rewards that can be claimed by users)
* Proof of Permission (the requirement for some modifications of the data system
  to be accepted)
* Proof of Protocol (the proof that the protocol has been followed)

The computer network that maintains a blockchain operates by (1) sharing data
through the communication system, (2) validating the rules of the consensus
system have been correctly applied to the communicated data, (3) verifying the
provided and applicable proofs, and finally (4) updating their local copy of the
blockchain accordingly.

Among the many components that a blockchain has, one of the most important ones
is the ‘proof-of-protocol’. A piece of data that can automatically prove to any
(reasonably capable) person that the protocol has been followed. Satoshi’s
(Bitcoin creator) solution to this problem was to encode the data as blocks in a
chain, hence the name blockchain.  However, this begs the question about whether
it’s possible to reversibly compress the data in a blockchain or whether we
should buy stock in data storage companies and begin hoarding petabyte drives.

Although the main data structure of a blockchain is the chain of blocks, a more
fundamental and underlying data structure is the transaction graph. In a
financial context, the links represent the relation between spent coins and
their new owners.  These contain the proofs of permission.

#### Problem Statement
* Determine to what extent a transaction graph can be compressed (for later
  decompression) or what obstructions exist to its compression.
* What compression ratio can you achieve for an ordered sequence of
  cryptographic hashes?

#### Pre-requisie Knowledge
##### Required
* Pure Math
* Mathematical proof writing
##### Nice to Have
* Undergraduate level Cryptography
* Python programming (to write any prototype code or provide simulations and
  illustrations as needed)
