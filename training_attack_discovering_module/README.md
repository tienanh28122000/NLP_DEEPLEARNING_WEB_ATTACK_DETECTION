# Attack Discovering Module

## Tutorial for training

1. Install Anaconda or Miniconda Package Manager from [here](https://www.anaconda.com/distribution/)
2. Create a new virtual environment and install packages.
```bash
conda create -n attack_discovering python pandas tqdm
conda activate attack_discovering
```
3. Install simpletransformers library
```bash
pip install 'git+https://github.com/bit-ml/date.git#egg=simpletransformers&subdirectory=simpletransformers'
```
4. Prepare the training and testing dataset
- Excecute the file [web_attack_dataset/preprocess.ipynb](web_attack_dataset/preprocess.ipynb)
5. Train the model (We can track the training progress by using Tensorboard)
```bash
cd experiments
python train_ag.py
```

Note: Read carefully the hyper-parameters in training file and fine-tune these params to get the best result



