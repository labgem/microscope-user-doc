.. _NGSProjectEvo:

.. TODO:
   Replace evo2.png and evo3.png with real formulas

##########################
Variant profiling projects
##########################

Variant profiling homepage displays the list of available projects.

By Clicking on the arrow available on the left of each project, user can expand the associated functionalities.

.. image:: img/start2.png

Selecting a project will allow the user to use :

* :ref:`Overview tool <NGSOverview>` (**Item #1**)
* :ref:`Read Count Analysis <NGSReadCountAnalysis>` (**Item #2**)
* :ref:`NGSEvoAnalysis` (**Item #3**)
* :ref:`Integrative Genomics Viewer <igv>` (**Item #4**)

What is the meaning of the score computed by SNiPer for each variation?
-----------------------------------------------------------------------

For each reported mutation, a **score**, which is meant to indicate the confidence one can have in the prediction, is computed:

* SNP_score=

.. image:: img/evo2.png

* Local-coverage : Number of reads containing the new base with a high quality.
* Total-coverage : Total number of reads containing the new base.

indel_score=

.. image:: img/evo3.png

* Local-coverage : Number of reads containing the indel.
* Total-coverage : Total number of reads mapping the mutated position.
