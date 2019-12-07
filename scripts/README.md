# SCRIPTS USED IN THE PROJECT
This directory includes all Jupyter notebooks used in the project.

### parsing.ipynb
#### Input
`drugbank_full_db.xml`

`dn_ds_human_mouse_chimp.csv`

#### Output
`drugs_from_xml_all.csv`

`targets_from_xml_all.csv`

`targets_from_xml_selected.csv`

#### What is it for
It parses the input files and exports `.csv` tables with all drugs, all targets and selected targets. It also creates some graphs but they are not exported as files.

### mapping.ipynb
#### Input
`targets_from_xml_selected.csv`

`filenames_mapping.csv`

`dn_ds_human_mouse_chimp.csv`

#### Output
`dnds_for_targets.csv`

#### What is it for
It merges all three file to produce a `.csv` table with all human genes with 1:1 orthologs in both mouse and chimpanzee, their dN/dS ratios and a column indicating whether or not they are present in **DrugBank** as targets.
