##############
Genome Browser
##############

==============================
Overview of the Genome Browser 
==============================

Organisation of the genomic map
-------------------------------

The MaGe genome browser is organised into 3 parts:

* the upper part of the window details the Coding Sequences (CDSs) that have been predicted for reading frames +1, +2 and +3 in the current region
* the middle part indicates the position of RNA objects (rRNA, tRNA, misc_RNA) as well as repeated regions (as turquoise rectangles) if any have been detected
* the bottom part of the window shows CDSs that have been predicted for reading frames -1, -2 and -3

The predicted CDSs are indicated by rectangles on each frame.

The blue lines symbolize the coding prediction curve. They increase when coding probability is high and drop when the coding probability is low.

.. image:: img/GB_overview1.png

What is the meaning of the Genomic Object color code ?
------------------------------------------------------

The rectangles symbolising each Genomic Object (CDS, RNA...) follow a color code that corresponds to their annotation status, summarized below:

.. image:: img/ColorCode_900.png

How to move along the sequence ?
--------------------------------

1) You can navigate along the selected sequence by using the grey arrows located on the left and right sides of the genomic map.
2) You can also enter directly a genomic coordinate and then click on **VIEW**.
3) Enter a gene name (e.g. dnaA) or a gene label (e.g., ECK0001) and click on **Move to**. The map is centered on the requested Genomic object. 
If several genes have been annotated with the same gene name, the window will move to the first occurrence of these genes on the genome sequence.

.. image:: img/img3.png

Why sometimes genes are framed with a black line?
-------------------------------------------------

.. image:: img/img4.png

This is a way to quickly identify a specific gene when annotator use the Move To functionalities:
* From result tables: 
.. image:: img/imgintermediaire.png

* From the toolbar below the synteny maps:
.. image:: img/img5.png

After a *Move To* action, the Genome Browser will be reloaded and centered around the corresponding gene, which will be framed with a black line.


How to read the table of annotated genomic objects ?
----------------------------------------------------

* **Sequence**: if you click on the DNA icon, it opens a new window with the sequences (nucleic and protein) of the genomic object
* **Label**: it gives you the label of the genomic object. If you click on it, the Gene Annotation Editor will popup for this Genomic Object
* **Type**: CDS, fCDS, tRNA, rRNA misc_RNA...
* **Gene**: gene name if any
* **Begin**: begin position of the genomic object on the sequence
* **End**: end position of the genomic object on the sequence
* **Length**: length of the genomic object, in nucleotides
* **Frame**: reading frame of the genomic object
* **Product**: description of the gene product of the genomic object
* **Matrix**: reference number for the matrix which has been used to predict the genomic object (see below)
* **Evidence**: automatic/validated/artefact // inprogress/finished/curated
* **AmiGene Status**: no/Wrong/New
* **GC content**: GC content of the sequence of the genomic object
* **GC3 content**: GC content on the 3rd position of the codons
* **CAI**: Codon Adaptation Index value
* **Mw**: Molecular weight in Daltons
* **Pi**: Isoelectric point
* **History**: Access to the annotation history of the genomic object

What is the Matrix ?
--------------------

For a given genome several gene Matrices can be built for gene detection. You can select a given matrix be using the Matrix menu located below the genomic map. Then click on View: the Coding prediction curves are updated.

How to access a gene’s information ?
------------------------------------

* 1) Enter a specific gene name or gene label into the right-most edit button below the genomic map, then click on Getinfo (opens an editable Genomic Object annotation window)
* 2) Click on a gene label in the table annotation editor (read-only window)
* 3) Click directly on a genomic object in the genomic map (editable annotation window)

How to access the annotation history of a genomic object ?
----------------------------------------------------------

Click on the **History icon** in located the table of genomic objects or in the Gene Annotation Editor window toolbar. 
The history opens in a new window, allowing you to follow the annotation’s evolution as well as the identity of previous annotators. You can send an email to an annotator by clicking on his/her login name.
.. image:: img/img6.png

How to use the "Export to Gene Cart" button ?
---------------------------------------------

The **Export to Gene Cart** button allows you to export all genomic objects contained in the genomic map to a Gene Cart. 
If you click on the button, a new window opens, offering the choice of creating a new cart or to selecting a pre-existing cart in which store the data. 
You can access to your gene carts via the Gene Cart Interface.

Can I create a new genomic object ?
-----------------------------------

The **NEW** button located below the genomic map allows you to create a new genomic object. If you click on the button, a Genomic Object Editor window opens. 
You have to manually fill in all fields to create your new object. You have to specify its Type, Begin, End, Frame, Mutation, Product, ... Then click on **SAVE**.

**Tips**:

* If you don’t have any modification rights on a sequence, the **SAVE** button is replaced by a **MAIL** button. In this case your proposition of a new genomic object is emailed to the project leader.
* Please note that you can’t delete a genomic object from the database.

Which program is used to detect the repeats ?
---------------------------------------------

Repeat detection is performed by the Repsek program.

*More*: http://wwwabi.snv.jussieu.fr/ public/RepSeek/

*Reference*: Achaz G, Boyer F, Rocha EP, Viari A, Coissac E. Repseek, a tool to retrieve approximate repeats from large DNA sequences. Bioinformatics. 2007 Jan1;23(1):119-21.

How to read the Repeat Regions table ?
--------------------------------------

* **Sequence**: Access to the nucleic sequence of the repeat region
* **Id**: Label of the repeat region on the replicon
* **Begin**: Begin of the region
* **End**: End of the region
* **Comments**: Number of repeat units contained in the repeat region

If you click on a repeat region label, you obtain the detailed list of the repeat units contained in the repeat region in a new window.

* **Sequence**: Access to the nucleic sequence of the repeat unit
* **Id**: Label of the repeat unit on the replicon
* **Type**: Type of repeat **Direct**, **Tandem** or **Overlap**
* **Strand**: Location of the repeat unit on the reverse **R** or direct **D** strand
* **Begin1**: Begin of the first unit
* **End1**: End of the first unit
* **Length1**: Length of the first unit in bp
* **Begin2**: Begin of the second unit
* **End2**: End of the second unit
* **Length2**: Length of the second unit in bp
* **Ident%**: Identity percentage between the 2 repeat units


