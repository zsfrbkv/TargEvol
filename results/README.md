# OBTAINED TABLES, GRAPHS AND OTHER DATA
This directory contains all tables and graphs produced using scripts in `scripts/` directory.

## `drugs_from_xml_all.csv`
This table is an output of `parsing.ipynb`. It contains info on every drug present in `drugbank_full_db.xml` (name, approval status, mass and number of targets). 

## `targets_from_xml_all.csv`
This table is an output of `parsing.ipynb`. It contains info on every target present in `drugbank_full_db.xml` (name, organism, GenBank ID, UniProt ID, drugs names and their number).

## `targets_from_xml_selected.csv`
As previous, but includes only Human targets with drugs with mass > 100. 

## `dnds_for_targets.csv`
This table is an output of `mapping.ipynb`. It is basically `drugs_from_xml_all.csv` merged with `targets_from_xml_selected.csv` (and `filenames_mapping.csv`). It contains info on every gene present in `drugs_from_xml_all.csv` (gene name, gene description, dN/dS with Chimpanzee, dN/dS with Mouse and whether it is present in `targets_from_xml_selected.csv` or not). 


