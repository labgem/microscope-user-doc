######################
Integron
######################

What are Integrons and IntegronFinder?
-------------------------------------------------------

Integrons are versatile gene acquisition systems commonly found in bacterial genomes. They are ancient elements that are a hot spot for genomic complexity, generating phenotypic diversity and shaping adaptive responses.
Integrons are composed of three essential core features:

•	intI : a gene which encodes for an integron integrase whose protein catalyzes recombination between incoming gene cassettes and the second feature, an integron-associated recombination site.
•	attI : attachment integrase is a proximal recombination site which is recognized by the integrase and at which gene cassettes may be inserted.
•	Pc: a promoter which directs transcription of a cassette-encoded gene.

Integrons acquire new genes as part of gene cassettes. These are simple structures, usually consisting of a single open reading frame (ORF) bounded by a cassette-associated recombination site known as attC.
Circular gene cassettes are integrated by site-specific recombination between attI and attC, a process mediated by the intI. This process is reversible, and cassettes can be excised as free circular DNA elements.
Insertion at the attI site allows expression of an incoming cassettte, driven by the adjacent Pc promoter.


.. image:: img/integronfunctionning.png

IntegronFinder is a tool that detects integrons in DNA sequences with high accuracy. It is accurate because it combines the use of HMM profiles for the dectection of essential protein, the site-specific integron integrase, and the use of Covariance Models for the detection of the recombination site, the attC site.
This tool also annotates gene casettes however we use our own annotations to make it run.
IntegronFinder distinguishes 3 types of elements:

•	Complete integron: integron with integron integrase nearby attC site(s)
•	In0 element: integron integrase only, without any attC site nearby
•	CALIN element: Cluster of attC sites Lacking INtegrase nearby. A rule of thumb to avoid false positive is to filter out singleton of attC site.

.. image:: img/IFelements.png

|

Know more about `Integrons <https://www.researchgate.net/publication/262533269_Integrons_Past_Present_and_Future>`_

Know more about `IntegronFinder <http://integronfinder.readthedocs.io/en/latest/>`_

|

**References:**

|

`Gillings MR. 2014. Integrons: past, present, and future<http://mmbr.asm.org/content/78/2/257.full.pdf+html?sid=37df918b-9e26-4064-83a8-1576a4012c7d>`. Microbiol Mol Biol Rev 78:257–277. 10.1128/MMBR.00056-13.

`Identification and analysis of integrons and cassette arrays in bacterial genomes<https://academic.oup.com/nar/article/44/10/4539/2516972/Identification-and-analysis-of-integrons-and>`. Jean Cury; Thomas Jove; Marie Touchon; Bertrand Neron; Eduardo PC Rocha. Nucleic Acids Research 2016;
doi: 10.1093/nar/gkw319

How to access to Integrons data ?
-------------------------------------------------------

IntegronFinder predictions are available through the Comparative Genomics section, in the main navigation menu.

#TO BE CONTINUED
