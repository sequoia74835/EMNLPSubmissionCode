# README

This repo is created for reproducibility purpose.

The captioning model is modified from https://github.com/salaniz/pytorch-gve-lrcn

The installation guide comes from Salaniz repo, the data downloading link is provided from the original repo. 

## Installation
This implementation uses Python 3, PyTorch and pycocoevalcap (https://github.com/salaniz/pycocoevalcap).  
All dependencies can be installed into a conda environment with the provided environment.yml file.

1.Clone the repository
```shell
git clone https://github.com/sequoia74835/EMNLPSubmissionCode.git
cd EMNLPSubmissionCode
```
2.Create conda environment
```shell
conda env create -f environment.yml
```
3.Activate environment
```shell
conda activate gve-lrcn
```

4.Download pre-trained model and data
```bash
sh rsa-file-setup.sh 
```

5. Install other packages

```bash
pip install -r requirements.txt
```

## Interactive

We provide a demo Jupyter Notebook for loading and running the model!

Once you installed the Conda Environment, you need to add it to the Jupyter Kernel:

```bash
conda activate gve-lrcn
conda install ipykernel
python -m ipykernel install --user --name=gve-lrcn
```

If you don't see "gve-lrcn" in your "Change kernel" drop-down manual, you may need to kill your previous Jupyter Notebook and rerun the command:

```bash
jupyter notebook
```