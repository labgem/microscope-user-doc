.. _selector:

#############################
Sequence and Genome selection
#############################

Since version 3.13.0, **MicroScope** the selection of sequences and genomes is based on a new selector
that has been designed to allow interactive and efficient selection of several sequences or genomes
in large lists.
It features selection based on several criteria and suggestions.

In this section, selection of **Genome** means that you are going to select the entire organism including all the replicons.
Selection of **Sequence** means that you are going to select the replicon you want to work on.
When talking indistinctively of genomes or sequence, we use the term *object*.

Sequences and genomes come either from **MicroScope** (PkGDB) or from **NCBI RefSeq**.

There are two kinds of selectors in the platform (the :ref:`simple-selector` and the :ref:`advanced-selector`) which are described in the following sections.
Generally speaking a page use either a simple selector or 1 or 2 advanced ones.
However, some pages use several selectors (of any type), from **PkGDB** or **NCBI RefSeq**.
For instance, the :ref:`keywords` page use a simple selector in single mode and
an advanced selector in multiple mode.

.. _simple-selector:

***************
Simple Selector
***************

This selector is used to select a single genome based on the strain name.
It's similar to the old genome selector in MicroScope but offers suggestion.

This selector is used in the homepage to select the reference genome
and more generally in pages where you must select a reference genome (e.g. :ref:`lineplot`).

It is also used for instance in the following pages:

  - :ref:`pattern_searches`

When the page opens, the selector is displayed like this (it may take some time to load):

.. image:: img/simple_selector.png

Note that the exact appearance of this selector may depend on the page.

To select an organism, type in some characters of its strain name.
A list of organisms matching this characters will open.
From this list, you can select the organism you want.

For example, if you type "esche", the following list will open:

.. image:: img/simple_selector_esche.png

Note that the search is case-insensitive.

Also you can type any character (not just the beginning).
For example, if you type "k12", the following list will open:

.. image:: img/simple_selector_k12.png

.. _advanced-selector:

*****************
Advanced Selector
*****************

This selector is used to select one or several objects based on the NCBI taxonomy, strain name or :ref:`MICGC <micgc>`.

This selector is used for instance in the following pages:

  - :ref:`phyloprofile`
  - :ref:`blast_searches`
  - :ref:`genoclust`

Overview
========

When the page opens, the selector is displayed like below (it may take some time to load):

.. image:: img/selector_closed.png

To start selecting organisms click on the **Edit** button.
The selector opens as shown below:


.. image:: img/selector_partname.png

The window is divided in 5 parts:

  - the **Search Criterion** and **Search Field** are used to create filters on the list of objects from the data source; see :ref:`search-field-filters` for detailed explanation on those fields
  - the **Pre-selection Zone** is used to select objects among the objects that match the filters
  - the **Selection Zone** shows the list of currently selected objects
  - the **Add/Remove buttons** allows to transfer objects between the Pre-selection Zone and the Selection Zone

The general usage of the selectors is as follows.
You can use the **Search Criterion** and **Search Field** to filter
the list of all objects from the data source.

Filters can be constructed from:

 * the *Strain name* when selecting a genome or the *sequence* name when selecting a sequence
 * the *Taxonomy* of the organism
 * the *MICGC* to which the organism belong (see :ref:`MICGC <micgc>`)

See :ref:`search-field-filters` for detailled explanation on filters.

The **Pre-selection Zone** will display the objects that match the filters.
You can then select objects from this list and add them to the **Selection Zone** with the **Add Button** (green arrow).

If you want to remove objects from the **Selection Zone**, select them and use the **Remove Button** (red arrow).
See :ref:`selection-zone` to learn more about the **Selection Zone** (including the use of filters in it).

You can use the **Pre-selection Zone** several times with different filters.
This allows to create arbitrarily complicated selections.

When satisfied with the list in the **Selection Zone**, click on **Save**.
The selection window will close and you will return to the page you are interested in
for further analysis.

The **Reset** button will revert both zones (**Selection Zone** and **Pre-selection Zone**)
to their initial value (*i.e.* when the page was opened).
The selection window stays open so you can restart the selection.

The **Cancel** button button cancels all the changes done in the current selector
(*i.e* the list of selected organisms is not changed) and closes the selection window.

