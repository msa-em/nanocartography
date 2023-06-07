---
title: Discussion
numbering:
  enumerator: 5.%s
---

The ability to accurately control the stage motion with respect to
crystallography has long been a desirable function in any microscopist's
toolbox. While Desktop Microscopist was one of the first programs to
accurately predict diffraction patterns and measure relative stage
positions given a specific crystallographic information, others have
done similar plotting programs for a variety of applications. ALPHABETA
a was designed to accurately determine two beam locations for proper
dislocation and microstructural analysis of stainless steels {cite:p}`cautaerts2018alphabeta`. A number of papers have detailed the study of either the
double tilt stage and/or its relation to crystallographic analysis, but
the overwhelming majority have approached it from an a priori standpoint
of having specific crystallographic information {cite:p}`liu1994simple, liu1995simple, qing1989calculation, qing1989equation, cautaerts2018alphabeta, xie2020tauompas`. These approaches are applicable for navigating known crystals,
but the challenge for materials science is the unknown, especially at
the nanoscale. This necessitates an approach by which to consider not
only the stage motion for known crystals but unknown structures as well,
whether they be crystals or non-crystalline physical constructs
important to materials science (e.g., grain boundaries and interfaces).

The approaches detailed in this paper focus on breaking down the complex
nature of materials analysis using a double stage tilt mechanism into
distinct parts for ease of understanding and explanation; 1) a simple
vector analysis approach to explain the physical nature of a crystal as
opposed to defining it through diffraction, 2) the stage motion for
crystallographic vectors and for physical constructs such as interfaces
and boundaries, 3) the introduction of crystallographic analysis
converting the physical description of a crystal to reciprocal space,
and finally, 4) the use of the structure factor as a discrimination
filter to be applied on top of the physical description of the crystal
to illuminate the allowable planes/pole for a pre-defined crystal.

Taking each of these components as individual parts assists in
developing tools by which it becomes easier to create and develop maps
of the crystallographic orientations within a sample in addition to its
overall relationship to the sample. These tools can then be utilized in
a variety of manners to quickly and efficiently manipulate the sample,
and also plan for future analyses.

## Crystals as Physical Objects

In order to deconvolute what is often described as one of the more
difficult subjects in the conversion of materials science to electron
microscopy, namely crystallography in reciprocal space, the derivations
in this research focus on delineating the description of crystals as
real space objects from their description in k-space. These derivations
serve a dual function in that movement of a crystal in real space is
more intuitive than in reciprocal space, and it also assists in relating
the crystal to additional non-crystalline physical objects (e.g., grain
boundaries) and their motion using a double tilt stage. Much of the
published research regarding the use of a double tilt stage for TEM
analysis has focused solely on the motion of the stage, and very few
have combined it with its relation to crystals. As noted prior,
{cite:p}`cautaerts2018alphabeta`, Cautaerts et al. approached the use of a
double tilt stage to calculate the motion of a cubic crystal for use in
determining the optimal tilt conditions for two beam analysis. While
this provided more information than simple stage motion, it still did
not fully concern all crystal types.

The explanation of both the description of vectors of non-cubic crystals
and their motion is often confusing to inexperienced microscopists along
with a larger portion of materials scientists. The understanding of low
index poles and vectors is typically the extent to which most curricula
extend. Even in many prominent electron microscopy textbooks, the
measurement of angles between planes is provided as a series of
equations confined to a given system. This further serves to shroud the
explanation of systems more complex than cubic.

By first showing the conversion of all systems to cubic and then
demonstrating that vectors are transformed in real space provides a
clearer, more manageable pathway towards more complex analysis in
reciprocal space.

## Stage motion of Crystallographic Vectors and Non-Crystallographic Structures

This research illustrates a logical method by which to convert all
crystallographic systems to a cubic system, and then demonstrate
systematically how the motion of any vector occurs through a double tilt
stage. Building upon these mathematical operations, the motion or
pathways between vectors could also then be calculated. Finally, using
similar mathematics of plotting planes of atoms, the motion of
non-crystalline physical objects such as grain boundaries, surfaces, or
matrix/precipitate interfaces could quickly be defined. The power and
flexibility of considering crystals and their motion in real space is
demonstrated when they could then be related back to
non-crystallographic objects within the sample.

