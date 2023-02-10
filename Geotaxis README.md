# Geotaxis 
Assay: Flies are knocked to the bottom of a vial, and the distance climbed in several seconds (typically 5) is measured.

Output Folder: A .xlsx file with a sheet for each experiment processed. Each sheet contains the results of a nested random effects model, which includes summary statistics (most notably mean and standard error) and pairwise comparisons between conditions (including p values).

Flies are scored with an integer 0 to 6 (including 0 and 6) indicated how high they climbed.

Each vial of flies is assayed 3-4 times: After 4 assays, they begin to get tired.

Each set indicates up to 7 vials of flies, with each vial stored in a unique column.

Each replicate indicates an indivual assay of a set of flies. The values measured for a replicate are all measured on the same 7 rows.

Additional metadata can be stored below the last replicate, including an average score for each vial.

See comments in the code for instructions on altering variables for each analysis. 

As long as the template is not altered, only the first 2 variables need to be adjusted. If adding replicates beyond the 4 in the template, maxReps is the only additional variable that needs to be adjusted, so long as the structure of the template is preserved.
