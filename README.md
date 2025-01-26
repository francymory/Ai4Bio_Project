 # Ai4Bio_Project

Project for the course of AI for Bioinformatics.
Explainability of CONCH model for zero-shot classification of histopathological images.

# Manual:

  1. Make sure that the files to request the GPUs from the Unimore server have all the necessary permits to be executed:
 ```bash
 chmod 755 bash.sh
 chmod 755 start_jupyter.sh
 ```
     
 
  2. Add the CONCH directory and create a conda environment with all the necessary requirements:
    
```bash
git clone https://github.com/mahmoodlab/CONCH.git
cd CONCH
```

```bash
conda create -n conch python=3.10 -y
conda activate conch
pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
pip install --upgrade pip
pip install -e .
pip install matplotlib
pip install ipykernel
python -m ipykernel install --user --name=conch --display-name "Python (conch)"
```


 3. To start the Unimore GPU with a Jupyter notebook:
     
     -execute *./start_jupyter.sh* and copy the URL link.
    
     -on the notebook press *select kernel* and select an existing jupyter server, past the link and choose as kernel: *Python (conch)*. 

