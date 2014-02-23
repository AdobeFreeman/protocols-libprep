.. include:: global.rst
..  _Adapters:

*********
Adapters
*********

TruSeq v3-style adapters (e.g. BFIDT-xxx)
==========================================

If you are using custom TruSeq-style sequencing adapters (i.e., not the standard
Illumina TruSeq adapters and something similar to those adapters in [Fair2012]_)
and you have ordered both indexed oligos and a universal oligo from IDT, you
need make indexed adapters from the indexed oligo + universal oligo.  This means
combining one indexed oligo with the universal oligo, and annealing those to
make double- stranded adapters.  You need to do this for all adapters you will
use, and it is best/easiest to do this in a PCR plate.

#. Assemble the following components to make Oligo Buffer:

    +--------------------------------------+---------+
    | 1X TE (10 mM Tris pH 8.0, 1 mM EDTA) | 9.9 mL  |
    +--------------------------------------+---------+
    | 5 M NaCl                             | 0.1 mL  |
    +======================================+=========+
    | Total                                | 10.0 mL |
    +--------------------------------------+---------+

#. Using the Oligo Buffer from above, assemble the following components to
   create the adapters:

    +---------------------------------+----------+
    | Oligo Buffer                    | 50.0 µL  |
    +---------------------------------+----------+
    | 100 uM TruSeq Universal Adapter | 25.0 µL  |
    +---------------------------------+----------+
    | 100 uM TruSeq Indexed Adapter   | 25.0 µL  |
    +=================================+==========+
    | Total                           | 100.0 µL |
    +---------------------------------+----------+

#. Anneal:

    * 95 C for 1 minute
    * -0.1 C/sec for each of 800 seconds (~13 minutes)
    * 14 C hold

#. Store adapters at -20 C.
