---
title: "Heat capacity of solids 1"
date: 2025-07-04
categories: [Physics, Thermodynamics, Statistical Mechanics]
tags: [Dulong-Petit Law, Boltzmann, Heat Capacity, Harmonic Oscillator, Partition Function]
math: true 
---
<script type="text/javascript"
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>

In 1819, Pierre Louis Dulong and Alexis Thérèse Petit experimentally discovered that the molar heat capacity for 13 measured elements was approximately constant. They observed that the product of the mass-specific heat capacity and the presumed relative atomic weight of the element yielded a nearly constant value. At the time, Dulong and Petit were unaware of the relationship between their findings and the gas constant ($R$), as this constant had not yet been defined through the kinetic theory of gases.

It wasn't until 1877 that Boltzmann theoretically elucidated this relationship, which we will explore in this post. Boltzmann modeled each atom in a solid as a three-dimensional harmonic oscillator, residing within a potential well created by its neighboring atoms. The Hamiltonian for such an oscillator is given by:

\\[
H = \\frac{P^2}{2m} + \\frac{1}{2}kx^2
\\]

Here, both $P$ (momentum) and $x$ (position) are three-dimensional vectors, meaning they each have three components. The partition function ($Z$) for such a system is then:

\\[
Z = \\frac{1}{(2\\pi\\hbar)^3} \\int \\exp(-\\beta H) \\, dx \\, dp
\\]
This integral can be separated into two independent integrals: one for the momentum term and one for the position term:

$$Z = \frac{1}{(2\pi\hbar)^3} \left( (\int \exp\left(-\beta \frac{P^2}{2m}\right) \, dp \right) )^3 \left(( \int \exp\left(-\beta \frac{1}{2}kx^2\right) \, dx \right))^3$$
The cube powers in the partition function arise because we are dealing with three spatial dimensions — each dimension contributes independently to the integral.

Now, the integrals involved are standard Gaussian integrals and are straightforward to evaluate using the identity:

\\[
\int_{-\infty}^{\infty} \exp(-\alpha x^2) \, dx = \sqrt{\\frac{\pi}{\alpha}}
\\]

Applying this identity to both the momentum and position integrals, and simplifying, we eventually arrive at the partition function:

\\[
Z = \\frac{1}{\hbar \omega \beta}
\\]

Once we have the partition function, calculating the average energy becomes straightforward. The average energy is given by:

\\[
\\langle E \\rangle = -\\frac{\\partial}{\\partial \\beta} \\ln Z
\\]

Substituting the expression for \( Z \), we find:

\\[
\\langle E \\rangle = 3k_B T
\\]

Finally, the heat capacity at constant volume is the derivative of the average energy with respect to temperature:

\\[
C_V = \\frac{\\partial \\langle E \\rangle}{\\partial T} = 3k_B
\\]

This is the classical result predicted by the Dulong–Petit law, which states that the molar heat capacity of a solid is approximately \( 3R \), where \( R \) is the universal gas constant.

However, don’t get too excited — this classical approach has its limitations. The Dulong–Petit law fails at low temperatures and cannot explain the observed decrease in heat capacity. In the next article, we'll explore how Einstein addressed this problem with a clever quantum correction.

---
