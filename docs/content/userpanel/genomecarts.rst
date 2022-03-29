.. TODO:
   Precise how to create them
   Add information in :ref:`advanced-selector` and how to select the favourite
   Remove favorites.rst and convert links/mentions (in particular in overview.rst and interface.rst)

.. _genomecarts:

############
Genome Carts
############

A « Genome Cart » is a (named) list of related genomes.
Genome carts are integrated in the :ref:`advanced-selector` (both for genome and sequence selection) to select them quickly.
The idea is that you can create your own groups of genomes (for instance for different projects).

Among those carts, you can (optionnally) choose a special one, called the « favourite » (this replace the list of favourite organisms found in previous versions).
This cart can be accessed quickly in some tools because they are integrated in the :ref:`advanced-selector`.

.. tip:: The content of genome carts is saved within your account settings, so it will persist even if you logout from your session.

.. warning:: For performance reasons, a genome cart can't contain more than 500 genomes.
    Also, you can't create more than 10 genome carts.

.. warning:: The name of the Genome Cart can not be longer than 30 characters.
     Also, only standard letters and numbers are allowed (it can't contain spaces and special characters) and the name can't contain only numbers.


.. _genomecarts-magic-carts:

***********
Magic carts
***********

Above the carts managed on this page, MicroScope maintains 2 « magic » carts:

* **My_Genomes:** This cart contains the genome of which you are **Administrator** (see :ref:`access-right-management`).
* **Recently_Used:** This cart contains the last 20 genomes used as reference.

Those carts are not displayed here (since their content is not editable) but they appear in the :ref:`advanced-selector`.
They can't be chosen as favourites.


*************************
Overview of the interface
*************************

The image below shows 2 carts (named **Test_Cart_1** and **Test_Cart_2** but you can choose better names).
Each cart is displayed in its own frame.
The name is displayed and can be edited with **Item 2** (see below) and **Item 3** indicates which cart (if any) is the current favourite and allow to change it.
The content of the carts is displayed and can be edited with an :ref:`advanced-selector` (**Item 6**).

.. image:: img/genomecarts.png


How to create a Genome Cart?
============================

The first way to create a Genome Cart is to click on the **NEW CART** button on top of the interface (**Item 1**).
This will create a new cart that you can edit with the selector.
The name of the new cart is **Cart_** plus a unique number.

Another way to create a cart is to copy an existing cart by clicking on the **COPY CART** button (**Item 4**).
The name of the new cart is formed by adding **_Copy** and a unique number to the name of the cart you copied.


How to edit a Genome Cart?
==========================

As mentionned, the content of the cart can be manipulated with the selector.
See :ref:`here <advanced-selector>` on how to do that.
This interface allows to easily manipulate cart content.
For instance, it's very easy to merge two carts: open the interface of a cart, select the cart you want to merge in
add it's content in the cart and save.


How to delete a Genome Cart?
============================

To delete a cart, simply press the **DELETE CART** button (**Item 5**).
A confirmation popup will appear.
Note that if you delete your favourite cart, you will have to choose a new one (see below).


How to rename a Genome Cart?
============================

To rename a cart, click on it's name in **Item 3**: a input area will be display so you can type in the new name and then press **OK** or **Cancel** as shown below.

.. image:: img/genomecarts_rename.png
   :align: center

If you enter an invalid name (according to the rules stated above), the cart won't be renamed as shown below:
<TODO>

.. _genomecarts-favourite-cart:

******************
The favourite cart
******************

As mentionned above one cart can be choosen as the favourite cart.
This cart is shown with a yellow star (see **Item 3**).

To select a new favourite, simply click on the star next to its name.

If you click on the star of the current favourite, it will be deselected (there won't be any favourite cart).
