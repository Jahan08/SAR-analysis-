Find the most common scaffold for a set of dataset
Pat walters used the [methods](https://pubs.acs.org/doi/pdf/10.1021/acsomega.8b03390) 

The method operates by carrying out three steps.

1. Decompose each molecule into a set of fragments. In this case we'll use the FragmentMol function from the Matched Molecular Pair Analysis (MMPA) functions in the RDKit decompose a molecule into a set of fragments. The RDKit MMPA methods use the Hussain and Rea methodology, which fragments a molecule by successively disconnecting acyclic single bonds.
2. Remove any fragments where the number of atoms is less than 2/3 the number of atoms in the original molecule.
3. Collect fragments and records their frequency. We can do this easily using the Pandas groupby method.

All of these functions have been encapsulated in a small python library called scaffold_finder. In this notebook, we'll use four functions from this library.

* generate_fragments - performs steps 1 and 2 above.
* find scaffolds - performs step 3 above
* cleanup_fragments - takes a set of fragments generated by steps 1 and 2 above, and coverts them to scaffolds
* get_molecules_with_scaffold - select molecules containing a specified fragment from a Pandas dataframe.

