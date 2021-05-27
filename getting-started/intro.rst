Introduction to topas-brachy
============================

** Note **
------------

The project is under development.


**The topas-brachy extension**
----------------------------------

Topas-brachy is an extension to the Monte Carlo toolkit TOPAS_ which wraps and extends the `Geant4 Simulation Toolkit`_. 
TOPAS was designed to make Geant4 more readily available to both research and clinical medical physicists as well as to extend its functionality.
Topas-brachy further extends the functionality of the toolkit for brachytherapy applications. 

**Motivation for topas-brachy**

TOPAS has been successfully applied to research in radiation therapy physics for external beam radiation therapy (EBRT).
However, its application in brachytherapy (BT) is not as natural as out-of-the-box due to some key features of BT.

First, in BT, the primary particle positions are coupled with the geometry/materials of BT sources (and seeds). Without topas-brachy, 
users have to describe sources components and use emitive-type sources separately. In case of multiple sources (or seeds), 
emitive source has to be created for each dwell position. Besides, there are a number of different commercial sources (or seeds)
are clinically used and they are difference from each other in design, radioactive isotopes, and other aspects. This worsens the
complexity of modelling in TOPAS parameter file.

Second, it is also the case to use phasespace(s) and multiple dwell positions simultaneously to simulate real BT clinical treatment in which
tens or even hundreds of dwell positions are involved. 
This cannot be easily described in TOPAS parameter file without the help of topas-brachy.

A high-quality extension brachytherapy surely reduces the steepness of learning curve of starting to use TOPAS in BT simulation.
The extenstion also features of ease-of-use -- BT simulations can be modelled with just a few lines in parameter file. That being said,
constancy is achieved across community in terms of geometry, materials, and energy spectrum of certain BT source or seed.

.. _TOPAS: http://www.topasmc.org
.. _Geant4 Simulation Toolkit: https://geant4.web.cern.ch