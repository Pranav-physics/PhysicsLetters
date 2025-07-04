---
title: "heat capacity of solids"
date: 2025-07-04
categories: [Physics, Thermodynamics, Statistical Mechanics]
tags: [Dulong-Petit Law, Boltzmann, Heat Capacity, Harmonic Oscillator, Partition Function]
math: true 
---

In 1819, Pierre Louis Dulong and Alexis Thérèse Petit experimentally discovered that the molar heat capacity for 13 measured elements was approximately constant. They observed that the product of the mass-specific heat capacity and the presumed relative atomic weight of the element yielded a nearly constant value. At the time, Dulong and Petit were unaware of the relationship between their findings and the gas constant ($R$), as this constant had not yet been defined through the kinetic theory of gases.

It wasn't until 1877 that Boltzmann theoretically elucidated this relationship, which we will explore in this post. Boltzmann modeled each atom in a solid as a three-dimensional harmonic oscillator, residing within a potential well created by its neighboring atoms. The Hamiltonian for such an oscillator is given by:

$$H = \frac{P^2}{2m} + \frac{1}{2}kx^2$$

Here, both $P$ (momentum) and $x$ (position) are three-dimensional vectors, meaning they each have three components. The partition function ($Z$) for such a system is then:

$$Z = \frac{1}{(2\pi\hbar)^3} \int \exp(-\beta H) \, dx \, dp$$

This integral can be separated into two independent integrals: one for the momentum term and one for the position term:

$$Z = \frac{1}{(2\pi\hbar)^3} \left( \int \exp\left(-\beta \frac{P^2}{2m}\right) \, dp \right) \left( \int \exp\left(-\beta \frac{1}{2}kx^2\right) \, dx \right)$$

---
