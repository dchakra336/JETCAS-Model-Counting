# JETCAS-Model-Counting
Code for finding crossbar designs that perform edge detection, with approximate model counting

src/edge_detect_MC_JETCAS.py: This is the main file that searches for the crossbar designs based on a computed truth table, or a truth table read from a file. In case of the JETCAS paper, we have built a truth table based on truncated pixel pair distribution and saved it in a text file in the format False, True, A0, A1, ..., An, B0, B1, ..., Bn, !A0, !A1, ..., !An, !B0, !B1, ..., !Bn. This file is read and converted, for ease of use, to the format False, True, A0, !A0, B0, !B0, ..., An, !An, Bn, !Bn to be used in the model counting search.

src/new_tt_fgt3_16.txt: Contains the truth table in the above mentionned format. All pixel pairs with an intensity difference of more than 16, which occur more than thrice on an average in each image in BSD500, are a part of this truth table.

A .zip file (jetcas_all.zip) containing all other material used towards/for/in the JETCAS'19 paper is available at:
Please note that a subset of the files in jetcas_all.zip has been used towards/for/in the JETCAS'19 paper.
