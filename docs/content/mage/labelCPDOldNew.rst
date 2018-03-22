#######################
Annotation Mapping
#######################

Only available for users having an account on MicroScope.

Provides CDS label (i.e, locus_tag) correspondences between a new version of the genome being annotated/analysed (progression of the sequencing step) and the old one(s).

=================================
Report Methods
=================================
At the moment the report is only perform with CDS (and fCDS).

In order to report the annotation from the previous version of the sequence to the updated one, we perform several BLAST analyses:

* 1- We use BLASTp between all the CDS automatically found in both sequences by the MicroScope annotation pipeline. We make a correspondence using the filter (pos>=100 and lrap=1) for the genes with the same length (AA) with Bidirectional Best Hits.
* 2- We perform a tBLASTn using genes which have been validated (annotated) or manually created by the user on the previous version of the sequence (if these genes have not passed the first BLAST filter) on the new sequence. We make a correspondence using the filter (pos>=100) for the genes with the same length (nucleic).


=================================
Manually report
=================================

In few cases, the correspondences may not have been established automatically between the previous and the current version.

It can be caused by 3 types of issues when we try to make the correspondences:

* **multiple mapping**: Several genes on the old sequence matched the same gene on the new sequence. It happens if the genes are identical (same best BLASTp possible match), you then have to chose which annotation to transfer to the gene on the new sequence.
* **Ambiguous mapping**: Two (or more) genes have the same stop codon but the identity between them is not good enough to report the annotation (the start codon is different). You have to check if the genes are the same and decide to report the annotation or not, adjust the start or not ...
* **No mapping**: no significant hit on the new sequence.

In order to solve these cases, the user have to manually check these CDS using specifics informations given in the different results tables and the gene information window.
