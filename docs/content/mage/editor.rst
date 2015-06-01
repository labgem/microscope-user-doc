######################
Gene annotation editor
######################

=================================
Overview of the annotation editor  
=================================

How to access to the Gene Annotation Editor?
--------------------------------------------

There are two ways of accessing the Gene Annotation Editor:

* 1- click on a genomic object on the genomic map
* 2- click on a label in the table of genomic objects which is below the genomic map

NB : requesting information via the GetInfo button only calls up a read-only Gene Annotation Editor window.


Overview of the Gene Annotation Editor
--------------------------------------

The Gene Annotation Editor window is made of 4 sections:

* a **toolbar** that allows access to different functionalities
* the **current annotation** of the genomic object. This section can be modified by the annotator (with sufficient rights).
* the **primary annotation** of the genomic object. It correspond to the MicroScope pipeline automatic annotation (if it is a first annotation) or to the databank annotation (if it is a reannotation project).
* the **Method results** section. This section gives an access to the results obtained by the different tools used for the syntactic and functional annotation process.


How to use the Gene Annotation Editor toolbar?
----------------------------------------------

.. image:: img/editor1.png

It contains several buttons allowing access to different functionalities:

* the sequence (nucleic and protein) of the genomic object
* the annotation history of the genomic object
* **5’/3’**: the sequence (nucleic and protein) of the genomic object
* **TrEMBL alignments**: visualisation of the alignments with TrEMBL best hits
* **SwissProt alignments**: visualisation of the alignments with SwissProt best hits
* **Phyloprofile**: this tool provides a list of all CDSs (from all replicons) that have the same phylogenetic profile (presence/absence of homologue in others species) than the current genomic object. Note: query can be slow.
* **PubMed**: this functionality opens a new window that shows the references that have been linked to this genomic object on PubMed
* **KEGG**: this functionality opens the KEGG description corresponding to the annotated EC number(s)
* **Brenda**: this functionality opens the Brenda entry corresponding to the annotated EC number(s)
* **BioCyc**: this functionality opens a new window showing information related to the genomic object in the BioCyc database


How to fill the Gene Annotation form?
-------------------------------------

As shown in the figure below, not all fields can be modified by the annotator. Furthermore, some of them are required and other are optional. These fields have to be filled after the careful analysis of the different methods results. 

.. image:: img/editor2.png

.. tip:: If one of the required field is missing or wrongly filled a warning will appear in the window.


What are the different annotation "Status"es?
---------------------------------------------

* **inProgress** : the annotator has not finished the expert annotation
* **finished** : the annotator has finished the expert annotation
* **Curated** : the expert annotation has been reviewed by a specialist of the functional process in which the CDS product is involved
* **Artefact** : An artefactual CDS corresponds to a false prediction by the gene detection program. An artefactual CDS should never be similar to any proteins from the databanks (except if the same erroneous annotation has been made in another genomes)
* **chkSeq** : this status is used by the annotator to flag potential sequencing errors in the sequence. When the sequencing is performed at Genoscope, these chkSeq sequences will be sent to the people working in the finishing team. They will then check the assembly to see if the sequence quality is good or not. If needed they can perform some additional PCRs to enhance the data.
* **chkStart** : the annotator suspects that a start position readjustment might be needed for the CDS, but hasn’t done it yet.


What are the different "Type" categories?
-----------------------------------------

* CDS
* fCDS
* tRNA
* rRNA
* misc_RNA
* intron
* exon
* IS
* misc_feature
* promoter


How to fill the "Mutation" field?
---------------------------------

* **no** => Normal CDS
* **frameshift** => CDS for which a true frame-shift has been biologically demonstrated
* **pseudo** => the CDS is part of a pseudogene
* **partial** => the CDS is a gene fragment
* **gene remnant** => the CDS is a highly degraded gene fragment
* **selenocysteine** => the CDS contains a Selenocysteine in its sequence


How to use the "Comments" field?
--------------------------------

The **Comments** field is dedicated to the annotators who want to leave some notes for themselves or for others annotators from the project. This field is not exported to the Genbank file at the end of the annotation process.


How to use the "PubmedID" field?
--------------------------------

The PubMedID or PMID correspond to the index of a publication on the PubMed section of the NCBI website. You can fill this field when you want to link a publication to your annotation. If you want to enter several publications, you simply have to write the PMIDs separated by commas.

You will find the PMID of a publication directly on Pubmed as shown on the figure below. You can also find PMIDs in the "References" section of the UniProt entries. 

.. image:: img/editor3.png

If this field is filled you will have a direct access to the publications on PubMed by clicking on the **Pubmed** button on top of the Gene annotation editor window.


