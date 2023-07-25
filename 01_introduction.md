---
title: Introduction
numbering:
  enumerator: 1.%s
---

Prior to the invention of global positioning systems (GPS), humanity relied mainly on accurate cartography to optimize navigation {cite:p}`council1995global`. Navigation by cartography was not only confined to terrestrial
travel, but extraterrestrial travel as well through the knowledge of
celestial orbits of the moon and planets {cite:p}`gehrz2007nasa`. Yet, even the most detailed maps eventually became outdated and possibly misread or misinterpreted depending on the level of spatial awareness of the
traveler. The advent of GPS in 1973 eventually brought about a
revolution among travelers for ease of use, but more importantly for the
confidence, it instilled in that no matter how complicated the route, a
step-by-step guide was provided. A similar approach is needed for the
nanoscopic world of electron microscopy. A guide that provides
microscopists the ability to record where they have been in a sample,
and to develop roadmaps for themselves and others to assist in future
analysis. Those positions could be converted between microscopes if and
when the sample needed to be re-analyzed. Just as a physical road map
need be turned and flipped to compare to a landmark, fiduciary marker,
or reference position, so too should electron microscopists have the
ability to flip and rotate positional data when moving a sample to a
different microscope.

Since the invention of electron microscopy {cite:p}`mulvey1996ernst, knoll1932elektronenmikroskop`, not only did the physical observation of microstructures
become important (e.g., shape, size, and morphology), but so too did
relating the crystallographic knowledge to those microstructures. The
spatial resolution of transmission electron microscopes (TEM) opened an
entirely new world as compared to X-ray and spectroscopic techniques. It
lead to the discovery and confirmation of deoxyribonucleic acid (DNA) in
the 1950s {cite:p}`watson1953molecular`, and is currently providing materials
researchers the ability to examine crystals atom-by-atom {cite:p}`meyer2008imaging` as well as to move atoms one by one to create larger structures at
the atomic scale {cite:p}`dyck2018building`. The push towards picometer
resolution a short 80 years after its introduction has been rivaled by
few technologies for volumetric analysis such as atom probe tomography
{cite:p}`blavette1993tomographic, cerezo1988application`. Yet, the ever-expanding
spectral, structural, and crystallographic techniques available in the
TEM still make it the most versatile and attractive analysis technique
for a wide range of research fields.

The ability to understand the crystallographic and microstructural
orientations of any region of interest within a TEM sample in relation
to the physical stage movements is crucial to extracting the most
concise and relevant information possible in the shortest amount of
time. The geometry and physics of extracting and understanding these
data have long been understood and published {cite:p}`duden2009k, klinger2015crystallographic, liu1994simple, liu1995simple, qing1989equation, qing1989calculation, zhang2018atomic`. Programs such as Desktop Microscopist[^1],
CrysTBox, ALPABETA, CrystalMaker, JEMS, τompas, SPICA, and K-space
Navigator provided a variety of ways to understand crystallographic data
{cite:p}`cautaerts2018alphabeta, klinger2015crystallographic, duden2009k, stadelmann1987ems, palmer2015visualization, degraef2012structure, xie2020tauompas, li2016spica`. In the conclusion of Liu's calculations on the
prediction of cubic crystals a statement was made that, "If an interface
between the microscope and the computer is developed, an automated
on-line method can also be developed..." {cite:p}`liu1994simple`. Others have
utilized stage positions and knowledge of crystalline poles to address
grain orientations, and more importantly grain boundary misorientations
{cite:p}`jeong2010characterization, liu1994simple, liu1995simple`. This research has been
widely available, but there is still not a concise, user-friendly manner
in which to fully utilize this knowledge for mapping out an entire
sample.

[^1]: Desktop Microscopist is a trademark of Desktop Microscopist

There is a need for increased speed and efficiency in electron
microscopy due to a wider field of materials being analyzed, an
increasing amount of analytical techniques being developed, higher
capital costs associated with purchasing newer instrumentation, and
decreased sources of funding {cite:p}`maia2018haves`. Current generation
spectrometers can be as costly as the base microscope itself. With the
revolution of aberration correction advancing resolution to the
picometer scale {cite:p}`yankovich2014picometre`, the inclusion of a corrector,
whether image or probe, has increasingly commonplace on all new
purchases. This increased technology has added to the steep costs of
doing innovative microscopy. These factors have made it such that each
minute spent in any microscopy session is precious. It has also made
collaboration and user facilities an attractive option for researchers
who do not have the capability to perform higher end research at their
home institutions. All of this taken into consideration, the future of
electron microscopy will be geared towards doing smarter microscopy and
automation {cite:p}`spurgeon2020towards`, similar to what has been
accomplished in the field of X-ray crystallography {cite:p}`abola2000automation`.
The eventual progression into full automation presents the possibility
of much of the underlying mathematics and physics being overlooked as
microscopes will eventually perform much of the data collection.

Automation and machine learning, while first pioneered and developed in
biological microscopy, is steadily being developed for materials science
applications {cite:p}`carter2019transmission, jansen2013towards`. The
genesis of automated detection and tomographic techniques within the
framework of understanding biological materials was born out of a need
for observing microstructural information over longer length scales,
such as counting cells {cite:p}`porter1945study, lidke2012advances`. The
complex nature of the electron interaction physics of material science
research such as crystallinity, defects, and variable Z contrast, makes
automation more difficult and most likely why it has slowed the adoption
and development in the field. This is not to mention the exceedingly
smaller length scales that become crucial to understanding any number of
atomic phenomena that control bulk materials properties.

