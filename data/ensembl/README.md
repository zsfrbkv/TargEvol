# ENSEMBL DATA
This repo contains all initial data downloaded from **Ensembl** database using **BioMart** (https://www.ensembl.org/biomart/martview/84419c3f598a9c1f51de0559a5041297).

### dn_ds_human_mouse_chimp.csv
This table contains all Human genes, their corresponding orthologs in Mouse and Chimpanzee as well as pre-calculated dN and dS. 

To download this table using BioMart select 'Ensembl Genes 98' => 'Human genes (GRCh38.p13)'. Then go to 'Attributes' and select 'Homologues'. Click on 'GENE' and uncheck 'Gene stable ID version', 'Transcript stable ID', 'Transcript stable ID version' and check 'Gene description' and 'Gene name'. Then click on 'ORTHOLOGUES (Max select 6 orthologues)', find 'Chimpanzee Orthologues' and 'Mouse Orthologues' and check '<Chimpanzee/Mouse> gene name', 'dN with <Chimpanzee/Mouse>' and 'dS with <Chimpanzee/Mouse>'. Finally, go to 'Results' => 'Export  all results to' => 'Go'.

### filenames_mapping.csv
Table with 'Gene stable ID' mapped to 'UniProtKB Gene Name ID'. The was used to merge `dn_ds_human_mouse_chimp.csv` with `targets_from_xml_selected.csv`. 

To download this table using BioMart select 'Ensembl Genes 98' => 'Human genes (GRCh38.p13)'. Then go to 'Attributes', click on 'GENE' and uncheck 'Gene stable ID version', 'Transcript stable ID', 'Transcript stable ID version'. Then click on 'EXTERNAL', find 'External References (max 3)' and check 'UniProtKB Gene Name ID'. Finally, go to 'Results' => 'Export all results to', select 'CSV' and click 'Go'.

### filenames_mapping_unique.csv
As previous but with 'Unique results only' checked.