How to use the "MetaCyc reaction" field?
----------------------------------------

This field allows user to link one ore more metabolic reactions from MetaCyc (BioCyc) to the current edited gene.

.. image:: img/editor4.png


* a - Reactions presented at the top of the field have been manually curated by an annotator.
* b - A multiple selection list gives quick access to all predicted (unselected) or curated (selected) reactions linked to this gene.
* c - A search box allows one to quickly access MetaCyc reactions corresponding to either EC numbers from previous EC number field or a given keyword.

**Search box :**

Clicking on the “EC” button will search all MetaCyc reactions corresponding to the EC number from the “EC number” field.

The keyword search will look for all MetaCyc reactions having an identifier, a name or involving a compound similar to the given keyword.

**Search result :**

.. image:: img/editor5.png

The search returns a list of MetaCyc reactions, with :

* the reaction identifier and name. Identifier is clickable and open the BioCyc reaction card.

And in some cases :

* Genes of the organism already linked to this reaction (eg. first row of the example). Genes are flagged with :
	* “validated” : reaction has been manually linked to this gene by users.
	* “annotated” : reaction has been linked to homologous gene and transferred here from a close genome.
	* “predicted” : reaction has been linked to this gene by the pathway-tools algorithm.

* If the reaction has no known coding genes but belongs to a pathway predicted to exist in the current organism, a clickable link to the MetaCyc pathway description is given (eg. fourth row of the example).

The “Reset” button deletes all results


How to use the "Rhea reaction" field?
-------------------------------------

This field allows user to link one ore more metabolic reactions from **Rhea** to the current edited gene.

.. image:: img/editor6.png


* a - Reactions presented at the top of the field have been manually curated by an annotator.
* b - A multiple selection list gives quick access to all curated reactions linked to this gene.
* c - A search box allows one to quickly access Rhea reactions corresponding to either EC numbers from previous EC number field or a given keyword.

**Search box :**

Clicking on the “EC” button will search all Rhea reactions corresponding to the EC number from the “EC number” field.

The keyword search will look for all Rhea reactions having an identifier, a name, involving a compound name or Chebi identifier similar to the given keyword.

**Search result :**

Rhea reactions are present in 4 exemplary according to the direction :

* bidirectionnal : <=>
* left to right : =>
* right to left : <=
* unknown (master reaction) : <?>

.. image:: img/editor7.png

The search returns a list of Rhea reactions, with :

* the reaction identifier and name. Identifier is clickable and open the Rhea reaction card. By default, the master reaction is presented. Select the direction wanted in the "direction-select".

And in some cases :

* Genes of the organism already linked to this reaction (eg. first row of the example). Genes are flagged with :
	* “validated” : reaction has been manually linked to this gene by users.
	
The “Reset” button deletes all results

**How to link a new reaction :**

For each reaction in the result set, check-box allows to add a reaction from the result set to the select element. All reactions selected in the multiple selection list will be saved as validated and linked to this gene. Unselecting a reaction in this list will remove this link from the curated data.


What are the different "Product type" categories?
-------------------------------------------------

* c : carrier
* cp : cell process
* e : enzyme
* f : factor
* h : extrachromosomal origin
* l : leader peptide
* lp : lipoprotein
* m : membrane component
* n : RNA
* o : ORF of unknown function
* pc : putative carrier
* pcp : putative cell process
* pe : putative enzyme
* pf : putative factor
* ph : phenotype
* pm : putative membrane component
* pr : putative regulator
* prc : putative receptor
* ps : putative structure
* pt : putative transporter
* r : regulator
* rc : receptor
* s : structure
* t : transporter


What are the different "Localization" categories?
------------------------------------------------- 
 
* 1 : Unknown
* 2 : Cytoplasmic
* 3 : Fimbrial
* 4 : Flagellar
* 5 : Inner membrane protein
* 6 : Inner membrane-associated
* 7 : Outer membrane protein
* 8 : Outer membrane-associated
* 9 : Periplasmic
* 10 : Secreted
* 11 : Membrane


How to use the "Class" field?
-----------------------------

The **Class** annotation categories are useful for assigning a "confidence level" to each gene annotation. It has been inspired by the "protein name confidence" defined in **PseudoCAP** (Pseudomonas aeruginosa community annotation project).

This information is not given by the automatic functional annotation procedure, except in case of functional annotation transfer from a genome being annotated with MaGe.

The different classes are:

