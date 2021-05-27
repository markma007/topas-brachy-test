Egsphant patient phantom
------------------------

TOPAS comes with out-of-the-box the patient modeling support by using either DICOM_ or ImageCube_ format.

Topas-brachy provides the implementation of the .egsphant phantom file. Egsphant_ is a phantom file designed 
by EGS MC code system, including EGSnrc, egs-brachy etc. The support of it in brachy-therapy setups a bridge
between TOPAS and EGSnrc.

The way of using Egspahnt phantom is as easy as ImageCube files ::

  s:Ge/Patient/Type           = "EgsphantPatient"
  s:Ge/Patient/InputDirectory = "./"
  s:Ge/Patient/InputFile      = "example.egsphant"



.. _DICOM: https://topas.readthedocs.io/en/latest/parameters/geometry/patient.html#geometry-patient-dicom
.. _ImageCube: https://topas.readthedocs.io/en/latest/parameters/geometry/patient.html#geometry-patient-imagecube
.. _Egsphant: http://www.google.com
