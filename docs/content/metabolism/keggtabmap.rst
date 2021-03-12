
########
KEGG map
########

How to read the table?
----------------------

This table lists the genes associated with the given KEGG pathway, either by their annotated EC numbers or by their KO (KEGG Orthology) family.
KO families are predicted by the :ref:`mage_kofamscan` software.


.. image:: img/keggtabmap_table.PNG

* **Label**: Label of the gene. If you click on the label, you access to the Gene annotation window
* **Region**: '+' means the genes is present in the selected region the genome browser. ‘-‘ indicates that the gene is found elsewhere on the genome.
* **Gene**: The gene name
* **EC number**: annotated EC numbers for the gene 
* **Product**: Product description of the protein
* **Evidence**: Status of the annotation: "validated" means the gene is manually annotated and "automatic" means the gene annotation comes from automatic annotation procedure
* **KEGG map EC**: list of EC numbers with their description that are involved in the pathway
* **KO**: ID number of KEGG Ortholog family entry
* **KO Definition**: Functional description of the KO
* **KO EC number**: EC numbers associated with the KO

How to explore the KEGG map?
----------------------------

On the KEGG map, reactions matching gene annotations by their EC number or their predicted KO family are highlighted in yellow if the gene is present in the selected region of the genome browser or in green if the gene is found elsewhere on the genome.

.. image:: img/keggtabmap_map.PNG
