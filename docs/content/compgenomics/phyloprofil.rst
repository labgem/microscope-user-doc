#################
Gene phyloprofile
#################

This interface allows the user to search for common OR specific genes/regions between a query genome and other genomes or replicons chosen from the ones available in our PkGDB database (i.e, (re)annotation of bacterial genomes) or complete proteome downloaded from the RefSeq/WGS sections.

How to read the interface?
--------------------------

.. image:: img/phyloprofile1.png

* **item A**: Use the «*Change*» button to set the reference genome that will be used for the comparison. The current reference genome is displayed as a subtitle at the top of the window.

* **item B**: Two modes are available, the *Organism* one, and the *Replicon* one.

	* use *Organism* mode to search within all replicons of the selected organisms
	* use *Replicon* mode to get the possibility to search within a specific replicon (chromosome/plasmid)
	
* **item C**: Use this form to search for genes in your reference genome which have homologs in other organisms/replicons coming from PkGDB and/or RefSeq databases.

* **item D**: Use this form to search for specific genes in your reference genome compared to a selection of organisms/replicons coming from PkGDB and/or RefSeq databases. 

.. tip:: You can mix the use of **item C** and **item D** to perform a very sensitive search. For example: get CDS of *Acinetobacter baylyi ADP1* (reference genome, item A) which have homologs in *Acinetobacter baumannii 6013113* and Acinetobacter baumannii AB0057 (item C), but **NO** homologs in *Acinetobacter baumannii AYE* (item D)

How to get genes with homologs in other organisms/replicons?
------------------------------------------------------------

.. image:: img/phyloprofile2.png

**Results**

.. image:: img/phyloprofile3.png


How to get specific genes of your reference genome compared to other organisms/replicons?
-----------------------------------------------------------------------------------------

.. image:: img/phyloprofile4.png

**Results**

.. image:: img/phyloprofile5.png


.. image:: img/phyloprofile6.png
