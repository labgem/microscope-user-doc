#####################
Secondary metabolites
#####################

What are secondary metabolites?
-------------------------------

Secondary metabolism (also called specialized metabolism) is a term for pathways and small molecule products of metabolism that are not absolutely required for the survival of the organism.  Secondary metabolites are produced by many microbes, plants, fungi and animals.
Bacterial secondary metabolites are an important source of antimicrobial and cytostatic drugs. These molecules are often synthesized in a stepwise fashion by multimodular megaenzymes that are encoded in clusters of genes encoding enzymes for precursor supply and modification. 


What is antiSMASH?
------------------

Antismash is a tool predicting secondary metabolite gene clusters in bacterial genomes.

Know  `more <https://microscope.readthedocs.io/en/latest/content/mage/info.html#antismash>`_ about `antiSMASH <http://antismash.secondarymetabolites.org/#!/about>`_


How to access to the secondary metabolites gene clusters predicted by antiSMASH?
--------------------------------------------------------------------------------

Secondary metabolites gene clusters predictions are available through the **Metabolism** section, in the main navigation menu.


What is the "Predicted secondary metabolite clusters"  table?
-------------------------------------------------------------

This table enumerates all secondary metabolite clusters predicted for the selected organism and its replicons.Each predicted cluster is associated to a **Cluster type** defined by antiSMASH.

.. image:: img/antiSMASH._prediction.PNG



What is the "Adjusted cluster coordinates"  table?
--------------------------------------------------

This table enumerates all secondary metabolite clusters alternative coordinates predicted for the selected organism and its replicons.

.. image:: img/antiSMASH_alternative_coord.PNG


Cluster Prediction: classical antiSMASH prediction, it corresponds to the Cluster core coordinates with an extention.

Cluster Border: Improved prediction of gene cluster boundaries using `ClusterFinder algorithm <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4123684/>`_ These estimations are based on frequencies of locally encoded protein domains detected by Pfam (based on these being either more or less BGC-like). 

Cluster Core: cluster coordinates correspond to the "main" genes used for characterization of secondary metabolite.

How to explore a secondary metabolite cluster?
----------------------------------------------

The `AntiSMASH cluster visualization window <https://microscope.readthedocs.io/en/latest/content/metabolism/domainviewer.html>`_ 
can be accessed by clicking on any cluster number in the **Cluster** field.
This window allows you to visualize the full antiSMASH cluster prediction and its genomic context.
