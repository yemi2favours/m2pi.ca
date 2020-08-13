---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Mcmillan Mcgee"
summary: "The goal of this project is to develop a reasonably accurate and
affordable design tool to model the performance of McMillan-McGee's patented
induction heaters, which are used for thermal conductive remediation of
contaminated soil.  A good design tool would be useful to assess the feasibility
and cost of using different heater lengths, diameters, and materials. 
Working knowledge of Maxwell's equations, vector analysis, boundary value
problems, Green's functions, complex variables, contour integration, residues,
integral transformations and differential equations would be essential
background for this project."
authors: [reid, bahri, rjt128, antoniatcenko, noahbolohan, AliRY95]
tags: []
categories: []
date: 2020-07-23T16:58:18-07:00

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


#  Simulating cylindrical induction heaters with helical electrical conductors

### Industry Mentor: Edwin Reid, Director of Electrical Technology, McMillan-McGee Corporation

#### Brief Description of the Problem

Here is a brief description of McMillan-McGee's (MC<sup>2</sup>) patented
induction heaters used for thermal conductive remediation of contaminated soil.
Without delving into the science of soil remediation, which is beyond the scope
of work, it is sufficient to say that a heater unit consist of a hollow steel
cylinder that is equipped with an internal electrically conducting helix that
runs inside the lateral extent of the cylinder.  The cylinder, called the
casing, is a 6-inch inner diameter carbon steel pipe, with wall thickness from
1/4 to 1/2 inch. The helix, called the work coil, is made from a very long piece
of copper or nickle bus bar stock with a rectangular cross section 1/4 inch
thick by 1 inch wide.  A stainless steel frame frame supports the work coil on
ceramic insulators that electrically isolate the work coil from both the frame
and casing.  The heater unit is essentially a transformer where the work coil is
the primary, and the casing, the secondary. In this construction, the casing
forms a single-turn short circuited secondary.  Heater units can have a length
from one to ten meters and these are buried vertically below ground level in a
volume of soil to be decontaminated.  Intense heat is usually needed to mobilize
contaminants trapped in the soil in order that these can be extracted and
disposed by certain processing equipment.  A typical field installation consists
of a multitude of heaters, which are spaced a few meters apart and arranged in a
repeated triangular pattern.  Heat is transferred from heaters to the volume of
soil solely by thermal conduction.

The purpose of the work coil is to induce circumferential eddy currents on the
inner wall of the casing.  These currents flow against the resistance of the
casing thereby generating heat, whereby, the casing transfers its heat  to the
soil.  Induction heating is not a new technology, which has been used in
foundries since 1910; however, it is a new technology to the soil remediation
industry.  In light of this McMillan-McGee Corporation have developed heaters
and an electronic generator, called an inverter, which supplies high frequency
alternating current to the work coil.

The inverter accepts three-phase 60 Hz low voltage (up to 600 volts is
considered to be low voltage in the power system trade) current drawn from the
utility, converts this to direct current with a rectifier, then regenerates the
current at a much higher frequency.  This is exactly what Danfoss variable
frequency drives do; however, our inverters supply current to work coils at a
much higher frequency.  Our inverters can supply alternating current to work
coils over the frequency range 7.5 kHz to 15 kHz.  Work coil current is
typically 80 to 100 Amperes and up to 50 kW can be drawn from one inverter.  The
purpose for the high frequency is two-fold: first, the work coil is constructed
from bus bar stock which has an appreciable pitch thereby resulting in a low
mutual inductance.  The work coil looks like a barber poll.  In order to induce
significant voltage on the wall of the casing using a work coil with low mutual
inductance will require a high frequency; this is by virtue of Faraday’s law.
Secondly, the wall of the pipe is very thick so operating on low frequencies
result in current occupying the entire wall thickness thereby forming an
extremely low resistance, thus a short circuit.  The steel casing does have
appreciable resistivity and magnetic permeability which can be used to an
advantage under certain operational conditions in order to establish appreciable
resistance against eddy currents to generate heat.  One way is to limit the
depth of penetration of current in the wall of the casing by exploiting the so
called skin effect.  To do this will require operating on a sufficiently high
frequency,, which is by virtue of the skin effect.  It is important to bear in
mind that the internal temperature of the heater can reach above 800C; and as
such, the electrical and magnetic properties of the heater unit will change with
temperature.  Thus, the problem itself is inherently a function of temperature.
Therefore, specification of material parameters is subject to their operating
temperature.  In light of this, we can still treat this problem as a constant
temperature one as long as we specify the heater temperature.

We seek is a reasonably accurate and affordable design tool as stated in the
above paragraph.  Certainly, finite element simulators such as Comsol
Multi-Physics and others can be used to tackle this problem, but these impose
two burdens: first simulators are expensive; secondly they are time and computer
memory intensive when analyzing practical problems.  There may be free software
available, but much work is needed to adapt them to suit our purpose.  Therefore
I am looking for a closed form solution that can be executed with a Matlab to
deliver timely and accurate results.

#### Why is the problem of interest?
I am often asked to assess the feasibility and associated cost on using
different heater lengths, diameters, and materials for prospective clients.  The
results of analysis using a good design tool would be useful to support my
assessment comments.  Presently, I comment with reservation, unless backed by
experimental results.  Often responses are called for which must be handled in a
short time frame.  In light of this, I would like assistance in further
developing the work in John Young's Journal paper that was published in the IEEE
[^1] almost two decades ago.  A similar approach is also found in a IEEE
technical monogram [^2]. Both approaches construct a good model of the problem
and apply will known mathematical methods to arrive at a solution which can
easily coded in Matlab and rapidly executed on a computer.     I favor these
approach and would like to extend the work to include the effect of Joule
heating on the casing.  I have started working on developing a solution but have
not reached one that .  I'm satisfied with because it lacks rigor.

#### What kinds of data are available?
Experimental data for different heater lengths is currently available.  Also, my
treatment of this problem by an elementary approach, which apparently works.

#### What would a solution to the problem look like?
The solution would be in the form of a Thevenin equivalent circuit (series
connected resistor and inductor) for a work coil in casing.  The problem can be
simplified when we relax the wave propagation requirement, thus reducing the
solution to one representing diffusion

#### What background knowledge would be needed
A good working knowledge of Maxwells equations [^3].  Vector Analysis, Boundary
Value Problems [^4], Green's Functions.  Fluency in Complex Variables, Contour
Integration,  Residues, Integral Transforms, and differential equations. 
 
#### References

[^1]: John C. Young and Chambers M. Butler, Inductance of a Shielded Coil, IEEE Transactions on Antennas and Propagation, Vol. 49, No. 6, June 2001
[^2]:  Donald G. Dudley, Mathematical Foundations for Electromagnetic Theory, IEEE Press,  1994
[^3]:  Dale Corson and Paul Lorrain, Electromagnetic Fields and Waves,  W.H. Freeman and Company, 1962
[^4]:  Hans Sagan, Boundary and Eigenvalue Problems in Mathematical Physics, Dover Publications Inc. 1961