Grain boundary and interface analysis are key components in assessing
the nanoscale properties of a material to further explain bulk
properties (e.g., micromechanical, thermoelectrical, electronic).
Therefore, correct orientation (i.e., on-edge) of grain boundaries for
chemical analysis becomes imperative for proper investigation. Equally
important, although often overlooked, is the crystallographic
relationship of crystals to these interfaces. This is often relegated to
more automatic detection/analysis approached such as EBSD in SEM because
of its ease of use {cite:p}`wilkinson2012strains, alam1954high, venables1973electron, harland1981accurate`. Unfortunately, the
deeper understanding of these programs more so than the general meaning
of inverse pole figures (IPFs) is taken for granted. Having a manner by
which to orient interfaces and then quickly relate their orientation to
adjacent crystallographic objects provides for more thorough analysis
opportunities during a session. Newer technologies such as precession
electron diffraction and 4-D STEM {cite:p}`ophus2019four, ghamarian2014development` will speed up these analyses, but similar to EBSD, they lack the
ability to take into account the physical description of surrounding
non-crystalline objects such as grain boundaries.

Additionally, the ability to describe the full stage motion with respect
to these objects also provides a pathway to understand their
three-dimensional structure within the confines of the foil. To date,
electron tomography plus atom probe tomography provides the highest
three-dimensional spatial resolution (even considering a multitude of
artifacts) of materials within the spectrum of analytical materials
science analysis tools. For all of the advantages these techniques
provide, the major drawback is their extremely localized view of the
sample. This tradeoff can be detrimental to a more representative
analysis of the sample as a whole, but as well can be costly and time
consuming. Using the double tilt stage to tilt samples about any given
axis allows microscopists to tell a more complete story of the sample,
even within a 50-100 nm volume without having to remove the sample and
orient to a logical axis (e.g., α tilt). This motion, when combined with
the knowledge of the surrounding crystal, becomes even more important.

Lastly, having the orientation solution of any possible grain within a
sample allows for a number of discriminatory actions by a microscopist.
If the local orientation of any neighboring ZA or pole is mapped, it can
then be compared to the tilt stage limit. Depending on the desired
crystallographic orientation, it may not be possible to achieve said
orientation within that tilt range. As has been previously demonstrated,
with the location of a few zone axes, the coordinates of the principle
axes can be accurately calculated {cite:p}`liu1995simple`. The comparison of the
principle axes of two neighboring grains can then be utilized) to
calculate the location misorientation and the axis of misorientation
that then leads to grain boundary type. Again, future development of
scanning diffraction techniques will eventually automate this analysis,
but the basic knowledge and understanding of this technique will assist
in demystifying the often black box approach to their use.

## Crystallographic Analysis/Conversion to Reciprocal Space

The description and understanding of crystals as real space objects
defined by vectors and vector motion is the first step in developing a
more logical pathway for materials scientists and electron
microscopists. The additional step, which can then be finally utilized
to develop a mapping filter, is to describe crystals within reciprocal
space. The latent introduction to reciprocal space is often performed
through the preliminary description of Miller indices to describe planes
of atoms. This is typically accomplished through utilization of inverse
nomenclature, but then drawn as a real space object. This can lead to
confusion as to the crystallographic conversion to reciprocal space,
especially for non-cubic crystals where the normal to the plane (a real
space description) is the same as the Miller indices description
(reciprocal space). As previously noted, the motion of a crystal is
predicated on the real space description, but in electron microscopy
analysis, the majority of terminology deals with reciprocal space.
Therefore, decoupling these two explanations as first described in the
section above through vector math and then subsequently the conversion
to reciprocal space is necessary for better understanding.

This additional conversion takes advantage of the previous conversion of
non-cubic systems to cubic. In doing so, the normal to any plane can
quickly be calculated given that the descriptions of the normals and the
Miller indices are the same. Utilizing these normals to describe the
plane motion in a double tilt stage provides a full description of any
plane. Given the understanding of dislocation imaging along specific
planes, the ability to accurately map along the trace of a given plane
is imperative for accurate imaging of defects and other
crystallographically dependent structures with a sample.

## Structure Factor as a Filter

A priori knowledge of the allowable planes and poles within a given
crystal based on the atomic arrangement in a specific crystal system is
the most frequent approach for the analysis of crystals within the
microscope. Programs such as Desktop Microscopist and K-space Navigator
relied on this a priori knowledge of any given crystal to output
diffraction and stereographic projections of said crystal. While these
programs were extremely well written descriptions of crystallographic
motion and were imperative to the development of this research, their
use was confined to known crystals. This utilization of this
crystallographic knowledge was based upon the structure factor. By
deconvoluting each step and finishing with the structure factor, it can
be shown that the structure factor simply acts a filter to be placed
upon the results of the previous calculations.

