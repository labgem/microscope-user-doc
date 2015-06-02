########################
Access Rights Management
########################

This interface is made for« Organism Administrators » and allows management of users access rights on organisms.

.. note:: **Only annotators defined as «Organism Administrators» are allowed to use this functionality. By default, «Organism Administrators» are users who submit a Delivery of Service asking for a Genome integration into MicroScope: when the organism is delivered by LABGeM team on the MicroScope platform, the Delivery of service submitter is set with an additionnal access right, that will allow him to manage access rights of other users on corresponding organisms**


How to read the interface?
--------------------------

.. image:: img/man1.png

Two display modes are available:

* the first one (default one), «**Order by Organisms**», will display all organisms for which the user have administration rights. Each organism, for which you are administrator, has a status called «**Private**» or «**Public**»:

	* «**Public**» status means everyone will have «View Only» access rights on the corresponding organism/sequences in MicroScope. Other access rights, such like «View & Annotate» access rights will need to be granted to users by an administrator.
	* «**Private**» status means that only people having access rights granted by an administrator will be able to «View» or «Annotate» the organism / sequence.

* the second one, «Order by Users», will list all the users that have access to organisms belonging to the administrator.

.. note:: «**Private**» or «**Public**» status are currently set by LABGeM team. By default we set the status this way:

	* If the organism is a new sequenced one, we will set the status to «**Private**» when we deliver the data on MicroScope, and we will give «Administrator» access level to the submitter of the corresponding Delivery of Service.
	* If the organism is coming from a public databank (RefSeq sequence, for example), the default status will be «**Public**», and no one will be set as «Administrator», except if you plan to re-annotate the organism (in this case, you have to contact us)

If you click on the *down arrow* on the left of an organism / user name, you will display the details about access rights on this organism / of this user.


What are the different Access Rights?
-------------------------------------

For now, we provide 4 main access rights levels:

* «**Administrator**» : this level is the higher one. Administrator will have full management rights on the organism. Administrator will be able to set access rights for other people. Note that you can set several Administrators on a same organism. Also, Administrator have annotation access rights on their organisms.
* «**View & Annotate**»: users having this access rights level, will only be able to «Annotate» and «View» the organism and the corresponding data on MicroScope.
* «**View Only**»: this level is the basic one. People having view access rights will not be able to annotate a sequence. Please note that for a «Public» organism, everyone has «View Only» access rights. For «Private» organisms, an administrator will need to give a «View» access rights to users.
* «**Remove**»: will delete the access rights of a given user.


How to Change Access Rights?
----------------------------

To change the user access rights, simply select the desired access level from the select menu, then the update will be performed automatically.

* «**Order by Organisms**» View

.. image:: img/man2.png

All users having access to the corresponding organism are grouped by access right level: firest, **Administrators**, then users having **View & Annotate** access rights and at the end, users having View Only access rights.

*Additional data about users are also available:*

	* *User name*
	* *User email*
	* *User account creation date*
	* *User last login date on MicroScope (and not necessarly on the organism you are looking at)*
	* *the last date the user access rights has been modified by an administrator*

* «**Order by Users**» View

.. image:: img/man3.png

For a given user, will be listed all the organisms for which:

	* user have access rights
	* you have administrator access level

Please note that an user may have also access rights for organisms you are not administrator of. In this case, corresponding orgainsms will not be displayed.

*Additional data are also available:*

	* *Organism name*
	* *related sequences (chromosomes, plasmids)*
	* *Organism status (private/public)*
	* *the last date the user access rights has been modified by an administrator*

.. note:: There is some restrictions about access rights an administrator can select:

	* an administrator can not change is own access rights. If an administrator, for some reasons, wants to drop his access level, he will need to set administrator access rights to another user. Then, this user will be allowed to drop the access level of the first administrator.
	* an administrator can not set a «View Only» access right to users on «Public» organisms, since these organisms are accessible for everyone.
	
	
How to give Access Rights to a new user?
----------------------------------------

To add new access rights to a new user, or set a same access rights to several organisms or users, click on the green button called «**+ Add New Access Rights**»

Then, you will be redirected into another interface with 3 steps:

.. image:: img/man4.png

* **Step 1**: this menu will list all the organisms you are administrator of. Select all the organisms for which you want to grant access rights.
* **Step 2**: this menu will list all the users that currently have access rights on the organisms you are administrator of. Select all the users for who you want to update access rights. If an user is missing in this list, you can add him by filling the upper field and click on «**ADD NEW USER**» button. You will have to **fill the field with the user email address used for his account creation**. So, be sure that people have already a MicroScope account before trying to give them access rights on your organisms.
* **Step 3**: select the access level you want to give to your selection. Then save.
