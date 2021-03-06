#This repository houses the jupyter notebooks and code used to parse molecular dynamics and interaction data for downstream network analaysis. 

1. Ca-Ca analysis 
- convert.py is a script written by Tsjerk A. Wassenaar which is used to convert the .xpm adjecancy matrix output generated by the GROMACS mdmat command, to a numerical matrix in .csv format. The
HRP_network _analysis.ipynb can then be used to parse and merge the two matrices into an adjacency list to enable downstream analysis with Cytoscape. This notebook also contains a function to remove edges that are greater than 5.5angstroms apart and i+4 residues apart.  

2. Interaction analysis 
- Here, the concatenate_ring_results.ipynb is used to parse and merge RING 3.0 outputs which have already been converted from JSON to csv using Cytoscape. This output can then be re-imported to Cytoscape for visualization. This notebook also contains a function to remove contact frequencies that change by greater than 10% between simulations. 
