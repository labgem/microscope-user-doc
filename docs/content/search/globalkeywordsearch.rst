.. _globalkeywordsearch:

#####################
Global Keyword Search
#####################

This tool allows You to search genes througout all of your Genomic Datas with keywords.

***********************
How to perform a search
***********************
SCREENSHOT
1. Select one or more words to search
2. Select which type of dataset you want to search
3. Click on the "Send" button or push Enter on your keyboard
.. Warning::
    **Warning**: Researches can take up to several minutes, do not leave the page!

****************************
Elements searched by dataset
****************************
/In the Koala And Interpro dataset you can only search for there ID numbers

Genomic Object:

- Gene Name\ :sup:`*`: Name of the Gene
- Synonym\ :sup:`*`: alternative name for the gene
- EC number\ :sup:`*`: EC (Enzyme Commission) number associated with the protein
- Reaction\ :sup:`*`: gives the reactions implying the database protein (reactions given by Rhea and MetaCyc)
- Label: Label of the genomic object
- Product: product description of the protein
\ :sup:`*` Optional fields

**************************
Search Operators available
**************************

The Global Keyword Search allows the use of special operators to construct advanced research queries.
These operators must be placed before the word concerned by it.

The operators available are as follow

+-------------+-----------------------------------------------+--------------------------------------------------------------------------------------------+
| Operator    | Description                                   | Example                                                                                    |
+=============+===============================================+============================================================================================+
|**+**        | Include, the word must be present.            | | '+helicase +putative' find results with both words in it.                                |
|             |                                               | '+helicase putative' find results with "helicase" but thos with "putative" will also be    |
|             |                                               | first displayed.                                                                           |
+-------------+-----------------------------------------------+---------------------------------------+----------------------------------------------------+
|**-**        | Exclude, the word must not be present.        | 'helicase -putative' find results with "helicase" but not "putative"                       |
+-------------+-----------------------------------------------+--------------------------------------------------------------------------------------------+
|(no operator)| By default, the word is optional,             | 'helicase putative' find results with at least one of the word in it and display those     |
|             | but the results that contains it will         | which have both of them first                                                              |
|             | be displayed first                            |                                                                                            |
+-------------+-----------------------------------------------+--------------------------------------------------------------------------------------------+
|**~**        | Act as a negation operator, results           | 'helicase ~putative' find results with "helicase" in it, if the results also contain       | 
|             | containing this word will be displayed last   | 'putative', it will be shown last                                                          |
+-------------+-----------------------------------------------+--------------------------------------------------------------------------------------------+
|**\***       | Wildcard operator. Unlike the other operators,| 'dna*' find results which contain "dnaA", "dnaB", "dnase" etc...                           |
|             | **it is appended to the word** to be affected.|                                                                                            |
|             | Words match if they begin with the word       |                                                                                            |
|             | preceding the * operator.                     |                                                                                            |
+-------------+-----------------------------------------------+--------------------------------------------------------------------------------------------+
|" "          | A phrase that is enclosed within double quote | '"putative helicase"' find results that contain the exact phrase 'putative helicase'       |
|             | characters matches only rows that contain     | but not 'helicase putative'                                                                |
|             | the phrase literally, as it was typed.        |                                                                                            |
+-------------+-----------------------------------------------+--------------------------------------------------------------------------------------------+

***************************
How to export the results ?
***************************
SCREENSHOT
You can export all your results in a gene cart by clicking the **Export to gene cart** button or export them in a csv file with the coresponding button (2)