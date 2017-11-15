###########
Export Data
###########

Replicon mode
----------------------

.. image:: img/download_extract_replicon.PNG

This tool allows to retrieve from a specific organism data stored in PkGDB : complete sequences, non coding DNA, coding sequences (nucleic or proteic), annotated data on genomic objects.

These information can be downloaded in the most common file formats (EMBL, GenBank, Fasta, GFF, Tab delimited). Moreover, data on role categories used in MicroScope, and/or MicroCyc metabolic Pathway/Genome database (PGDBs) can be downloaded too.

First, select a reference replicon from the `CHANGE button (Item #2) <../overview/interface.html>`_ available in the top right corner of the interface. Or select an organism from your `Favourite Organisms <../userpanel/favourites.html>`_ selection.

Organism mode
---------------------

.. image:: img/download_extract_organism.PNG

This tool allows to retrieve from a group of organism sequences data stored in PkGDB. Extraction of several organisms may take several minutes.


Extract genome:
-------------------

.. image:: img/download_extract_genome.PNG

In both mode, you can extract the genome(s):

* Pseudomolecule (all the genomes)
* Contigs (genomes split by contigs)
* Scaffolds (genomes split by scaffolds)

In all the formats: `FASTA <http://www.ncbi.nlm.nih.gov/blast/fasta.shtml>`_, `GENBANK <http://www.ncbi.nlm.nih.gov/genbank/>`_,  `EMBL <http://www.ebi.ac.uk/embl/Documentation/User_manual/usrman.html>`_, `GFF3 <https://en.wikipedia.org/wiki/General_feature_format>`_


Extract data:
-------------------

.. image:: img/download_extract_data.PNG

In replicon mode, you can extract in `FASTA <http://www.ncbi.nlm.nih.gov/blast/fasta.shtml>`_:

* CDSs (All the CDS of the genome in nucleic)
* Proteins (All the CDS of the genome in proteic)
* Repeats (All the repeat region of the genome in nucleic)
* ncRNAs (All the non-coding RNA of the genome in nucleic)

You can also extract in Tabulation delimited format:

* Genome (All the current genomic objects annotation)
* Auto (All the automatic genomic objects annotation)

You can download COG automatic classification (http://www.ncbi.nlm.nih.gov/COG/):

* Genome (All the COG automatic annotation)

finally, you can obtain the `Microcyc pathway <https://biocyc.org/download.shtml>`_


Extract region:
-------------------

.. image:: img/download_extract_region.PNG

* Select the *Begin*, *End* positions and precise the strand you want to get. The default values correspond to the region where the `Genome Browser <../mage/viewer.html>`_ is centered.

The **Sequence** part allow you to extract the sequence (nucleic) in fasta format in the coordinate.

The second part allow you  to extract the annotation in different format (genbank, embl, gff3, tabulation). 

Activating the **Full sequence** option allow you to obtain the whole genome sequence with the annotation of the objects within the coordinates. 
If this option is disable, you will obtain the genome sequence and the annotation within the coordinate, the annotation location will be recalculate.



Noncoding DNA
-------------

.. image:: img/download_extract_ncrna.PNG

Extract the ncDNA sequences from a genome. Indicate a minimal length and include, if necessary, the RNAs.


Extract a sequence fragment
---------------------------

.. image:: img/download_extract_label.PNG

You can extract a sequence fragment:

* Indicate directly a Genomic Object Label to extract and manage, if necessary, the 5’/3’ extension length.


Extract Classification
---------------------------

.. image:: img/download_extract_classification.PNG

Get the complete `Role Classification <../mage/info.html#what-is-the-roles-classification>`_ in a text format.

Get the complete `BioProcess Classification <../mage/info.html#what-is-the-bioprocess-classification>`_ in a text format.

