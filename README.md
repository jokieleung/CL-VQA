# Source Code for "Learning to Contrast the Counterfactual Samples for Robust Visual Question Answering"
The source code for our paper "Learning to Contrast the Counterfactual Samples for Robust Visual Question Answering". This repo contains code modified from [here](https://github.com/yanxinzju/CSS-VQA), Thx for their efforts.

### Prerequisites

Make sure you are on a machine with a NVIDIA GPU and Python 2.7 with about 100 GB disk space. <br>
h5py==2.10.0 <br>
pytorch==1.1.0 <br>
Click==7.0 <br>
numpy==1.16.5 <br>
tqdm==4.35.0 <br>

### Data Setup
All data preprocess and set up please refer to [bottom-up-attention-vqa](https://github.com/hengyuan-hu/bottom-up-attention-vqa)

1. Please run the script to download the data.

```
bash tools/download.sh
```

2. Please run the script to preprocess the data.

```
bash tools/download.sh
```



### Training

All the args for running our code is preset in the main.py.

Run
```
CUDA_VISIBLE_DEVICES=0 python main.py
```
to train a model

### Testing
Run
```
CUDA_VISIBLE_DEVICES=0 python eval.py --dataset [] --debias [] --model_state []
```
to eval a model
