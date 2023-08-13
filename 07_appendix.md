---
title: Appendix
numbering:
  enumerator: 6.%s
---

### Conversion to Cubic

In order to perform math on any crystal system it is first necessary to transform each system such that it can be described as a cubic cell.  The simplest manner in which to accomplish this is to first constrain one of the new vectors onto the z-axis.  For simplicity, and to match the convention that the beam axis is along the z-axis, c is chosen to align with the z-axis ([](#figA1)).  As mentioned in the main body of the text, other equivalent starting choices could be made but they do not inhibit the overall conversion.  The next step is to constrain the second of the new vectors in one plane.  In this case, a is constrained to the xz plane, and then decomposed into the components of that plane using the angle β to the z-axis.  Finally, the third vector is decomposed onto each of the x, y and z axes using the angles α, γ, and δ.  The angle α is the angle from b to the z-axis.  The angle γ is the angle between the vectors a and b.  The last angle, δ, is an auxiliary quantity that is the angle between the projection of the b vector onto the xy plane and the y axis.  Typically, a crystallographic system is specified with a, b, c, α, β, and γ.  The auxiliary angle, δ, is then expressed in terms of these known quantities.

To understand how δ is related to the known quantities, a set of geometric objects is shown in [](#figA2) to break down the calculation into smaller steps.  Using the law of cosines on the triangle in the xy plane gives a relationship between the lengths of the three sides and the angle δ.

$$\label{law_cosines} D^2=\ \left(a \sin{\beta}\right)^2+\left(b\sin{\alpha}\right)^2-2\left(a\sin{\beta}\right)\left(b\sin{\alpha}\right)\cos{\delta}
$$

This has introduced another quantity, D, which is the length of the side of the triangle opposite the angle δ.   Solving for δ yields:

$$\label{delta} \delta={\cos}^{-1}{\left(\frac{\left(a\sin{\beta}\right)^2+\left(b\sin{\alpha}\right)^2-D^2}{2ab\sin{\alpha}\sin{\beta}}\right)}$$

:::{figure} ./images/Figure A1.jpg
:name: figA1
Schematics illustrating step-by-step derivation of the non-cubic to cubic conversion matrix.
:::

To find the value of D, the Pythagorean Theorem is used on the right triangle with D as the base.

$$\label{d_squared}\ D^2+\left(a\cos{\beta}-b\cos{\alpha}\right)^2=G^2 $$

In this equation, G, is the side opposite the angle γ in the triangle which has legs a and b.  The law of cosines is also applied here to find:

$$\label{g_squared}\ G^2=a^2+b^2-2ab\cos{\gamma} $$

Eliminating G^2 to find D^2 and then substituting back into the equation for δ and simplifying the trigonometric functions yields a simplified expression:

$$\label{appendix_delta} \delta={\cos}^{-1}{\left(\frac{\cos{\gamma}+\cos{\alpha}\cos{\beta}}{\sin{\alpha}\sin{\beta}}\right)}$$

:::{figure} ./images/Figure A2.jpg
:name: figA2
 Schematic illustrating the calculation of the angle δ that accounts for non-orthogonal angles between axes in monoclinic and triclinic systems in the conversion matrix.
:::

With the angle $\delta$ known, the full expression for the conversion matrix is what was presented above in the text as Eq. [](#conversion_matrix_appendix):

$$\label{conversion_matrix_appendix} M=\ \left[\begin{matrix}a\sin{\beta}&b\sin{\alpha}\cos{\delta}&0\\0&b\sin{\alpha}\sin{\delta}&0\\a\cos{\beta}&b\cos{\alpha}&c\\\end{matrix}\right]$$

This matrix will convert a vector from a non-cubic system to a cubic system after matrix multiplication. The reverse process (going from cubic to a non-cubic system) is accomplished by multiplying by the inverse matrix.  The inverse matrix for M is:

$$\label{inversion_matrix_appendix} M^{-1}=\left[\begin{matrix}\frac{1}{a\sin{\beta}}&\frac{-\cos{\delta}}{a\sin{\beta}\sin{\delta}}&0\\0&\frac{1}{b\sin{\alpha}\sin{\delta}}&0\\\frac{-\cos{\beta}}{c\sin{\beta}}&\frac{\cos{\beta}\sin{\alpha}\cos{\delta}-\sin{\beta}\cos{\alpha}}{c\sin{\alpha}\sin{\beta}\sin{\delta}}&\frac{1}{c}\\\end{matrix}\right]$$

### Hexagonal to Cubic

Whereas ([](#fig1)) provided a simplistic example of the need to convert non-cubic systems to cubic before performing mathematical calculations, ([](#figA3)) illustrates a more complicated crystal system.  A number of low index vectors in the hexagonal unit cell provided in ([](#figA3)), which are described in the native nomenclature and are invariable despite the c/a ratio (([](#fig2))).  A schematic presentation of the cubic matrix conversion can be envisioned by placing a cube with the x and z axes commensurate with the hexagonal x and z axes and observing the traces of the vectors in the hexagonal system overlapping with the inserted cube.  After a mental transcription of the vectors onto the cube, the hexagonal vectors can be removed, thereby leaving the vectors in the cubic cell.  The positions of the vectors within the cube can then be observed.  Mathematical operations, such as the angle between poles, can then be performed.

:::{figure} ./images/Figure A3.jpg
:name: figA3
Illustration showing the conversion of a hexagonal matrix to cubic form.
:::

### Rotation about an Arbitrary Axis

Rotations about the principal axes are simple to state, but are of limited use when considering general crystal orientations.  Instead, it is useful to rotate about an arbitrary axis in space for any angle, not just rotation about one of the principal axes (Eqns. [](#rotation_x) to [](#mirror_z)).  As previously stated, this rotation is not necessary to create useful tip/tilt maps, but it is necessary when comparing two crystals in a misorientation matrix.  The misalignment that arises in the misorientation matrix as compared to the tip/tilt maps is that while the vector moves to the correct position in both derivations (e.g., the [111] to the [001]), the location of the unit vectors (i.e., [001], [100], and [010]) will vary depending on pathway.  This will be derived subsequently, but is illustrated schematically in [](#figA4).  

The vector [uvw] is rotated to the [001] orientation about [xy0] through angle θ.  The schematic details two pathways by which to achieve this rotation; path 1 which is about a single axis, and path 2 which is through two concurrent tilts about the additional unit vector axes (in this case x and y).  A movie is provided that indicates the motion of path 2.  In both cases the [111] vector is rotated to [001], but the location of the unit axes (as shown by the projection of a cube down the [111]) will differ by some angle (Δ) as compared to the rotation about the arbitrary axis.  Note that the illustrated angle is exaggerated for effect, and is only approximately a few degrees.  Depending on the order of the pathway, the angle (Δ) would also be different, hence providing two distinct projections of the unit vectors for misorientation calculations.

The example described above and illustrated in [](#figA4) pertains directly to the formulation of a tip/tilt map for a double tilt stage (i.e., the rotation axis is always calculated normal to the [001] orientation), but a more general formulation of the tilt about an arbitrary axis needs be derived to account for non-crystallographic motions.  Therefore, the full derivation is provided below.  

To describe this general rotation, a sequence of steps can be used to decompose any rotation down into rotations about the principal axes.  To accomplish this the desired axis of rotation needs to be rotated to coincide with any one of the principal axes through two rotations about the other axes (in the tip/tilt map calculation the z or probe axis is chosen).  The desired rotation about the arbitrary axis is accomplished with the system aligned along a principal axis (e.g., $φ_{c}$).  Finally, the arbitrary axis is returned to its original location by performing the inverse of the first two rotations.  For more details of this process, consult {cite:p}`Cole2015`. 

The axis of rotation is a unit vector, $\hat{\mathbf{u}}=(u_x,\ u_y,\ u_z)$ and the desired angle of rotation about this axis is θ.  Without loss of generality, the arbitrary axis will be rotated to the x-axis where the rotation by θ occurs.  First, $\hat{\mathbf{u}}$ rotates into the x-y plane by rotating about the y-axis by an angle $φ_{1}$.  This angle is computed by the requirement that the resulting vector, $\widehat{\mathbf{u}_\mathbf{1}}=(u_{1,x},\ u_{1,y},0)$ has no y-component.  The angle $φ_{1}$ which accomplishes this rotation is $\varphi_1=\tan^{-1}{\left(\frac{u_z}{u_x}\right)}$ and can be found from the z-component ([](#figA5)). 


$$\label{math_matrix} \left[\begin{matrix}\cos{\varphi_1}&0&\sin{\varphi_1}\\0&1&0\\-\sin{\varphi_1}&0&\cos{\varphi_1}\\\end{matrix}\right]\left[\begin{matrix}u_x\\u_y\\u_z\\\end{matrix}\right]=\ \left[\begin{matrix}u_x\cos{\varphi_1}+u_z\sin{\varphi_1}\\u_y\\{-u}_x\sin{\varphi_1}+u_z\cos{\varphi_1}\\\end{matrix}\right]=\ \left[\begin{matrix}u_{1,x}\\u_{1,y}\\0\\\end{matrix}\right]$$

In particular, since the y-component is unchanged $(u_y=u_{1,y})$ and the magnitude of the vector is still 1, this intermediate vector can be written as $\widehat{\mathbf{u}_\mathbf{1}}=\left(\sqrt{1-u_y^2},u_y,\ 0\right)$.  Next, the vector $\widehat{\mathbf{u}_\mathbf{1}}$ is rotated to point along the x-axis.  This rotation is by an angle $φ_{2}$ about the z-axis and the angle is determined by the requirement that the resulting vector should have no x-component.  This angle is $\varphi_2=\tan^{-1}{\left(\frac{-u_y}{\sqrt{1-u_y^2}}\right)}$ as can be seen by equating the y-component of the vector to 0.  

$$\label{math_matrix_two} \left[\begin{matrix}\cos{\varphi_2}&-\sin{\varphi_2}&0\\\sin{\varphi_2}&\cos{\varphi_2}&0\\0&0&1\\\end{matrix}\right]\left[\begin{matrix}\sqrt{1-u_y^2}\\u_y\\0\\\end{matrix}\right]=\ \left[\begin{matrix}\left(\sqrt{1-u_y^2}\right)\cos{\varphi_2}-u_y\sin{\varphi_2}\\\left(\sqrt{1-u_y^2}\right)\sin{\varphi_2}+u_y\cos{\varphi_2}\\0\\\end{matrix}\right]=\ \left[\begin{matrix}1\\0\\0\\\end{matrix}\right]$$

These two angles move the vector to the x-axis, where it is rotated by an angle θ and then rotated back to the original position by rotating the negative of $φ_{2}$ and $φ_{1}$.  Combining all of these rotations into one yields the overall rotation matrix, $R_{\hat{u},\theta}$:

$$\label{rotation_matrix_appendix} R_{\hat{u},\theta}=R_{-φ1,y} R_{-φ2,z} R_{θ,x} R_{φ2,z} R_{φ1,y}$$

In this equation, each rotation matrix is defined by the angle and the axis about which the rotation occurs.  Note that the negative angle rotations are undoing the initial rotations to bring the vector to the x-axis and are the inverses of the first two rotations which can be found by taking the transpose of the $R_{φ_{1},x}$ and $R_{φ_{2},y}$ since for any rotation matrix, $R^{-1}=R^{T}$.  If we express these matrices in terms of the matrices and simplify the trigonometric expressions in terms of the components of $\hat{\mathbf{u}}$, then the matrix product is:

$$\label{matrix_product} R_{\hat{u},\theta}=\left[\begin{matrix}\frac{u_x}{\sqrt{u_x^2+u_z^2}}&0&\frac{{-u}_z}{\sqrt{u_x^2+u_z^2}}\\0&1&0\\\frac{u_z}{\sqrt{u_x^2+u_z^2}}&0&\frac{u_x}{\sqrt{u_x^2+u_z^2}}\\\end{matrix}\right]\left[\begin{matrix}\sqrt{1-u_y^2}&{-u}_y&0\\u_y&\sqrt{1-u_y^2}&0\\0&0&1\\\end{matrix}\right]\left[\begin{matrix}1&0&0\\0&\cos{\theta}&-\sin{\theta}\\0&\sin{\theta}&\cos{\theta}\\\end{matrix}\right]\left[\begin{matrix}\sqrt{1-u_y^2}&u_y&0\\-u_y&\sqrt{1-u_y^2}&0\\0&0&1\\\end{matrix}\right]\left[\begin{matrix}\frac{u_x}{\sqrt{u_x^2+u_z^2}}&0&\frac{u_z}{\sqrt{u_x^2+u_z^2}}\\0&1&0\\\frac{{-u}_z}{\sqrt{u_x^2+u_z^2}}&0&\frac{u_x}{\sqrt{u_x^2+u_z^2}}\\\end{matrix}\right]$$

After matrix multiplication and simplification, recalling that the magnitude of $\hat{\mathbf{u}}$ is one $({u_x^2+u}_y^2+u_z^2=1)$, the full matrix for rotation of angle θ about an axis of rotation $\hat{\mathbf{u}}$ is:

$$\label{rot_theta_about_u} R_(\hat{r},θ)=\left[\begin{matrix}u_x^2+(u_y^2+u_z^2 )  \cos⁡\theta & u_x u_y (1-\cos⁡θ )-u_z  \sin⁡θ & u_x u_z (1-\cos⁡θ )+u_y \sin⁡θ \\ u_x u_y (1-\cos⁡θ )+u_z  \sin⁡θ&u_y^2+(u_x^2+u_z^2 )\cos⁡θ & u_y u_z (1-\cos⁡θ )-u_x  \sin⁡θ\\ u_x u_z (1-\cos⁡θ )-u_y  \sin⁡θ & u_y u_z (1-\cos⁡θ )+u_x  \sin⁡θ & u_z^2+(u_x^2+u_y^2 )  \cos⁡ θ \end{matrix}\right]$$

::: {figure} ./images/Figure A4.jpg
:name: figA4
Direct rotation about an arbitrary axis as compared to two rotations about unit vector axes.
:::

::: {figure} ./images/Figure A5.jpg
:name: figA5
Schematics demonstrating the angles necessary to rotate around an arbitrary vector.
:::

### Examples of Tip/Tilt Maps in Lower Symmetry Systems

As demonstrated in ([](#figA7)), tip tilt maps for cubic and hexagonal crystal systems can be procured in any number of orientations.  The same can be done for other non-cubic systems such as tetragonal and orthorhombic (Figure A6a-c).  In the [001] orientation a tetragonal crystal with a c:a ratio of 2 (as illustrated in Figures 1 and 10 ) there are more accessible poles within an ~40° range as compared to the cubic form (i.e., [](#figA7)a).  To demonstrate the asymmetry of the tetragonal system the [010] is plotted in [](#figA6)b.  When the third unit axis vector is changed (i.e., orthorhombic), the larger asymmetry can be observed in ([](#figA6))c.  In order to best demonstrate how the tip/tilt maps can vary between a high symmetry system (i.e., cubic) and lower symmetry systems (e.g., monoclinic and triclinic) the [112] of the three systems is plotted in [](#figA6)d-f with the orientation of the [001] pole in each system ~15° from the α tilt axis.  The various tilt positions of the [001] between the three systems as well as other surrounding poles highlights the large discrepancy when the unit axes and angles between axes varies.  While each of these crystal system parameters were utilized from real crystals, it should be noted that the plotting of poles is in a general form to highlight the variability and does not fully represent whether each of the poles are expressed in those systems.  Additionally, while the family of poles (e.g., the <112>) are plotted with the same format (e.g., blue dots) practically they are different families due to the variation in axes and angle between axes (e.g., the [112] is not in the same family of the [121] for a triclinic system). 

:::{figure} ./images/Figure A6.jpg
:name: figA6
Tip/Tilt plots of various crystal systems.
:::

### Plotting Kikuchi Bands

Plotting the traces of planes of atoms was accomplished by using the normal to the plane as an arbitrary axis by which to rotate any vector in the plane.  This approach is not appropriate for tracing Kickuchi bands that are located at an angular distance equaling the Bragg angle from the trace of the plane of atoms.  If these planes were to be plotted on a tip tilt map ([](#figA7)) it is unlikely that the precision of current double tilt stages would be able to discretely tilt to these conditions.  In [](#figA7) the [111] orientation of an FCC crystal is shown plotted on a tip tilt map with a corresponding Kikuchi pattern.  The strong (4-40) bands shown in the Kikuchi pattern are the approximately the smallest d-spacings observed in all materials systems, and when plotted in the tip/tilt map it becomes apparent that all larger d-spacings would be bound within these lines (hence not within the precision of current double tilt holders).  The projection of the large condenser aperture (~103 mrad) shown in the Kikuchi pattern is overlaid on the tip/tilt map for scale.

::: {figure} ./images/Figure A7.jpg
:name: figA7
Plot of tilt map for [111] FCC austenitic stainless steel in the [111] orientation with the {440} planes expressed (a) and a CBED pattern in the same orientation (b).
:::

### Vector Equations to Matrix

The key to solving the system of equations for the coordinate vectors in Eqns. [](#linear_A1)-[](#linear_A3) is to rewrite them as vector equations for the elements of $\vec{p}, \vec{q}$, and $\vec{t}$.  Writing out all nine equations gives:

$$\label{XA1} u_{A1}p_{Ax}+v_{A1}q_{Ax}+w_{A1}t_{Ax}=x_{A1}$$
$$\label{YA1} u_{A1}p_{Ay}+v_{A1}q_{Ay}+w_{A1}t_{Ay}=y_{A1}$$
$$\label{ZA1} u_{A1}p_{Az}+v_{A1}q_{Az}+w_{A1}t_{Az}=z_{A1}$$
$$\label{XA2} u_{A2}p_{Ax}+v_{A2}q_{Ax}+w_{A2}t_{Ax}=x_{A2}$$
$$\label{YA2} u_{A2}p_{Ay}+v_{A2}q_{Ay}+w_{A2}t_{Ay}=y_{A2}$$
$$\label{ZA2} u_{A2}p_{Az}+v_{A2}q_{Az}+w_{A2}t_{Az}=z_{A2}$$
$$\label{XA3} u_{A3}p_{Ax}+v_{A3}q_{Ax}+w_{A3}t_{Ax}=x_{A3}$$
$$\label{YA3} u_{A3}p_{Ay}+v_{A3}q_{Ay}+w_{A3}t_{Ay}=y_{A3}$$
$$\label{ZA3} u_{A3}p_{Az}+v_{A3}q_{Az}+w_{A3}t_{Az}=z_{A3}$$

In this order, the patterns in these equations are not clear, so instead, they are grouped as Eqns. [](#XA1), [](#XA2), [](#XA3), Eqns. [](#YA1), [](#YA2), [](#YA3), and Eqns. Eqns. [](#ZA1), [](#ZA2), [](#ZA3).  These groupings yield:

$$\label{XA1_v2} u_{A1}p_{Ax}+v_{A1}q_{Ax}+w_{A1}t_{Ax}=x_{A1}$$ 

$$\label{XA2_v2} u_{A2}p_{Ax}+v_{A2}q_{Ax}+w_{A2}t_{Ax}=x_{A2}$$

$$\label{XA3_v2} u_{A3}p_{Ax}+v_{A3}q_{Ax}+w_{A3}t_{Ax}=x_{A3}$$


$$\label{YA1_v2} u_{A1}p_{Ay}+v_{A1}q_{Ay}+w_{A1}t_{Ay}=y_{A1}$$

$$\label{YA2_v2} u_{A2}p_{Ay}+v_{A2}q_{Ay}+w_{A2}t_{Ay}=y_{A2}$$

$$\label{YA3_v2} u_{A3}p_{Ay}+v_{A3}q_{Ay}+w_{A3}t_{Ay}=y_{A3}$$



$$\label{ZA1_v2} u_{A1}p_{Az}+v_{A1}q_{Az}+w_{A1}t_{Az}=z_{A1}$$

$$\label{ZA2_v2} u_{A2}p_{Az}+v_{A2}q_{Az}+w_{A2}t_{Az}=z_{A2}$$

$$\label{ZA3_v2} u_{A3}p_{Az}+v_{A3}q_{Az}+w_{A3}t_{Az}=z_{A3}$$

In this grouping, these systems become much more recognizable as matrix equations:

$$\label{XA_matrix} \left[\begin{matrix}u_{A1}&v_{A1}&w_{A1}\\u_{A2}&v_{A2}&w_{A2}\\u_{A3}&v_{A3}&w_{A3}\\\end{matrix}\right]\left[\begin{matrix}p_{Ax}\\q_{Ax}\\t_{Ax}\\\end{matrix}\right]=\left[\begin{matrix}x_{A1}\\x_{A2}\\x_{A3}\\\end{matrix}\right]$$

$$\label{YA_matrix} \left[\begin{matrix}u_{A1}&v_{A1}&w_{A1}\\u_{A2}&v_{A2}&w_{A2}\\u_{A3}&v_{A3}&w_{A3}\\\end{matrix}\right]\left[\begin{matrix}p_{Ay}\\q_{Ay}\\t_{Ay}\\\end{matrix}\right]=\left[\begin{matrix}y_{A1}\\y_{A2}\\y_{A3}\\\end{matrix}\right]$$

$$\label{ZA_matrix} \left[\begin{matrix}u_{A1}&v_{A1}&w_{A1}\\u_{A2}&v_{A2}&w_{A2}\\u_{A3}&v_{A3}&w_{A3}\\\end{matrix}\right]\left[\begin{matrix}p_{Az}\\q_{Az}\\t_{Az}\\\end{matrix}\right]=\left[\begin{matrix}z_{A1}\\z_{A2}\\z_{A3}\\\end{matrix}\right]$$

In particular, the 3x3 matrices in each grouping are the same, which means that the same set of row operations will row reduce all of them simultaneously.  As such, they are combined into a single augmented matrix that is Eqn. [](#augmented_matrix) in the text.

$$\label{augmented_matrix_appendix} \left[\begin{matrix}u_{A1}&v_{A1}&w_{A1}\\u_{A2}&v_{A2}&w_{A2}\\u_{A3}&v_{A3}&w_{A3}\\\end{matrix}\middle|\begin{matrix}x_{A1}&y_{A1}&z_{A1}\\x_{A2}&y_{A2}&z_{A2}\\x_{A3}&y_{A3}&z_{A3}\\\end{matrix}\right]$$
