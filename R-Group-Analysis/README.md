In this notebook, we will use an R-group decomposition to perform exploratory data analysis on a dataset from the ChEMBL database. We will define a common scaffold for a set of molecules and use the function rdRGroupDecomposition.RGroupDecompose from the RDKit to create a table of substituents attached at different positions on the scaffold.
To perform this analysis, we will carry out the following steps.

1. Read the input data from a SMILES file
2. Cluster the input data to identify similar molecules
3. View the largest cluster and identify the common scaffold
4. Perform the R-group decomposition
5. View the R-groups and their frequency