* **1a : Function experimentally demonstrated in the studied strain**
* **1b : Function experimentally demonstrated in the studied species**
* **1c : Function experimentally demonstrated in the studied genus**
* **2a : Function of homologous gene experimentally demonstrated in an other organism**
* **2b : Function of strongly homologous gene**
* **3 : Function proposed based on presence of conserved amino acid motif, structural feature or limited homology**
* **4 : Homologs of previously reported genes of unknown function**
* **5 : No homology to any previously reported sequences**
* **6 : Doubtful CDS**. A doubtful CDS is a CDS for which the annotator is not sure that it codes for a protein. If this CDS really seems like a false prediction, he will then choose the **Artefact** status.
* **7 : Gene remnant**


What is the "BioProcess" classification?
----------------------------------------

This functional classification is based on the **CMR JCVI Role IDs.**

This field is optionally filled in during the expert annotation process.


What is the "Roles" classification?
-----------------------------------

This functional classification corresponds to the MultiFun classification which has been developed by Monica Riley for E. coli (http://genprotec.mbl.edu/).

**Reference**:`Serres MH, Riley M. MultiFun, a multifunctional classification scheme for Escherichia coli K-12 gene products. Microb Comp Genomics. 2000;5(4):205-22. <http://www.ncbi.nlm.nih.gov/pubmed/11471834>`_ 

This field is optionally filled in during the expert annotation process.


How to choose the "Class" annotation category?
----------------------------------------------

.. image:: img/editor8.png

.. image:: img/editor9.png


How to identify artefacts?
--------------------------

.. image:: img/editor10.png



================
Annotation Rules  
================

.. image:: img/annotation1.png

Considering the Class field, here are some basic annotation rules:

1 a/b/c: Function experimentally demonstrated in the studied organism/species/genus
-----------------------------------------------------------------------------------

Gene [optional]
Synonyms [optional]
Product **[mandatory]**
EC number [optional]
MetaCyc Reaction [optional]
PubMedId **[mandatory]**
ProductType **[mandatory]**
Localization [optional]
BioProcess [optional]
Roles [optional]


2a : Function of homologous gene experimentally demonstrated in an other organism
---------------------------------------------------------------------------------

Gene [optional]
Synomyms [optional]
Product **[mandatory]**
EC number [optional]
MetaCyc Reaction [optional]
PubMedId **[mandatory]**
ProductType **[mandatory]**
Localization [optional]
BioProcess [optional]
Roles [optional]


2b : Function of strongly homologous gene
-----------------------------------------

Gene [optional]
Synonyms [optional]
Product **[mandatory]**
EC number [optional]
MetaCyc Reaction [optional]
PubMedId [optional]
ProductType **[mandatory]**
Localization [optional]
BioProcess [optional]
Roles [optional]


3 : Function proposed based on presence of conserved amino acid motif, structural feature or limited homology
-------------------------------------------------------------------------------------------------------------

Gene [not allowed]
Synonyms [not allowed]
Product **[mandatory]**: putative function
EC number [optional]
MetaCyc Reaction [optional]
PubMedId [optional]
ProductType **[mandatory]**: putative function
Localization [optional]
BioProcess [optional]
Roles [optional]


4 : Homologs of previously reported genes of unknown function
-------------------------------------------------------------

Gene [not allowed]
Synonyms [not allowed]
Product **[mandatory]** : conserved (exported/membrane) protein of unknown function (; [domain description])
EC number [not allowed]
MetaCyc Reaction [optional]
PubMedId [optional]
ProductType **[mandatory]**: unknown
Localization [optional]
BioProcess [optional]
Roles [optional]


5 : No homology to any previously reported sequences
----------------------------------------------------

Gene [not allowed]
Synonyms [not allowed]
Product **[mandatory]**: (exported/membrane) protein of unknown function
EC number [not allowed]
MetaCyc Reaction [optional]
PubMedId [optional]
ProductType **[mandatory]**: unknown
Localization [optional]
BioProcess [optional]
Roles [optional]


6 : Doubtful CDS
----------------

Gene [not allowed]
Synonyms [not allowed]
Product **[mandatory]** : protein of unknown function
EC number [not allowed]
MetaCyc Reaction [not allowed]
PubMedId [optional]
ProductType **[mandatory]**: unknown
Localization [not allowed]
BioProcess [not allowed]
Roles [not allowed]


7 : Gene remnant
----------------

Gene [not allowed]
Synonyms [not allowed]
Product **[mandatory]**: protein name (fragment)
EC number [not allowed]
MetaCyc Reaction [not allowed]
PubMedId [optional]
ProductType **[mandatory]**: unknown
Localization [not allowed]
BioProcess [not allowed]
Roles [not allowed]


=============
BLAST results
=============


What is the meaning of the minLrap and maxLrap values?
------------------------------------------------------

These values are ratios of alignment lengths computed for each comparison using the BLAST software :

* **minLrap** = Lmatch/min(Lprot1, Lprot2)
* **maxLrap** = Lmatch/max(Lprot1, Lprot2)

where Lmatch = length of the match, Lprot1 = length of protein 1, Lprot2 = length of protein 2.

**if minLrap=1 and maxLrap=1** => the 2 proteins both align on their whole length

**if minLrap=1 ans maxLrap<1** => one of the proteins is longer than the other, or the alignment is partial. Different interpretations are possible:

* the longer protein is a modular protein (domain fusion/fission)
* there is an erroneous start codon for one of the 2 genes
* the smaller gene is a fragment (pseudogene).
* a frameshift (due to a sequencing error or not) causes a premature stop codon in one of the genes.

**if minLrap<1 and maxLrap<1** => the sequences are poorly aligned. We can observe this kind of situation in the case of gene remnants.


What is the meaning of orderQ and orderB values?
------------------------------------------------

The orderQ and orderB values give an information about the rank of the BLAST hit for a protein of the query genome (orderQ) or for a protein of a databank (orderB).

Best bidirectional Best Hits (BBH) will have a 1:1 relationship The following Best hits will have 1<=>n relationship

.. image:: img/blast.png

.. tip:: These indicators can be useful to identify fusion/fission events.



=====
Start
=====

Coming soon...



======================
Compositional features
======================

Gene compositional features
---------------------------

Coming soon...

Protein compositional features
------------------------------
Coming soon...



============
Duplications 
============

This dataset contains the list of genes of the genome that have an identity > 25% with a minLRap > 0.75 to the selected gene.



===========
E. coli K12
===========

This menu indicates the best BLAST hit for the current Genomic Object against the genome of Escherichia coli K12, if any.

This dataset is a useful reference since E. coli is a very well known bacteria, with a carefully annotated genome and large quantities of experimental data and publications are available.

.. tip:: This dataset can help you to complete your expert annotation.



===========
B. subtilis
===========

This menu indicates the best BLAST hit for the current Genomic Object against the genome of Bacillus subtilis, if any.

This dataset is a useful reference since B. subtilis is a very well known bacteria, with a carefully annotated genome and large quantities of experimental data and publications are available.

.. tip:: This dataset can help you to complete your expert annotation.



===============
Genomes/Project
===============

This section indicates the best BLAST hits for the current Genomic Object with Genomic Objects from other PkGDB genomes that are linked to the current annotation Project.

These other Genomic Objects having been automatically (re-)annotated using the MaGe platform, and maybe even been manually annotated/curated by MaGe users, can serve as informative references for your own annotations.

How to read the result table?
-----------------------------

* **Label**: Label of the protein. If you click on the label, you access the Gene annotation window for that Genomic Object.
* **Organism**: Organism name. If you click on the name, you access the organism’s sequences on the NCBI website
* **Gene**: Gene name of the protein
* **Evidence**: Status of the annotation.
* **Gene**: Gene name of the genomic object
* **Product**: Product description of the protein
* **maxLrap**: see BLAST results
* **minLrap**: see BLAST results
* **Ident%**: Percentage of identity between the studied protein and the database protein
* **Eval**: E value of the BLAST result
* **OrderQ**: see BLAST results
* **OrderB** :see BLAST results
* **BeginQ**: Start of the alignment for the studied protein
* **EndQ**: End of the alignment for the studied protein
* **LengthQ**: Length the studied protein
* **BeginB**: Start of the alignment for the database protein
* **EndB**: End of the alignment for the database protein
* **LengthB**: Length of the database protein



========================
MaGe/Curated annotations
========================

This section indicates the best BLAST hits obtained with other Genomic Objects from PkGDB which have been manually annotated/curated by other MaGe users.

How to read the result table?
-----------------------------

* **Label**: Label of the protein. If you click on the label, you access to the Gene annotation window
* **Synteny**: If you click on the magnyfying glass, it opens a synton visualisation window
* **Organism**: Organism name. If you click on the name, you access to the sequences on the NCBI website
* **Gene**: Gene name of the protein
* **Product**: Product description of the protein
* **maxLrap**: see BLAST results
* **minLrap**: see BLAST results
* **Ident%**: Percentage of identity between the studied protein and the database protein
* **Eval**: E value of the BLAST result
* **OrderQ**: see BLAST results
* **OrderB**: see BLAST results
* **Roles**: Funtional categories associated with the protein using the Roles functional classification
* *ECnumber**: EC number associated with the protein, if any
* **Localization**: Cellular localisation of the protein
* **BioProcess**: Funtional categories associated with the protein using the BioProcess functional classification
* **Product type**: Description of the product type of the protein
* **PubMedId**: References linked to the annotation of the protein
* **Class**: Confidence class of the annotation
* **BeginQ**: Start of the alignment for the studied protein
* **EndQ**: End of the alignment for the studied protein
* **LengthQ**: Length the studied protein
* **BeginB**: Start of the alignment for the database protein
* **EndB**: End of the alignment for the database protein
* **LengthB**: Length of the database protein


============================
Syntonome / Syntonome RefSeq 
============================

How to use the Syntonome results?
---------------------------------

This section gives access to the list of syntons which contain homologs to the studied gene in other organisms:

* from PkGDB for the **Syntonome** section
* from RefSeq for the **Syntonome RefSeq** section


How to read the result table
----------------------------

* **Synteny**: If you click on the magnifying glass, it opens a synton visualisation window
* **NbGeneQ**: Number of genes involved in the synton in the studied genome
* **NbGeneB**: Number of genes involved in the synton in the database genome
* **Organism**: Organism name. If you click on the name, you can access the associated genome sequence on the NCBI website.
* **Label**: Label of the database protein. If you click on the label, you can access the Gene annotation window (Syntonome) or to the corresponding NCBI entry (Syntonome RefSeq)
* **Gene**: Gene name of the database protein
* **Product**: Product description of the database protein
* **maxLrap**: see BLAST results
* **minLrap**: see BLAST results
* **ident%**: Percentage of identity between the studied protein and the database protein
* **Eval**: E value of the BLAST result
* **OrderQ**:see BLAST results
* **OrderB**:see BLAST results
* **BeginQ**: Start of the alignment for the studied protein
* **EndQ**: End of the alignment for the studied protein
* **LengthQ**: Length of the studied protein
* **BeginB**: Start of the alignment for the protein of the database
* **EndB**: End of the alignment for the protein of the database
* **LengthB**: Length of the protein of the database



=====
HAMAP
=====

What is HAMAP?
--------------

HAMAP (High-quality Automated and Manual Annotation of microbial Proteomes) is a system, based on manual protein annotation, that identifies and semi-automatically annotates proteins that are part of well-conserved families or subfamilies: the HAMAP families. HAMAP is based on manually created family rules and is applied to bacterial, archaeal and plastid-encoded proteins.

**More**: http://www.expasy.ch/sprot/hamap/

**Reference**:

`HAMAP: a database of completely sequenced microbial proteome sets and manually curated microbial protein families in UniProtKB/Swiss-Prot. Lima T et al (2009) Nucleic Acids Res. 2009 Jan;37(Database issue):D471-8. <http://www.ncbi.nlm.nih.gov/pubmed/18849571>`_


How to read HAMAP results?
--------------------------

.. image:: img/hamap.png

This section is filled in when the sequence can be linked to a HAMAP family. The corresponding HAMAP family identifier is given in the first column. If you click on it, it will open a new window on the HAMAP website, giving you a full description of the family.

The evidence column gives an indication about the strength of the hit. The value can be:

* *high*: the sequence is considered to be trusted member of the HAMAP family
* *medium*: the sequence is considered as a putative member of the HAMAP family

The following columns give a description of the HAMAP family with the gene name (if any), the product description, the EC number (if any). The comments column can give you some insight into the corresponding function or the subcellular location of the protein. The last column describes a list of keywords related to the function of the HAMAP family.



===============================
Similarities SwissProt / TrEMBL
===============================

What is UniProt?
----------------

The Universal Protein Resource (UniProt) is a comprehensive resource for protein sequence and annotation data. The mission of UniProt is to provide the scientific community with a comprehensive, high-quality and freely accessible ressource of protein sequence and functional information.

The UniProt Knowledgebase consists of two sections:

* **Swiss-Prot** which contains high quality manually annotated and non-redundant protein sequences. This database brings together experimental results, computed features and scientific conclusions.
* **TrEMBL** which contains protein sequences associated with computationally generated annotation and large-scale functional characterization that await full manual annotation.

More than 99% of the protein sequences provided by UniProtKB are derived from the translation of the coding sequences (CDS) which have been submitted to the public nucleic acid databases, the EMBL-Bank/GenBank/DDBJ databases. All these sequences, as well as the related data submitted by the authors, are automatically integrated into UniProtKB/TrEMBL.

**More**: http://www.uniprot.org/

**Reference**: `UniProt Consortium. The Universal Protein Resource (UniProt) in 2010. Nucleic Acids Res. 2010 Jan;38(Database issue):D142-8 <http://www.ncbi.nlm.nih.gov/pubmed/19843607>`_
