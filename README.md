 # Ai4Bio_Project

Project for the course of AI for Bioinformatics.
Explainability of CONCH model for zero-shot classification of histopathological images.

# Manual:
  1. To start the Unimore GPU with a Jupyter notebook:
     execute *./start_jupyter.sh* and copy the link and change the permissions. On the notebook select an existing jupyter notebook, past the link and choose a Python kernel. Now you can execute the notebook cells

  2. Add the CONCH directory and create a conda environment with all the necessary requirements:
    
```bash
git clone https://github.com/mahmoodlab/CONCH.git
cd CONCH
```

```bash
conda create -n conch python=3.10 -y
conda activate conch
pip install --upgrade pip
pip install -e .
```
