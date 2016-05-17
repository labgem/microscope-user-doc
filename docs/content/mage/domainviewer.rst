######################
AntiSMASH cluster visualization
######################


How can I visualize the clusters predicted by antiSMASH?
--------------------------------------------------------

You can access to the AntiSMASH cluster visualization window from the Cluster column of the antiSMASH annotation table.
This window allows you to visualize the full antiSMASH cluster prediction and its genomic context.
In case of NRPS/PKS cluster type, the predicted peptide monomer composition is indicated as well. You can also see the smile prediction if its exist.

.. image:: img/antiSMASH3_viewer.PNG

The **Knowncluster** table provide information about known cluster in MIBiG database

`Medema M.H., et al. (2015) Minimum Information about a Biosynthetic Gene cluster. Nat Chem Biol. Sep;11(9):625-31. <http://www.ncbi.nlm.nih.gov/pubmed/26284661>`_

.. image:: img/antiSMASH3_Knowncluster.PNG

All informations regarding the CDS present in the graphical representation are available in the **Features** table below the graphical representation of the cluster.

.. image:: img/antiSMASH3_Feature.PNG

The **Tailoringcluster** table provide information about gene which may be involve in tailoring reaction. By clicking on the number, you can access to the Pubmad related article.

.. image:: img/antiSMASH3_Tailoringcluster.PNG

What is the meaning of the color code in the AntiSMASH cluster visualisation window?
-------------------------------------------------------------------------------------------
.. image:: img/antiSMASH3_domain_color_code.PNG
.. image:: img/antiSMASH3_Feature_color_code.PNG
