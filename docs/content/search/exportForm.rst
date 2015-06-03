###########
Export Data
###########

This tool allows to retrieve from a specific organism data stored in PkGDB : complete sequences, non coding DNA, coding sequences (nucleic or proteic), annotated data on genomic objects.

These information can be downloaded in the most common file formats (EMBL, GenBank, Fasta, XML, Tab delimited). Moreover, data on role categories used in MicroScope, and/or MicroCyc metabolic Pathway/Genome database (PGDBs) can be downloaded too.

First, select a reference replicon from the `CHANGE button (Item #2) <http://microscope.readthedocs.org/en/latest/content/overview/interface.html>_` available in the top right corner of the interface. Or select an organism from your `Favourite Organisms <http://microscope.readthedocs.org/en/latest/content/userpanel/favourites.html>`_ selection.


FASTA (http://www.ncbi.nlm.nih.gov/blast/fasta.shtml)
-----------------------------------------------------

For a given replicon, you can export:

* Repeats
* ncRNAs
* CDSs
* Proteins
* Genome


XML (http://en.wikipedia.org/wiki/XML)
--------------------------------------

Export:

* Region: corresponds to the region where the `Genome Browser <http://microscope.readthedocs.org/en/latest/content/mage/viewer.html>`_ is centered.
* (complete) Genome


GENBANK (http://www.ncbi.nlm.nih.gov/genbank/)
----------------------------------------------

Export:

* Region: corresponds to the region where the `Genome Browser <http://microscope.readthedocs.org/en/latest/content/mage/viewer.html>`_ is centered.
* (complete) Genome


EMBL (http://www.ebi.ac.uk/embl/Documentation/User_manual/usrman.html)
----------------------------------------------------------------------

Export:

* Region: corresponds to the region where the `Genome Browser <http://microscope.readthedocs.org/en/latest/content/mage/viewer.html>`_ is centered.
* (complete) Genome


Tab(ulation) Delimited (http://en.wikipedia.org/wiki/Delimiter-separated_values)
--------------------------------------------------------------------------------

Useful for exporting data into a spreadsheet. Export:

* Region: corresponds to the region where the `Genome Browser <http://microscope.readthedocs.org/en/latest/content/mage/viewer.html>`_ is centered.
* (complete) Genome


Feature Table (http://www.ncbi.nlm.nih.gov/Sequin/table.html)
-------------------------------------------------------------

Export:

* Region: corresponds to the region where the `Genome Browser <http://microscope.readthedocs.org/en/latest/content/mage/viewer.html>`_ is centered.
* (complete) Genome


COG automatic classification (http://www.ncbi.nlm.nih.gov/COG/)
---------------------------------------------------------------

Export the COG data of the complete genome in a tabulation delimited format.


MicroCyc Pathway/Genome Database (http://biocyc.org/download.shtml)
-------------------------------------------------------------------

Export the MicroCyc Pathway/Genome Database data into a `tar.gz <http://en.wikipedia.org/wiki/Tar_(computing)>`_ compressed file.


Role Classification
-------------------

Get the complete `Role Classification <http://microscope.readthedocs.org/en/latest/content/mage/editor.html#what-is-the-roles-classification>`_ in a text format.


BioProcess Classification
-------------------------

Get the complete `BioProcess Classification <http://microscope.readthedocs.org/en/latest/content/mage/editor.html#what-is-the-bioprocess-classification>`_ in a text format.


Noncoding DNA
-------------

Extract the ncDNA sequences from a genome. Indicate a minimal length and include, if necessary, the RNAs.


Extract a sequence fragment
---------------------------

You can extract a sequence fragment:

* Select the *Begin*, *End* positions and precise the strand you want to get.
* Indicate directly a Genomic Object Label to extract and manage, if necessary, the 5’/3’ extension length.