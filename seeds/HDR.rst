High Dose Rate (HDR) Sources
============================

A common end point of measurement for cells cultured *in vitro* in radiobiology is clonogenic cell survival. Single cell Monte Carlo simulations can provide insight into the total dose received by the cell or the distribution of dose within sub-regions of the cell (e.g., dose to the cell nucleus). This may be correlated with experimental measurements of the loss of a specific function or cell death. Single cell models can also form the geometric boundary for more complex studies, for example, calculating the energy deposited in other sub-cellular components (e.g., organelles, cell membranes) or investigating DNA damage in the nucleus. 

TOPAS-nBio provides users with a unique framework for simulating multiple cell types and the option of including organelle sub-components in the model. 

Spherical Cell
---------------
.. figure:: images/SphericalCell.png
   :width: 300
   :align: center 


The TsSphericalCell component is a model of a spherical cell with the option of including organelles. 
To create the model specify the component name as well as the cell radius required::  

  s:Ge/MyCell/Type="TsSphericalCell"
  d:Ge/MyCell/CellRadius=20 um