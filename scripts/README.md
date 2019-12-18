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

`targets_from_xml_selected_approved.csv`

`targets_from_xml_selected_experimental.csv`

`targets_from_xml_selected_none.csv`

#### What is it for
It parses the input files and exports `.csv` tables with all drugs, all targets and groups of selected targets. See the definition of each group of targets in `results` dir. It also creates some graphs but they are not exported as files.

### mapping.ipynb
#### Input
`targets_from_xml_selected.csv`

`filenames_mapping.csv`

`dn_ds_human_mouse_chimp.csv`

#### Output (only one at a time)
`dnds_for_targets.csv`

`dnds_for_targets_approved.csv`

`dnds_for_targets_experimental.csv`

`dnds_for_targets_none.csv`

#### What is it for
It merges all three file to produce a `.csv` table with all human genes with 1:1 orthologs in both mouse and chimpanzee, their dN/dS ratios and a column indicating whether or not they are present in **DrugBank** as targets. See the definition of each group of targets in `results` dir.

### visual_all.ipynb
#### Input
`dnds_for_targets(_/group/).csv`

#### Output
`/pictures/*png`

#### What is it for
It creates density plot + histogram graphs for each group of targets.  See the definition of each group of targets in `results` dir.
