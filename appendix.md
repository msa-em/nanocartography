---
title: Appendix
numbering:
  enumerator: 6.%s
---

### Conversion to Cubic

In order to perform math on any crystal system it is first necessary to transform each system such that it can be described as a cubic cell.  The simplest manner in which to accomplish this is to first constrain one of the new vectors onto the z-axis.  For simplicity, and to match the convention that the beam axis is along the z-axis, c is chosen to align with the z-axis ([](#fig26)).  As mentioned in the main body of the text, other equivalent starting choices could be made but they do not inhibit the overall conversion.  The next step is to constrain the second of the new vectors in one plane.  In this case, a is constrained to the xz plane, and then decomposed into the components of that plane using the angle β to the z-axis.  Finally, the third vector is decomposed onto each of the x, y and z axes using the angles α, γ, and δ.  The angle α is the angle from b to the z-axis.  The angle γ is the angle between the vectors a and b.  The last angle, δ, is an auxiliary quantity that is the angle between the projection of the b vector onto the xy plane and the y axis.  Typically, a crystallographic system is specified with a, b, c, α, β, and γ.  The auxiliary angle, δ, is then expressed in terms of these known quantities.

To understand how δ is related to the known quantities, a set of geometric objects is shown in Figure S2 to break down the calculation into smaller steps.  Using the law of cosines on the triangle in the xy plane gives a relationship between the lengths of the three sides and the angle δ.

$$\label{law_cosines} D^2=\ \left(asin{\beta}\right)^2+\left(b\ sin{\alpha}\right)^2-2\left(asin{\beta}\right)\left(bsin{\alpha}\right)cos{\delta}
$$

This has introduced another quantity, D, which is the length of the side of the triangle opposite the angle δ.   Solving for δ yields:

$$\label{delta} \delta={cos}^{-1}{\left(\frac{\left(asin{\beta}\right)^2+\left(b\ sin{\alpha}\right)^2-D^2}{2absin{\alpha}sin{\beta}}\right)}$$
