# Haldane model

This notebook is inspired by the great series of lectures provided here [topocondmat](https://topocondmat.org/w4_haldane/haldane_model.html) . Here I will just recall some basics concepts but I would recommend as a starting point to see the link. This notebook is written in Python and therefore for such calculations is not very efficient since Python is an interpreted language. C, C++ or Fortran should be more appropriated for these applications. However this can be used as a basic introduction to the problem. 

In this notebook is an introduction to the Haldane model (proposed as a toy model by F. Duncan M. Haldane in 1988 [here the original paper](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.61.2015)).
The original idea of Haldane was to show that the Quantum Hall effect could be obtained without a magnetic field applied to the system but just by having a standard Bloch band structure with broken time reversal symmetry (TRS) with no net flux through the system.

In this notebook it is possible to see how to make graphene topological. 

Graphene is a single layer of carbon atoms arranged in a honeycomb lattice. It is a triangular lattice with two atoms per unit cell, we denote them as *A* and *B* see the figure below

![Imaginary next-nearest neighbour hopping term](https://topocondmat.org/_images/graphene.svg)

If we consider the most minimal tight-binding model where electrons can hop between neighbors with a strength *t* , it is possible to obtain a so called Bloch Hamiltonian 


## Making graphene topolocical:

As showed in the link provided, the first way (and easiest ) to break TRS is by using a simple mass term or so called onsite energy term of opposite sign +*M* and -*M*. The effect is to open a gap, which can be seen by setting in the notebook the mass term to a value different from zero. Without going into the details of the calculations it can be showed that the energy spectrum is now gapped.

However this mass term preserves time-reversal symmetry and no topological states are expected (also if one calculates the Berry curvature and Chern number this will show that the system is trivial).



### Haldane approach

Haldane found an ingenious way to break TRS without the presence of a magnetic field. The idea was to introduce a next-nearest neighbor (NNN) hopping parameter 

![Imaginary next-nearest neighbour hopping term](https://topocondmat.org/_images/haldane_hoppings.svg)

Note that to have zero flux across the system the hopping is performed on opposite directions (+*i* t<sub>2</sub> and -*i* t<sub>2</sub>)


Where the  t<sub>2</sub> term represents the strength of the NNN parameter. This term changes sign under TRS meaning that is responsible of breaking it.  This in a nutshell is the effect of the NNN term to the standard linear relation of graphene.

I leave to the link attached a more detailed explanation both on the Berry curvature and the calculation of the edge states which are shown in the notebook. 


