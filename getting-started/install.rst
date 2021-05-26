How to Install topas-brachy
===========================

Installing TOPAS
----------------

Topas-brachy is an extension to the TOPAS toolkit. In order to install topas-brachy, users must first install TOPAS. 

Topas-brachy requires TOPAS version 3.2.0 or newer. 

TOPAS can be downloaded from `topasmc.org <http://topasmc.org>`_. Installation instructions for TOPAS can be found bundled the following README.txt: 

.. highlight:: plain
.. literalinclude:: README.txt

An updated README.txt file is distributed with every new TOPAS version.


Installing topas-brachy
-----------------------
Download the topas-brachy extension and put in a separate directory (e.g. /path-To-WorkDirectory/topas-brachy). This path should not be inside the main TOPAS installation directory to avoid accidental loss of your extensions and parameter files when updating to a new TOPAS version. 
After building TOPAS link the topas-brachy extension and rebuild the code::
 
	cmake -DTOPAS_EXTENSIONS_DIR=/path-To-WorkDirectory/topas-brachy
	make -j8

When done, the topas executable within the TOPAS/bin folder is updated and the topas-brachy components are available and working.