As electron microscopy is a projection technique, there will always be a
conundrum in analyzing material properties in that the thinner the
sample becomes the more accurate the information collected (e.g.,
decreased multiple scattering); yet, the thinner the sample becomes the
less representative the information is of the entire bulk sample (e.g.,
only a thin slice of a three dimensional object is being observed).
Additionally, the thinner the sample the more questions of surface
effects dominating the analysis arise {cite:p}`carter2019transmission, findlay2010dynamics`. Machine and smart learning algorithms require
more demanding analytical image analysis techniques within the realm of
materials science {cite:p}`braidy2012correcting, jones2017optimising, jones2015smart, jansen2013towards`. To be able to position a sample to
understand specific **g** vectors, contrast changes, and orientation
effects requires more math than simple edge detection or shape
recognition. Even when algorithms are developed to address this, the
nature of relevant nanoscopic information within a finite sample
thickness (e.g., even with a sample being 40-50 nm thick) may hinder
their widespread acceptance. Therefore, there is still a need for the
materials science microscopist to interact and guide the collection of
data, and as such, there needs to be an intermediary that provides
microscopists with tools to better analyze and understand their data.

More importantly, due to a more an ever-increasing reliance on metadata
and digital capture, there has been less concentration on dictation and
annotation of data. Electron microscopy is becoming more of a tool than
a science, and although there are many programs to process and analyze
data, there are few that serve as a digital notebook. While at first
seemingly counter intuitive, current research into the human memory
suggests that the brain is less likely to remember captured data than
what is observed {cite:p}`soares2018forget`. This should seem familiar to
any microscopist in discussing microscopy sessions with collaborators in
that they "saw" additional features not apparent in the recorded data.
There is a need to develop programs that act as a prediction tool, but
as well a digital notebook.

Therefore, it is essential to have more accurate and directed electron
microscopy to provide a pathway in alleviating the increased demand on
current and future instrumentation. While there are inroads being made
into automation and machine learning, there will be an unfortunate gap
before the technology becomes available and even fiscally tenable {cite:p}`maia2018haves`. This paper provides a way to link together a long
database of crystallographic data and double tilt stage mechanics that
can be applied to any microscope, regardless of age or technological
advancement. The framework of this research is based upon many papers
and formulas of past electron microscopists, but it serves to combine
all these data as a different manner of thinking to make microscopy more
efficient and concise. This research will fully document how to best
utilize crystallographic and microstructural information in combination
with a double tilt stage to collect the most pertinent information, but
also provide a roadmap for future analysis or plan for analysis on a
different microscope. The protocol, which is being coined
nanocartography, provides insight on how to travel within any given
crystal system, quickly plot and solve the orientation of unknown
crystals with as little information as one diffracting plane, create
oblique tilt series, rapidly position interfaces on edge, relate
interfaces to adjacent crystallographic information, quickly understand
the tilt limits of each crystalline grain, and most importantly
translate any microstructural or crystallographic information collected
when reloading a sample or transferring the sample to a different
microscope. This goes beyond the broader description of
"nano-cartography" described in an editorial by Demming {cite:p}`demming2015nano`
describing instrument agnostic analysis at the nanoscale to understand
materials systems.

The advent of digital capture (first with charge-coupled devices (CCDs),
and more recently with direct electron detection), has provided
microscopists with a double-edged sword in terms of data {cite:p}`oxley2020deep, ophus2019four`. More data is always preferential, but it has
provided a false sense of information capture in the form of metadata.
The latent information that users typically believe is embedded within
each digital capture often means less meticulous note taking in the
belief all information is being transferred. The ability to capture
k-space, whether through diffraction or through the Ronchigram, affords
microscopists with an advantage in terms of not only knowing that the
data collected is correct (as say compared to oversaturation in film),
but more importantly the ability to digitally measure that information.

The basis of nanocartography is understanding the control and predictive
tilting of a double tilt stage in relation to the orientation and motion
of all crystal systems, in addition to the physical constructs within a
sample (such as grain boundaries and interfaces) and their relationship
to crystallographic orientations. The development of these formulations
have long been understood, but rarely, if ever, discussed with
relationship to one another {cite:p}`cautaerts2018alphabeta, degraef2012structure, duden2009k, hayashida2019parameters, hayashida2016practical, klinger2015crystallographic, li2016spica, liu1994simple, liu1995simple, qing1989equation, qing1989calculation, xie2020tauompas, moeck2006transmission`. Unfortunately, the wide breadth of literature on this subject has
failed to yield a complete picture that provides clear methodologies for
understanding and controlling the motion of samples using a double tilt
stage in a transmission electron microscope (TEM). The need to connect
the theoretical and practical into a single document is long overdue,
and this work serves this purpose but as well expands upon methodologies
inherent to more experienced microscopists. These latent data collection
techniques are most often considered best practices within individual
labs but rarely published. Incorporation into the context of
nanocartography became exceedingly relevant.

The following publication is divided into three major sections followed
by discussion and conclusions. The first develops mathematical concepts
of nanocartography, illustrating how vector analysis, TEM stage
movement, and crystallography can be combined to accurately navigate
sample analysis. The second portion utilizes the derivations from
section one to develop practical derivations for nanocartography,
including the use of digital capture to more accurately navigate a
sample as well as identification of grain boundary type. Finally, the
third section explores practical applications of nanocartography; how to
correctly calibrate stage motion as well as apply derivations from
sections one and two. Taken in whole, this Element serves as a rich
summary of optimization of TEM data collection and analysis.
