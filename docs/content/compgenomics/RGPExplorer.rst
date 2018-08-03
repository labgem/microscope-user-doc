##########
How to explore an RGP?
##########

The RGP visualization page allows you to access a detailled description of the RGP composition.

The "component" part allow you to know the partion of the gene within the given RGP.

The "RGP gene content" table contains information about the genes which define the given RGP by matching with some other method results:

 - Resistance genes: Antibiotic resistance prediction using `CARD method <https://microscope.readthedocs.io/en/latest/content/compgenomics/card.html>`_
 - Virulence genes: `Virulence prediction <https://microscope.readthedocs.io/en/latest/content/compgenomics/virulence.html>`_
 - Biosythetic gene clusters: `AntiSMASH Prediction <https://microscope.readthedocs.io/en/latest/content/metabolism/antismash.html>`_
 - Macromolecular systems: `MacSyFinder Prediction <https://microscope.readthedocs.io/en/latest/content/compgenomics/macsyfinder.html>`_
 - Integrons: `IntegronFinder Prediction <https://microscope.readthedocs.io/en/latest/content/compgenomics/integron.html>`_

Then you can set parameters to personalize the resistance/virulence shearch within the RGP by using the filters above.
 
.. image:: img/RGPexplorer1.PNG

The "Matching RGPs within Genome Cluster" compare the given RGP with the RGPs in the other organism in the same MICGC ( group of organism made with our method of  `Genome Clustering <https://microscope.readthedocs.io/en/latest/content/compgenomics/genoclust.html>`_ ). 
The comparaison between two RGP is done by looking at the number of gene in each RGP which are in the same MICFAM  `MICFAM <https://microscope.readthedocs.io/en/latest/content/compgenomics/pancoreTool.html#how-the-analysis-is-computed>`_ (MicroScope gene families). 

You can change the filter parameter "% coverage" to change the minimal value of "Shared gene families (%)" in the table.

.. image:: img/RGPexplorer2.PNG
