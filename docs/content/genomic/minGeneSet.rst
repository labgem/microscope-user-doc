################
Minimal Gene Set
################

The **Minimal Gene Set** is composed of 206 protein coding genes which include well conserved housekeeping genes for basic metabolism and macromolecular synthesis, many of which are essential genes. This dataset is based on the publication of Gil et al. (2004) which aim was to determine the core of a minimal bacterial gene set.

This functionality propose a list of homologs to the 206 genes defined by Gil et al. classified into 5 main categories: (1) Information storage and processing, (2) Protein processsing, folding and secretion, (3) Cellular processes, (4) Energetic and intermediary metabolism, (5) Poorly catacterized.

For each candidate gene is indicated:

* the number of genes from RefSeq organisms sharing a BBH relationship
* the number of synteny groups from RefSeq organisms sharing a homology relationship

To find the homologs, the tool analyses the similarity results between the genes of each organism and the set of 206 genes from 7 genomes (Escherichia coli K12, Bacillus subtilis 168, Candidatus Blochmania floridanus, Buchnera aphidicola APS, Buchnera aphidicola Bp, Buchnera aphidicola Sg and Mycoplasma genitalium G37). The candidate genes have to fill one of the 2 following conditions:

* share a BBH relationship with a minLRap >0.5
* belong to a synteny group

**Reference**: `Gil R, Silva FJ, Peretó J, Moya A. Determination of the core of a minimal bacterial gene set. Microbiol Mol Biol Rev. 2004 Sep;68(3):518-37. <http://www.ncbi.nlm.nih.gov/pubmed/15353568>`_
