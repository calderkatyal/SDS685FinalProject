# SDS685FinalProject
Final project repo for S&DS 685 at Yale

### Setup

Setup RL-VLM-F:
```
cd RL-VLM-F
conda env create -f conda_env.yml
conda activate rlvlmf
conda install -y pytorch==1.12.1 torchvision==0.13.1 torchaudio==0.12.1 cudatoolkit=11.3 -c pytorch  
pip install numpy==1.26.0
````

Setup r3m:
```
cd r3m
pip install -e .
```

Download additional requirements
```
pip install matplotlib scikit-learn
```

We use the cached VLM-generated labels provided by the [RL-VLM-F repository] (https://github.com/yufeiwang63/RL-VLM-F) for the Open Drawer task. Download seed_0, seed_1, and seed_2 from this [Google Drive link](https://drive.google.com/drive/folders/11LuzMXIk3dVMJZIiWA24bwjRlYUmY7li) and place each seed at ```RL-VLM-Fdata/cached_labels/Drawer/seed_{i}```. 

The jupyter notebook is at `src/project.ipynb`
