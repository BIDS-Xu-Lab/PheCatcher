# PheCatcher
## Overview
This repository contains the code and resources for PheCatcher, a Information Extraction (IE) system designed to extract Phenotype, Code, and Coding System from biomedical literature.


## Environment
```bash
git clone https://github.com/BIDS-Xu-Lab/Kiwi-LLaMA.git
cd Kiwi-LLaMA
pip install -r requirements.txt
```

## Instruction Tuning
To instruction tune the model from scratch, you will have to specify your huggingface token in train.py, and run it by:
```bash
### set CUDA_VISIBLE_DEVICES to multiple GPU for multi-GPU training
CUDA_VISIBLE_DEVICES=0,1 accelerate launch train.py
```

## Inference
For inference, you will have to acquire model weights from https://kiwi.clinicalnlp.org/. Then specify the model directory in inference.py, and run it by:
```bash
python inference.py
```
