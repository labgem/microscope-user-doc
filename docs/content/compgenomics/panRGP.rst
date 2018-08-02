######################
panRGP
######################

What is PPanGGOLiN ?
-------------------------------------------------------

This PPanGGOLiN compiles the genomic content of a species (A) also named a pangenome. It relies on a graph approach to model pangenomes in which nodes and edges represent families of homologous genes (B and C, not included in the pipeline) and chromosomal neighborhood information, respectively. This approach thus takes into account both graph topology (D.a) and occurrences of genes (D.b) to classify gene families into three partitions (i.e. persistent genome, shell genome and cloud genome) yielding to what we called Partitioned Pangenome Graphs (F). More precisely, the method depends upon an Expectation/Maximization algorithm based on Bernoulli Mixture Model (E.a) coupled with a Markov Random field (E.b).

Partitions:
1) Persistent genome: equivalent to a relaxed core genome (genes conserved in all but a few genomes);
2) Shell genome: genes having intermediate frequencies corresponding to moderately conserved genes potentially associated to environmental adaptation capabilities
3) Cloud genome: genes found at a very low frequency.

.. image:: img/ppanggolin.png

When referenced, PPanGGOLiN will generate a graph projection of every organism. In other terms, it will parse all genomes used to build the pangenome and it will project the corresponding part of the graph on it. This means that instead of a succession of genes, the organisms will be represented by the succession of their corresponding gene family partitions (i.e. persistent, shell and cloud).

**Reference:**

.. PPanGGOLiN: https://github.com/ggautreau/PPanGGOLiN

What is a Region of Genomic Plasticity (RGP) ?
-------------------------------------------------------

Following the definition given by Ogier et al., 2010, we define a Region of Genomic Plasticity (RGP) as both integrated Mobile Genetic Elements (MGEs) and hypervariable segments that are likely to be the result of deletions of DNA regions in one or more strains (gene loss). Studying those regions is of particular medical, environmental or industrial interest as they are known to encode virulence and antimicrobial resistance factors, and to harbor genes conferring specific adaptation (pathogenicity, symbiosis properties, detoxification ...).

**Reference:**

`Bertelli C. et al. 2018 Microbial genomic island discovery, visualization and analysis. Briefings in Bioinformatics; [PMID 29868902] <https://www.ncbi.nlm.nih.gov/pubmed/29868902>`_

What is a panRGP ?
-------------------------------------------------------

The goal of panRGP is to efficiently extract RGPs within a partitioned pangenome graph. Firstly, PanRGP needs to extract each gene with its matching partition from the PPanGGOLiN output. Based on its content, the algorithm uses the chaining of gene families partitions to determine the RGPs within a given genome, relying on a double pass linked-list partitioning method

.. image:: img/panRGP.png

The algorithm uses a sequence of genes that are represented by their family’s partition (persistent: yellow; shell: green; blue:cloud). (1) A score is attributed to sets of consecutive genes, based on their partition. Persistent genes get a score of −(3) x (x being the number of consecutive genes) and both cloud and shell ones get a score of +1; (2) Consecutive persistent genes (preserved region) and consecutive cloud and shell genes (variable region) are regrouped in nodes; (3) Each node representing a preserved region is evaluated to determine if it should be grouped with its surrounding node(s), therefore being considered as a gap in the variable region it will results in. This is done only if the addition of its score with the minimum score of its neighboring RGP node(s) is at equals to 0 or more; (4) All nodes have been processed, so variable regions can be parsed to extract the genes they encompass. Here, a RGP of 5 genes (3 shell, 1 persistent and 1 cloud) and one of 1 gene (1 cloud) are obtained.

How to access to panRGP data ?
-------------------------------------------------------


What is the 'panRGP' table?
--------------------------------------------------------


.. image:: img/integronFinder_prediction.png



How to explore panRGP ?
--------------------------------------------------------



