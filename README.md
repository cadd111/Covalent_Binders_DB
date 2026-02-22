# Covalent_Binders_DB
A curated database of covalent binders (CBs) deposited in the Protein Data Bank (PDB).

## 01_CovDB.csv  
	- Identifiers of the covalent binders (LIGID)
	- SMILES notation
	- Molecular weight (MW)
        - Number of hydrogen bond acceptors (HBA) and donors (HBD)
	- Calculated logarithm of the octanol-water partition coefficient (logP)
	- Topological polar surface area (TPSA)
	- Fraction of sp3-hybridized carbon atoms (CSP3)
	- Number of rings (NumRings)
	- Number of heteroatoms (HetAtoms)
	- Number of rotatable bonds (RotBonds)
	- Values used for t-SNE, UMAP, and PCA plots
	
Each covalent binder is annotated to indicate whether it is a fragment, a FDA-approved drug (DrugBank ID), and/or present in the COCONUT database (COCONUT ID).

## 02_Warheads.csv
	- Identifiers of the covalent binders (LIGID)
	- Full (Warhead-01) and summarized (Warhead-02) warhead notation
	- InChI notation

## 03_Pairs.csv
Upon completion of the adducts derived from structures deposited in the PDB, several covalent binders were found to have more than one ligand identifier. 
This document lists the covalent binder IDs corresponding to shared structures. To avoid duplicates and ensure proper database curation, only the first identifier was retained (LIGID-01).

## 04_PDBs.csv
	- Covalent binder identifier (LIGID): The unique identifier assigned to each covalent ligand
	- PDB identifier (PDB): The Protein Data Bank code associated with the structure
	- Protein classification (CLASS)

    CLASS: hydrolases (HYD), transferases (TRF), oxidoreductases (OXI), lyases (LYA), isomerases (ISO), ligases (LIG), translocases (TRL), and non-enzymatic targets (OTR).

## 05_Alpha-hydroxysulfonic_to_Aldehyde.csv
The conversion of the α-hydroxysulfonic acid warhead to an aldehyde in some peptidomimetics resulted in identical structures being associated with different ligands reported under separate IDs. To standardize this, only one identifier was retained.