Describing it in this fashion, the position and motion of all possible
vectors within a crystal (regardless of system) can be detailed. Similar
methodologies can be applied in the conversion of planes from reciprocal
space to real space to describe their motion in a double tilt stage. The
structure factor can be viewed as which of those planes, and as well
ZA/poles, are possible thereby dropping out a large fraction that need
to be plotted. Granted, as has been described herein, what is being
plotted is not diffraction or Kikuchi lines, but the pathways between
poles. Whether tilt stages will ever be developed that provide the
precision to accurately discriminate between the (200) or (400) Kikuchi
lines is beyond the scope of this paper, but similar methodologies could
be developed if and when this ever becomes reality. Even so, given the
tendency for local sample foiling and misorientations, even with the
most accurate stages this type of tilting may never be practical.

## General Applications of Nanocartography

Whereas previous research has been confined to crystallographic analysis
and through the motion of a double tilt stage, it will become evident
that only by decoupling real space and reciprocal space can strategies
for solving unknowns and mapping of samples as real space objects be
attained. This takes the extensive amount of previous research on this
subject into a new realm that changes the dynamic of how sample analysis
in the electron microscope is conducted. The limitations of quickly
performing single analyses are removed, and most importantly, it creates
a pathway by which rapid utilization of analytical tools at various
institutions for a single sample can be performed with ease.

The necessity to accurately and rapidly calculate crystallographic
orientations using computer-aided programming is an idea as old as the
personal computer itself. With the advent of crystallographic programs
to assist in understanding and comparing diffraction data to simulated
patterns, it has assisted microscopists in more precisely describing
samples. Programs such as Desktop Microscopist even provided the ability
to input stage conditions to further predict additional tilt protocols.
Unfortunately, due to the delayed data analysis due to film capture,
immediate reaction to these directions was difficult if not time
prohibitive. Additionally, many of these programs consider only a priori
knowledge of crystallographic samples. Much like current EBSD analysis
on modern SEMs, their analyses are beholden to input of candidate
crystals for optimal results. By considering crystals (and their motion)
as physical objects rather than through diffraction and reciprocal
space, it allowed and easier transition to considering the motion of
non-crystalline objects such as grain boundaries and interfaces. More
importantly, it opens the avenue to mapping samples that can then be
later scrutinized for planning of subsequent microscopic analysis or
even for others to rapidly repeat experiments.

Crystallographic analysis using TEM (diffraction) as well as STEM
(atomic column imaging) provides highly localized, site-specific
identification at the nanoscale of both known and unknown phases. Having
full control of the stage both in terms of guiding crystallographic
analysis and the orientation of non-crystallographic features can assist
in a more complete description of any sample analysis. Combining these
together then becomes the ultimate tool for microstructural sample
analysis. Describing the sample as a solid object, which can be
manipulated similar to crystallographic directionality, allows a greater
sense of flexibility. Accurate tilting of an interface or a surface to
an edge on condition can mean the difference between measuring a
diffusion profile of a few nanometers as compared to tens of nanometers.
Similarly, the ability to tilt a boundary or a structure along or
against a logical axis can elucidate a wide variety of latent
microstructures. Two such examples are accurate tilting a boundary in
combination with crystallographic knowledge of adjacent grains and rapid
development of tilt series.

Grain boundaries are an extremely important subject in all of materials
science analysis due their excess free energy that provides a wide array
of phenomena to occur within a microstructure. Rapid diffusion of
chromium in stainless steels provides the means for a thin protective
layer of chromia to form both on free surfaces and at crack tips to
arrest stress corrosion cracking (SCC) {cite:p}`bruemmer2017grain, olszta2014high`. Gallium can decimate the structure of an aluminum body as it
quickly diffuses along grain boundaries, unzipping the entire structure
and leaving behind individual grains {cite:p}`rajagopalan2014atomic`.
Therefore, the study of how elements diffuse and segregate along grain
boundaries is extremely valuable, especially at the nanoscale. At this
scale, phase analysis can be difficult because crystallographic
information from adjacent grains can obfuscate proper analysis of the
desired boundary phase. Given the crystallographic solution of each
adjacent grain in combination with the motion of the boundary to an
on-edge condition can assist in deduction of the unknown phase. With a
boundary edge on, tilting the boundary along the plane can be directed
to an adjacent ZA of either grain which might then provide for low index
planes to be expressed {cite:p}`carter1996transmission`. More importantly,
understanding of parasitic reflections from adjacent grains can be used
to discriminate the possible orientation of the unknown phase to either
grain.

