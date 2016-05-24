######################
AntiSMASH cluster visualization
######################

What is antiSMASH?
------------------

Know  `more <https://microscope.readthedocs.io/en/latest/content/mage/info.html#antismash>`_ about `antiSMASH <http://antismash.secondarymetabolites.org/about.html>`_



How can I visualize the clusters predicted by antiSMASH?
--------------------------------------------------------

You can access to the **AntiSMASH cluster visualization** window from the Cluster column of any antiSMASH result table.
This window allows you to visualize the full antiSMASH cluster prediction and its genomic context.
You can also use the main navigation menu in the **Metabolism** section to obtain the **AntiSMASH predictions** page.
This page enumerates all secondary metabolite cluster detected for the choosen sequence and its replicons.


What informations are in this window?
--------------------------------------------------------

In case of NRPS/PKS cluster type, the predicted peptide monomer composition may be indicated as well, if this composition is specific enough, the smile prediction is displayed.

.. image:: img/antiSMASH3_viewer.PNG


|
|

Thanks to `https://cdkdepict-openchem.rhcloud.com/depict.html <https://cdkdepict-openchem.rhcloud.com/depict.html>`_ for Picture's displays 

|
|


The **MIGiB Clusters Similarities** table provide information about similar cluster in MIBiG database. The Minimum Information about a Biosynthetic Gene cluster (MIBiG) can help to know more on biosynthetic gene clusters and their molecular products.

`Medema M.H., et al. (2015) Minimum Information about a Biosynthetic Gene cluster. Nat Chem Biol. Sep;11(9):625-31. <http://www.ncbi.nlm.nih.gov/pubmed/26284661>`_


.. image:: img/antiSMASH3_Knowncluster.PNG


|
|


All informations regarding the CDS present in the graphical representation are available in the ** Genomic Objects** table below the graphical representation of the cluster.

.. image:: img/antiSMASH3_Feature.PNG

|
|


The **Tailoring Clusters Similarities** table provide information about gene which may be involve in tailoring reaction. By clicking on the number, you can access to the Pubmed related article.

The 6 first columns help to know more about the predict tailoring clusters, the *label* column give MicroScope gene label.
The next 3 columns: *TC protein id* , *TC gene name* and *Protein description* give informations about tailoring genes in this tailoring cluster and the last 3 columns give match informations between tailoring gene and MicroScope one.


.. image:: img/antiSMASH3_Tailoringcluster.PNG

|
|


What is the meaning of the color code in the AntiSMASH cluster visualisation window?
-------------------------------------------------------------------------------------------

.. image:: img/antiSMASH3_domain_color_code.PNG
.. image:: img/antiSMASH3_Feature_color_code.PNG
