---
layout: post
title: Barenblatt and Darcy's law
date: 2023-04-18 
description: Barenblatt and Darcy's law
tags: formatting math
categories: math
related_posts: false
---

I found a copy of the rare original Barenblatt, Entov and Ryzhik "ДВИЖЕНИЕ ЖИДКОСТЕЙ И ГАЗОВ В ПРИРОДНЫХ ПЛАСТАХ". The English translation of this book "Theory of Fluid Flows Through Natural Rocks" runs pretty expensive nowadays without known online copies of the digital version. 

Here is the [link] (https://www.geokniga.org/bookfiles/geokniga-dvizhenie-zhidkostey-i-gazov-v-prirodnyh-plastah-gibarenblatt-vmentov-vmryzhik.pdf). Please contact me if you want it removed. 


I translated a relevant section about Darcy's law using some translating engine as I don't speak Russian at all. It is interesting to see how much more elegant the Russian version is both mathematically and in writing, even if it is a translation. 

I will be making gradual improvements of the translation and math as it is still full of mistakes. 

The following is from Barenblatt et al. (1984):

Darcy's law limits of its applicability and clarifications


The main characteristic of the filtration movement, the filtration velocity vector $\mathbf{u}$ , is determined as follows. We choose a point $M$ of the porous medium and draw an arbitrary elementary area $\Delta S$ with normal $\mathbf{n}$ through it. A mass of liquid $\Delta Q$ flows through the selected area per unit time. Then the projection of the vector $\mathbf{u}$ onto the normal $\mathbf{n}$ to the selected area is equal to the limit of the ratio $\Delta Q/\rho \Delta S$  as $\Delta S \lim 0$. Here $\rho $ is the fluid density. not on its part, occupied by pores.



The main relation of the filtration theory - the filtration law - establishes a connection between the filtration velocity vector and the pressure field that causes the filtration movement. Here and below, unless otherwise specifically stated, pressure is the difference between total pressure and hydrostatic pressure; in the absence of motion, the fluid pressure in the pores is distributed according to the hydrostatic law. As soon as movement begins, excess (above hydrostatic) pressure becomes variable in space. The motion of a fluid in a porous medium differs from the motions considered in ordinary hydrodynamics in that in any macrovolume there is a stationary solid phase, at the boundary with which the liquid is also motionless. Therefore, the system of pore channels of an elementary macrovolume is hydrodynamically equivalent to a system of pipes connected in a complex way. The filtration rate characterizes the flow through this system. On the other hand, the flow rate is determined by the pressures at the inlets and outlets of the pore channels. Since the flow rate is the total value for many pore channels, it is determined by the differential, i.e., the gradient of the average fluid pressure


That is why, in contrast to the equations of ordinary hydrodynamics, in the theory of filtration there is a local dependence between the pressure gradient and the filtration velocity vector.



Some information about the form of the filtration law relating the filtration rate and the pressure gradient can be obtained based on the most general ideas. A porous medium is described by geometric parameters—characteristic size d and some dimensionless quantities: porosity m, distribution curve parameters, etc. The filtration law must follow from the equations of fluid motion in the pore space, so the system of defining quantities also includes those characteristics of the fluid that are included in these equations: density p and viscosity mu. Thus, we are looking for the form of dependence of the pressure gradient grad p on the filtration velocity vector u, the geometric characteristics of the porous medium m, d, etc.


and liquid characteristics r and c. Among the quantities on which grad p depends, only the filtration rate is a vector. Due to the isotropy of the medium, the vector grad p must be directed along the same straight line as the vector u. Indeed, let the vector grad p form an angle distinct from zero with the direction of the vector. If the chosen arbitrary coordinate system is rotated around a vector and through a certain angle, then neither this vector nor any other of the defining parameters will change. Consequently, the vector grad p, which depends only on these parameters, should not change either. But if grad p makes a non-zero angle with the direction of the vector and, then when rotating its direction relative to the coordinate axes, it must necessarily change.


This implies that the directions of the vectors and and grad p must coincide, so that

$$
\nabla p = - c \mathbf{u}
$$

where $c$ is some scalar quantity depending on the modulus of the velocity vector $u$, as well as on the quantities $d$, $m$, $\rho$, $\mu$.


Let us consider filtration motions when inertial forces are insignificant. Most of the filtration flows encountered in practice belong to the number of such inertial motions, since they occur slowly. In this case, the density p, which characterizes the inertial properties of the liquid, is insignificant and is excluded from the number of determining parameters. Thus, with inertial motions, the value of $c$ depends only on $u$, $d$, $m$ and $\mu$. Let us write down the dimensions of the quantities of interest to us:

$$
[m] = 1; [с] = ML^{-3}T^{-1}; [u] = LT^{-1}; [d] = L; [\mu] = ML^{-1}T^{-1}. (1.3)
$$


Of the four defining parameters, three ($u$, $d$ and $\mu$) have independent dimensions. Then, according to the analysis of dimensions, the dimensionless combination $cd^2/\mu$. can depend only on the only dimensionless quantity among the determining parameters - porosity $m$:

$$
cd^2/\mu = f(m); c = d^{-2} \mu f(m)
(1.4)
$$


After that, equation (1.2) can be represented as 

$$
\nabla p = - \mu d^{-2} \mathbf{u}; \mathbf{u} = - (\kappa/\mu) \nabla p; \kappa = d^2/f.   (1.5)
$$


Relation (1.2) describes the Darcy filtration law (named after the French engineer A. Darcy, who established it experimentally in 1856). The value $\kappa$ is called permeability (it has the dimension of area, does not depend on the properties of the liquid, and is a purely geometric characteristic of a porous medium).


If instead of $\rho$ we consider the true pressure in the liquid
$P = p - \rho gz $, where $g$ is the free fall acceleration, $z$ is the height of the considered point above some calculated level, then (1.5) can be written in the form

$$
\mathbf{u} = -\nabla (P+ \rho g z). (1.6)
$$

In hydrotechnical calculations, the head $H = p/\rho g $ is usually used, then we have

$$
\mathbf{u} = - C \nabla H, C = \kappa \rho g /\mu (1.7)
$$

where $C$ is the filtration coefficient, has the dimension of velocity.


As can be seen from the above derivation, Darcy's law is a consequence of the assumption of inertia-free fluid motion. A filtration flow obeying Darcy's law is a special case of a creeping flow, which is characterized by the predominance of viscous forces over inertial ones (i.e., the Reynolds numbers are very small - $Re<< 1$). Therefore, attempts to derive Darcy's law by averaging the equations of hydrodynamics are reduced to calculating the permeability from a given geometric structure of a porous medium.



Most often, from formulas of this type, the Kozeny-Karman equation is used, obtained on the basis of an analogy between a porous medium and a system of parallel tubes, expressing the permeability through the specific surface $\Sigma$ and porosity $m$:

$$
\kappa = K m^3 \Sigma^{-2}. (1.8)
$$

The constant $K$ is determined from experimental data and turns out to be different for porous media of various structures. Formula (1.8)



They are mainly used in calculations of the filtration resistance of artificial porous media used in chemical apparatuses, as well as in determining the specific surface area of powders.


Until now, it has been assumed that the porous medium is isotropic. Natural reservoirs are often characterized by anisotropy, associated either with natural layering (for sedimentary rocks) or with the development of systems of parallel microcracks caused by stresses in the rock. If the porous medium is not isotropic, then in an arbitrary orthogonal ekart coordinate system $х_1$, $х_2$ and $х_3$ components of the vector $ grad \rho$ are expressed in terms of the components $u_i$ of the vector $\mathbf{u}$  followin a descriptive way:

$$
\partial p/\partial x_i = - c_{i \alpha} u_{\alpha} (1.9)
$$


where $c_{ij} $ is a certain tensor (summation is assumed over all values of the repeated Greek indices, so that $c_{i\alpha}u_{\alpha}$ means $c_{11}u_{1}+c_{12}u_{2}+c_{13}u_{3})$. In the case of inertial motions, the the components of the tensor $c_{ij} $ can depend only on the viscosity of the fluid $\mu$ and certain geometric characteristics of the porous medium. other geometric characteristics of the porous medium.

Similarly to the derivation of formula (1.9), we can show that $c_{ij} = \mu r_{ij}$ where $r_{ij}$  is the specific filtration resistance tensor, which depends only on the geometric characteristics of the porous medium.



Its components have a dimension inverse to the dimension of the area.
Expressing the components of the velocity vector in terms of the components of the pressure gradient vector, we obtain

$$
u_i =  - (\kappa_{i\alpha}/\mu)\partial p/\partial x_{alpha}, (1.10)
$$

where $k_{ij}$ is the permeability tensor, inverse to the tensor $r_{ij}$, depends only on the geometric characteristics of the porous medium and has the dimension of area. Dependence (1.10) describes Darcy's law for an anisotropic porous medium.

The resistance tensors $r_{ij}$ and permeability $k_{ij}$ are symmetrical$^1$
Subscript
$^$1
This follows from the fact that the quadratic form $$r_{\beta \alpha}u_{\beta}u_{\alpha}$$, proportional to the specific effect of the forces of interaction of the liquid with the porous medium should not depend on the choice of coordinate system,
—



 If the anisotropy of a porous medium is associated with natural layering, the permeability along the layers has one value, and in the perpendicular direction it has another, usually much smaller value. Therefore, one of the principal axes of the permeability tensor - $x_3$  is perpendicular to the bedding plane, and the other two are $x_1$ and $x_2$ can be chosen arbitrarily in the bedding plane. The  $x_1$, $x_2$, $x_2$ sysstem will be the main one at each point of the porous medium;
while we have

$$
k_{11} = k_{22} = k; k_{33} = k_{0}; k_{ij} = 0 (i \ne j). (1.11)
$$

Darcy's law in the chosen coordinate system is written by virtue of relations (1.11) as follows:

$$
u_1 =  - (\kappa/\mu)\partial p/\partial x_{1};
u_2 =  - (\kappa/\mu)\partial p/\partial x_{2};
u_3 =  - (\kappa_0/\mu)\partial p/\partial x_{3}
$$


At significant speeds, when it is no longer possible to ignore the inertial component of the resistance to fluid movement, the prerequisites laid down in the derivation of Darcy's law cease to be valid. Density p with dimension ML~3 should be added to the number of defining parameters. Then the coefficient e in (1.2) will already depend on five quantities, from which two dimensionless combinations can be formed, which gives

$$
\nabla p = - \frac{\mu}{\kappa} \mathbf{u} g ( u\rho d/\mu,  m). (1-12)
$$

The combination of $ u\rho d/\mu = Re$$ is the Reynolds number for filtration micromotion. Assuming that the function $g(Re)$ expands in a power series, and restricting ourselves to the first two terms, we obtain the equation of the two-term filtering law:

$$
-\frac{\kappa}{\mu} \nabla p =  \mathbf{u} + \beta k^{1/2} \mu^{-1} \rho u \mathbf{u}   (1.13)
$$



Here, $k^{1/2}$ is taken as the characteristic dimension $d$ and it is taken into account that for $u \lim 0$ Darcy's law must be valid.
The two-term filtration law was first proposed by Forchheimer. Formula (1.13) describes the observational data well even for very large Reynolds numbers. Thus, for non-cemented (bulk) porous media, this law is valid up to Reynolds numbers of the order of 10-100, while deviations from the linear law begin at $Re \approx$ 0.1-1.0. Repeated attempts have been made to choose the characteristic size $d$ in such a way that the filtration process in porous media of various structures can be described by a single formula. It turned out to be successful introduction as characteristic size of the quantity $(\kappa /m)$^{1/2} proposed by M. D. Millionshchikov. Then the number $Re$ turns out to be equal to $ \rho u \kappa^{1/2} m^{3/2}/\mu$.
In this case, it is possible to uniformly describe the law of filtration in many media of different permeability. For unconsolidated porous media, the coefficients of the two-term filtration law (1.13) can be written in the form

$$
\alpha = A(1-m)^3 m^{-3}/D/ \beta = B(1-m) m^{-3}/D
$$


Here $D$ is the average grain size of the rock, A and B are the values of the coefficients close to constant for individual groups of unconsolidated media, but they depend, for example, on the shape of the grains.

Therefore, this form of writing a two-term law is not universal.

The appearance of a quadratic term in the equation of the filtration law is still sometimes explained by flow turbulence. However, the order of the critical Reynolds numbers in filtration theory (0.1-10), calculated from the diameter of grains or a porous medium, points to the incorrectness of such a statement. The absence of turbulence (i.e., fluctuations in velocity with time) has also been proven by direct experiments. This incorrect view is due to the fact that in the hydraulics of round cylindrical pipes, the deviation from the linear dependence is necessarily associated with flow turbulence, but this is not the case even for laminar flow in curved pipes. In the problems of the theory of oil and gas filtration in natural reservoirs, the application of the two-term law is limited to the movement of high-rate wells in the near-wellbore zone and filtration in fractured media. In addition to violations of the Darcy law associated with the manifestation of inertial forces, the linear filtration law can be violated at very low velocities, when anomalous rheological properties of moving fluids appear.
These questions will be discussed in Chap. III
