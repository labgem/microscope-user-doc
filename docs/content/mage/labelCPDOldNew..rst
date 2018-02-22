################
Old » New Labels 
################

Only available for users having an account, i.e working on a MicroScope project with the LABGeM team.

Provides CDS label (i.e, locus_tag) correspondences between a new version of the genome being annotated/analysed (progression of the sequencing step) and the old one(s).

=================================
Report Methods
=================================
At the moment the report is only perform with CDS (and fCDS).

In order to report the annotation from the previous version of the sequence to the new one, we perform some analysis.

* 1- We use BLASTp between all the CDS automatically find in both sequences by the MicroScope annotation pipeline. We make a correspondence using the filter (pos>=100 and lrap=1 ) for the genes with the same length (AA) with Bidirectional Best Hits.
* 2- We perform a tBLASTn using genes which have been validated (annotated) or manually created by the user on the previous version of the sequence (if these genes have not pass the first BLAST filter) on the new sequence. We make a correspondence using the filter (pos>=100) for the genes with the same length (nucleic).


=================================
Manually report
=================================

In some case, for few genes, the correspondences may not have been establish automatically between the old and new version.


It can be cause by 3 types of issues when we try to make the corespondence:

* **multiple_hit**: Several genes on the old sequence matched the same gene on the new sequence. Happen if the genes are identical (same best BLAStp possible match), you have to chose which annotation to transfert to the gene on the new sequence.  
* **overlap**: Two (or more) genes have the same stop but the identity between them is not good enought to make the report. You have to check if the genes are the same and report the annotation or not.
* **no_cpd**: no significant hit on the new sequence.

In order to solve these cases, the user have to manually check these CDS using specifics informations given in the different results tables.
