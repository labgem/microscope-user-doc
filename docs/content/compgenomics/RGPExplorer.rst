.. _rgpexplorer:

######################
How to explore an RGP?
######################

The RGP visualization page allows you to access a detailed description of the RGP composition.

The "Components" table gives the percentage of genes for each partition within the RGP.

The "RGP gene content" table contains information about the genes which define the given RGP and results with other methods:

 - Resistance genes: Antibiotic resistance prediction using :ref:`CARD method <card>`
 - Virulence genes: :ref:`Virulence prediction <virulence>`
 - Biosythetic gene clusters: :ref:`AntiSMASH Prediction <antiSMASH>`
 - Macromolecular systems: :ref:`MacSyFinder Prediction <macsyfinder>`
 - Integrons: :ref:`IntegronFinder Prediction <integron>`

To personalize the resistance/virulence search within the RGP, you can set alignment parameters using the form above.
 
.. image:: img/RGPexplorer1.PNG

The "Matching RGPs within Genome Cluster" table compares the given RGP with the predicted ones in the other organisms of the same MICGC (see method of  :ref:`Genome Clustering <genoclust>`). 
The percentage of shared gene families correspond to the number of  :ref:`MICFAM <pancore-analysis>` (MicroScope gene families) that are present in the RGP of the compared organism. 

You may use the filter parameter "% coverage" to change the minimal value of "Shared gene families (%)" in the table.

.. image:: img/RGPexplorer2.PNG