Example
=======

In this example, will we show how to select some organisms from the phylum Actinobacteria
and whose strain name contains some characters.

Select by taxonomy
------------------

The first step is to filter organisms in the Actinobacteria phylum.
To do so, opens the selector and select *Taxonomy* in the **Search Criterion**.
Then type "actinobacteria" in the **Search Field**.
You will notice that suggestions are shown as you type.

.. image:: img/advanced-selector-select-actinobacteria.png

The filters are shown in the drop down list.
In taxonomy mode, the filters can operate on any taxonomic level.
Click on "Actinobacteria".

The list of all organisms in the Actinobacteria phylum is then in the **Pre-selection Zone**. 

.. image:: img/advanced-selector-list-actinobacteria-genus.png

Note that the filter and the number of organisms filtered appear on the interface.
In this example, we have specified the phylum exactly.
Hence the filter is "phylum is 'Actinobacteria'".
See :ref:`filters` for more detailled explanations.

By default, organisms are grouped by Genus.
Use the "Display by" menu to group by phylum.

.. image:: img/advanced-selector-list-actinobacteria-phylum.png

Select by strain name
---------------------

We will now select organisms whose strain name contains "bifi".
To do so, select "Strain" in the **Search Criterion** and type "bifi" in the **Search Field**.

.. image:: img/advanced-selector-select-bifi.png

The list of organisms that match both filters is displayed:

.. image:: img/advanced-selector-list-bifi.png

Final selection
---------------

We can now select some organisms from the filtered list in **Pre-selection Zone**.
To do so, simply select one of them by clicking on it and click on the **Add Button**.

.. image:: img/advanced-selector-selection.png

As you can see, the number of organisms in the **Pre-selection Zone** is updated.
See :ref:`select-organisms-of-interest` for detailled description.

Congratulations, you have made your first advanced selection in MicroScope !
The rest of this page explains some details about the advanced selector.

Detailed description
====================

.. _search-field-filters:

The search field and the filters
--------------------------------

The **Search Criterion** allows to choose on which aspect you want to filter.
Typing in the **Search Field**, will bring suggestions.

* *Strain name*/*Sequence* filters by name of organism/sequence

  .. image:: img/selector_search.PNG

* *Taxonomy* filters by taxonomic information

  .. image:: img/selector_search2.PNG

Those suggestion are in fact filters.
There are 2 kinds of filters:

  - partial filter (shown in red in the image below): the genus must contain "Acinetobacter"
  - exact filter (shown in green in the image below): the genus must be exactly "Acinetobacter"

Pressing *enter* at any time in the **Search Field** creates partial filter.

.. image:: img/advanced_selector_search.png

Clicking on a filter will add it.

You can add several filters to improve the accuracy of your pre-selection.

To remove a filter, click on the little "x" next to its name.

What is the display menu?
-------------------------

By default, objects in the **Pre-selection Zone** and **Selection Zone** are grouped bu genus.
You can change this by changing the value of the display drop down menu.

.. image:: img/selector_display.PNG

The display by "species" with "Acinetobacter" filter active will group all pre-selected organism by species.

.. image:: img/selector_display2.PNG

The display by "genus" with "Acinetobacter" filter active will show all the 32 organisms in one single group.

.. _select-organisms-of-interest:

How to select my organisms of interest?
---------------------------------------

To select you organisms, move the mouse with the button down on the wanted organisms in the **Pre-selection Zone** (shift + click works too).
Then press the green button to put them in the **Selection Zone**.


.. tip::
   You can select the group of organism by double clicking on the bold tittle inside the **Pre-selection Zone**.

.. _selection-zone:

Selection Zone
--------------

The **Selection Zone** is there to allow you to see all the selected organisms for the analysis.
You can remove some of them by moving the mouse with the button down and pressing the red button to remove them from the **Selection Zone**.
If the active filter allow them, they will appear in the **Pre-selection Zone**.

When you are satisfied with your selection, press the save button to continue the analysis.

What is "Advanced filter"?
--------------------------

This part allow you to make filter in the **Selection Zone** to remove more efficiently organisms.
It works exactly the same as the first **search field**.
