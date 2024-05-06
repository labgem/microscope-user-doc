.. _macsyfinder:

######################
Macromolecular Systems
######################


What is MacSyFinder?
--------------------

Macromolecular System Finder (**MacSyFinder**) provides a flexible framework to model the properties of molecular systems (cellular machinery or metabolic pathway) including their components, evolutionary associations with other systems and genetic architecture.
Modelled features also include functional analogs, and the multiple uses of a same component by different systems.
Models are used to search for molecular systems in complete genomes or in unstructured data like metagenomes.
The components of the systems are searched by sequence similarity using Hidden Markov model (HMM) protein profiles.
The assignment of hits to a given system is decided based on compliance with the content and organization of the system model. 

Learn more about MacSyFinder `here <https://research.pasteur.fr/fr/software/macsyfinder-macsyview/>`_.

.. Don't use MacSyFinder as the name of the link since that would make
   a duplicate with the label.

**Reference:** 

`Abby SS, et al. 2014. MacSyFinder: a program to mine genomes for molecular systems with an application to CRISPR-Cas systems, PLoS ONE 2014;9(10):e110726 ; [PMID 25330359] <http://www.ncbi.nlm.nih.gov/pubmed/25330359>`_


What type of macromolecular systems can be detected?
----------------------------------------------------

MacSyFinder can detect two categories of macromolecular systems:

* A broad range of secretion systems (`TXSScan 1.1.3 <https://github.com/macsy-models/TXSScan>`_): Flagellum, MSH, T1SS, T2SS, T3SS, T4P, T4aP, T4bP, T5aSS, T5bSS, T5cSS, T6SSi, T6SSii, T6SSiii, T9SS, Tad, pT4SSi, pT4SSt.
* A list of conjugative, decayed conjugative and mobilisable elements (`CONJScan 2.0.1 <https://github.com/macsy-models/CONJScan>`_): MOB, T4SS_typeB, T4SS_typeC, T4SS_typeF, T4SS_typeFA, T4SS_typeFATA, T4SS_typeG, T4SS_typeI, T4SS_typeT, dCONJ_typeB, dCONJ_typeC, dCONJ_typeF, dCONJ_typeFA, dCONJ_typeFATA, dCONJ_typeG, dCONJ_typeI, dCONJ_typeT.

To search for them, MacSyFinder is run independently with each category of system. The results are then summarized in a single results table.

**References:**

* `Bongiovanni, T. R., Latario, C. J., Le Cras, Y., Trus, E., Robitaille, S., Swartz, K., Schmidtke, D., Vincent, M., Kosta, A., Orth, J., Stengel, F., Pellarin, R., Rocha, E. P. C., Ross, B. D., & Durand, E. (2024). Assembly of a unique membrane complex in type VI secretion systems of Bacteroidota. Nature communications, 15(1), 429. <https://doi.org/10.1038/s41467-023-44426-1>`_
* `Coluzzi, C., Garcillán-Barcia, M. P., de la Cruz, F., & Rocha, E. P. C. (2022). Evolution of Plasmid Mobility: Origin and Fate of Conjugative and Nonconjugative Plasmids. Molecular biology and evolution, 39(6), msac115. <https://doi.org/10.1093/molbev/msac115>`_
* `Denise, R., Abby, S. S., & Rocha, E. P. C. (2019). Diversification of the type IV filament superfamily into machines for adhesion, protein secretion, DNA uptake, and motility. PLoS biology, 17(7), e3000390. <https://doi.org/10.1371/journal.pbio.3000390>`_
* `Cury, J., Touchon, M., & Rocha, E. P. C. (2017). Integrative and conjugative elements and their hosts: composition, distribution and organization. Nucleic acids research, 45(15), 8943–8956. <https://doi.org/10.1093/nar/gkx607>`_
* `Abby, S. S., Cury, J., Guglielmini, J., Néron, B., Touchon, M., & Rocha, E. P. (2016). Identification of protein secretion systems in bacterial genomes. Scientific reports, 6, 23080. <https://doi.org/10.1038/srep23080>`_


How to access to MacSyFinder predictions?
-----------------------------------------

MacSyFinder predictions are available through the **Comparative Genomics** section and the **Macromolecular Systems** subsection, in the main navigation menu.


What is the 'Macromolecular Systems' table?
-------------------------------------------

This table enumerates all macromolecular systems predicted for the selected organism and its replicons.

.. image:: img/macromolecular_systems.png

* **System id**: identifier of the system in the organism
* **System**: type of system detected by MacSyFinder
* **Replicon name**: identification of the replicon
* **Replicon type**: chromosome, plasmid or WGS
* **Begin** / **End**: position of the system on the replicon
* **Locus type**: single or multi locus
* **Mandatory present**: list of mandatory genes of the system identified in the organism
* **Mandatory missing**: list of mandatory genes of the system not detected in the organism
* **Nb of mandatory present**: number of mandatory genes of the system identified in the organism
* **Nb of mandatory missing**: number of mandatory genes of the system not detected in the organism
* **Nb of accessory present**: number of accessory genes of the system identified in the organism


How to explore a Macromolecular System?
---------------------------------------

The :ref:`MacSyFinder System visualization window <macromolecular-system-vizualization>` can be accessed by clicking on any cluster number in the **System id** field.
This window allows you to access to a detailled description of a selected Macromolecular System.