While the description of the precipitation along grain boundaries is
most relevant, understanding morphology and density can also be an
effective means in describing more global bulk properties. Whereas the
typical goal for most effective sample preparation techniques is to
achieve the thinnest possible sample, here it is posited that even
without extremely high accelerating voltages, preliminary analysis of
slightly thicker samples (100-200 nm) can be just as informative as to
the data garnered from subsequent thinning and high-resolution analysis.
Within the volume of a 100-200 nm thick sample the density and
distribution of grain boundary precipitates can provide a more
representative picture of the sample being analyzed. This can be
accomplished through simple logical tilt series that takes advantage of
having the ability to tilt against or along a given interface.
Tomography and APT will always be a more accurate description of the
three-dimensional volume, but they both suffer from being locally
destructive techniques in addition to only providing an extremely narrow
view of the sample volume. Creating rapid tilt series at any given step
size using the protocols, all interfaces within a sample, regardless of
orientation, may be transformed into a digital movie that allows for
more informative data presentation. Since the step sizes between tilts
are minimized for a more accurate description, non-eucentric tilting of
non-orthogonally oriented interfaces is not as drastic, which in turn
allows for quicker data collection. Lastly, while tilt series of
dislocations have been demonstrated in the literature {cite:p}`liu2011three, hata2020electron, yamasaki2015visualization`, if the tilt
map for any given crystal has been solved, tilt series directions for
any plane can quickly be calculated. Instead of following the trace of
the plane systematically, if the directions for the trace of the plane
are calculated it provides for easier data collection.

As with many of the subjects described herein, relating adjacent
crystals to one another is an important topic in material science
analysis and has been discussed in a variety of different manners. Qui
et al. demonstrated how knowledge of crystallographic poles of two cubic
crystals could assist in solving the local misorientation angle between
them {cite:p}`liu1994simple, liu1995simple`, and Jeong et al. {cite:p}`jeong2010characterization`
attempted the use of a triangulation method in solving the same problem.
In section 2 it was demonstrated how one could the orientation of cubic
crystals be solved, but all crystal systems as well. The research herein
takes a similar approach to Qui to demonstrate how the calculation of
the unit vectors for any crystal can be calculated from the solution of
the crystal and then be compared to an adjacent crystal through a
misorientation matrix to achieve similar results {cite:p}`qing1989equation`. In the
derivation of these formulae an important distinction must be considered
in that the rotation about an arbitrary rotation axis to move a known
pole to the \[001\] beam orientation must be performed instead of two
successive rotations about the α and β axes. In solving the
crystallographic orientation of any crystal, the two procedures provide
identical results because the known vector is rotated to the \[001\]
position, but in comparing the location of the unit vectors of two
adjacent crystals the final misorientation angles does not yield a
unique solution. Tilting in the α then subsequently in the β will yield
a different result than first β then α (as shown the Supplemental
**_Figure S4_**). Additionally, through these calculations it has been
determined that the triangulation method is not sufficient in accurately
describing the local misorientation {cite:p}`jeong2010characterization`. Vectors chosen
closest to the \[001\] beam direction will provide a differing result
than vectors farther away from the \[001\]. This is because the
triangulation method does not consider the dependency of the β tilt on
the first α tilt, and therefore errors can be compounded for vectors
farther from the \[001\] beam direction.

Finally, whereas the capture of data on film, either by diffraction or
imaging, was tedious or time consuming (and often erroneous), digital
capture has provided microscopists with the ability to optimize and
improve data collection. The improved accuracy can be utilized in two
distinct manners, first through the tilt of the stage through small
angles, and secondly by calibration of probe deflection. Observation of
a large field of view in k-space in larger crystals provides a sense of
ease because microscopists can immediately observe the motion of the
crystal much like traveling along an open highway. With the advent of
probe corrected instruments, the ability to observe even small volumes
in Ronchigram mode has allowed microscopists to observe small regions of
k-space down to the order to 10s of nanometers. Yet, the ability to tilt
within this small area can be difficult, and therefore being able to
directly provide directions through self-identified regions on a screen
(i.e., a mouse click) is highly desirable. The calculations provided in
this research expand upon the tilt motion of the stage in combination
with the calibration of k-space within digital capture. Conversely, dark
field imaging in TEM mode, a widely useful technique in its own right,
is dependent upon the microscopist's knowledge of accurately deflecting
the beam using condenser lens deflectors. Most often, this is performed
by eye, but calibrating the digital capture with respect to this
deflection allows for more difficult deflection protocols. For instance,
blind tilting can could be achieved by simply pointing to a region on
the screen and having the computer read out the necessary deflections.
Once a diffraction pattern is collected, the beam could be shuttered and
a complete array of deflections could be planned out without introducing
additional dose to the sample. Finally, even more complex schemes by
which the a darkfield map exploring the entire k-space of an FCC versus
BCC crystal could be programmed to best discriminate within a field of
suspected dissimilar phases. Digital manipulation and control of either
small stage tilts or beam deflections provides a clear advantage for
rapid and accurate data collection.
