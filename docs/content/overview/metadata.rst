.. _metadata:

########
Metadata
########

.. TODO:
   We don't mention strain metadata for now because it's not in the public instance.
   Adding it require to change the title (without renaming the file), create dedicated sections.
   Links in :ref:`selector` should be OK.

A metadata is a piece of data used to define or describe another piece of data.
In the case of a genome, the data is the sequence(s) and the metadata can describe the shape of the cell, its motility, the temperature at which it grows best, the known metabolic pathways, etc.

This page presents the metadata available in MicroScope.
Those metadata can be used in the :ref:`advanced-selector` to select objects.
Note that we only support *qualitative* metadata for now.

.. _species_metadata:

****************
Species metadata
****************

Currently, there is only one source of metadata associated to the *species* of the genome (identified by its NCBI taxid).

Source of data
--------------

Species metadata are taken from `Joshua S. Madin et al., A synthesis of bacterial and archaeal phenotypic trait data. Sci Data 7, 170 (2020) <https://www.nature.com/articles/s41597-020-0497-4>`_.
This article unifies phenotypic and quantitative genomic traits from 26 sources.
The description of all available data can be seen `here <https://www.nature.com/articles/s41597-020-0497-4/tables/4>`_.
We use `version 1.2 <https://figshare.com/collections/A_synthesis_of_bacterial_and_archaeal_phenotypic_trait_data/4843290/3>`_.

Data
----

For our use, we have selected 9 qualitative metadata which are described in the table below:

.. list-table:: Selected metadata in MicroScope
   :widths: 20 48 42
   :header-rows: 1

   * - Trait name
     - Description
     - Exemple values
   * - Cell shape
     - The typical shape of cells
     - bacillus, coccobacilus, ...
   * - Gram stain
     - Gram positive or negative
     - Gram positive, Gram negative
   * - Motility
     - Capacity to move
     - motile/non motile, gliding, ...
   * - Sporulation
     - Can produce spores
     - sporulating/non sporulation
   * - Metabolism
     - Oxygen usage
     - aerobic, microaerophilic, ...
   * - Range tmp
     - Coarse environmental preference
     - mesophilic, psychrophilic, ...
   * - Range salinity
     - Coarse environmental preference
     - stenohaline, halophilic, euryhaline, ...
   * - Pathways
     - List of metabolic pathways undertaken
     - aerobic_anoxygenic_phototrophy, fermentation, nitrate_reduction, ...
   * - Isolation source
     - Where the microbe was sourced from
     - host, biofilm, soil, ...

See the reference for more precise description and the meaning of the values.
