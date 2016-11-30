###########
Export Data
###########

This tool allows to retrieve from a specific organism data stored in PkGDB : complete sequences, non coding DNA, coding sequences (nucleic or proteic), annotated data on genomic objects.

These information can be downloaded in the most common file formats (EMBL, GenBank, Fasta, GFF, Tab delimited). Moreover, data on role categories used in MicroScope, and/or MicroCyc metabolic Pathway/Genome database (PGDBs) can be downloaded too.

First, select a reference replicon from the `CHANGE button (Item #2) <../overview/interface.html>`_ available in the top right corner of the interface. Or select an organism from your `Favourite Organisms <../userpanel/favourites.html>`_ selection.


FASTA (http://www.ncbi.nlm.nih.gov/blast/fasta.shtml)
-----------------------------------------------------

For a given replicon, you can export:

* Repeats
* ncRNAs
* CDSs
* Proteins
* Genome
* Contigs
* Scaffolds


GENBANK (http://www.ncbi.nlm.nih.gov/genbank/)
----------------------------------------------

Export:

* (complete) Genome
* Contigs
* Scaffolds

EMBL (http://www.ebi.ac.uk/embl/Documentation/User_manual/usrman.html)
----------------------------------------------------------------------

Export:

* (complete) Genome
* Contigs
* Scaffolds

GFF 3 (https://en.wikipedia.org/wiki/General_feature_format)
----------------------------------------------------------------------

Export:

* (complete) Genome
* Contigs
* Scaffolds

Tab(ulation) Delimited (http://en.wikipedia.org/wiki/Delimiter-separated_values)
--------------------------------------------------------------------------------

Useful for exporting data into a spreadsheet. Export:

* (complete) Genome
* Auto (automatic annotation)


COG automatic classification (http://www.ncbi.nlm.nih.gov/COG/)
---------------------------------------------------------------

Export the COG data of the complete genome in a tabulation delimited format.


MicroCyc Pathway/Genome Database (http://biocyc.org/download.shtml)
-------------------------------------------------------------------

Export the MicroCyc Pathway/Genome Database data into a `tar.gz <http://en.wikipedia.org/wiki/Tar_(computing)>`_ compressed file.


Role Classification
-------------------

Get the complete `Role Classification <../mage/info.html#what-is-the-roles-classification>`_ in a text format.


BioProcess Classification
-------------------------

Get the complete `BioProcess Classification <../mage/info.html#what-is-the-bioprocess-classification>`_ in a text format.

Extract a region
----------------

* Select the *Begin*, *End* positions and precise the strand you want to get. The default values correspond to the region where the `Genome Browser <../mage/viewer.html>`_ is centered.


Noncoding DNA
-------------

Extract the ncDNA sequences from a genome. Indicate a minimal length and include, if necessary, the RNAs.


Extract a sequence fragment
---------------------------

You can extract a sequence fragment:

* Indicate directly a Genomic Object Label to extract and manage, if necessary, the 5’/3’ extension length.
