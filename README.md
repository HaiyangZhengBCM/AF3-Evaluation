# AF3-Evaluation
Repository for AlphaFold3 in Drug Discovery: A Comprehensive Assessment of Capabilities, Limitations, and Applications.

# analyze_interactions_from_schrodinger.ipynb - use environment_analysis-struct.yml
This script process protein-ligand interaction result files from Schrodinger Maestro's script poseviewer_interactions.py for real structures and their corresponding AlphaFold3 predicted structures. This script compare the structures, identify the residue number matchings, and then compare the protein-ligand interactions between the real and AF3 predicted structures. Demo data for this script has been included in demo_data folder.

# binary_interactions.ipynb - use environment_analysis-struct.yml
This script calculates protein RMSD and ligand RMSD between AlphaFold3 predictions and real structures. A folder containing Chai-1 model's predictions and all intermediate file has been uploaded in demo_data folder.

# CaSR_evaluation.ipynb - use environment_analysis-struct.yml
This script calculates the protein RMSD for CaSR prediction evaluation.

# gnina_docking.ipynb - use environment_openmm_docking.yml
This script contains gnina docking workflow we adopted in various of our analysis. To use GNINA, please install GNINA Docker image: docker pull gnina/gnina. A demo structure file 3ant.cif andd its corresponding result log file has been included in demo_data folder.

# input_compile.ipynb - use environment_AF3.yml
This script contains the AF3 input file compilation functions that we used. Example use has been included in the script.

# ternary_ppi.ipynb - use ternary_ppi_environment.yml + Schordinger Installed by SBGrid
This script runs Schrodinger Maestro's protein_interaction_analysis.py and conduct comparison between real structures and AF3 predicted structrues. Similar to analyze_interactions_from_schrodinger.ipynb, this script contains a methhod that establish the sequence mapping between protein structures, but this time with a chain ID for the mapping. Examples of Schrodinger's script output has been included in demo_data folder. The authors are requesting permission from DeepMind to publish AF3 predicted structures before official publication of this manuscript. Once the permission is granted, we will upload demo structures for this function. 

# Installation
To use scripts from this repository, build the environment with the corresponding .yml. 