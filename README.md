```bash
conda create -n kg python=3.10
conda activate kg

nvcc --version
# Cuda compilation tools, release 12.4, V12.4.131
conda install cudatoolkit cuda-cudart cuda-nvtx cuda cuda-compiler -c nvidia -c conda-forge
conda install cudatoolkit cuda-cudart cuda-nvtx cuda cuda-compiler=12.4 -c nvidia -c conda-forge

conda install pytorch pytorch-cuda torchvision torchaudio -c pytorch
conda install pytorch pytorch-cuda=12.4 torchvision torchaudio -c pytorch

conda install sentence-transformers -c conda-forge

conda install datasets -c HuggingFace
conda install huggingface_hub transformers tokenizers datasets -c conda-forge
conda install azure-identity openai wandb rich accelerate evaluate nltk -c conda-forge

conda remove --name kg --all
conda clean --all -y
```

```bash
conda create -n uni python=3.10
conda activate uni

nvcc --version
# Cuda compilation tools, release 12.4, V12.4.131
conda install cudatoolkit cuda-cudart cuda-nvtx cuda cuda-compiler -c nvidia -c conda-forge
conda install cudatoolkit cuda-cudart cuda-nvtx cuda cuda-compiler=12.4 -c nvidia -c conda-forge

conda install pytorch pytorch-cuda torchvision torchaudio -c pytorch
conda install pytorch pytorch-cuda=12.4 torchvision torchaudio -c pytorch

conda install huggingface_hub transformers tokenizers datasets timm -c conda-forge

conda remove --name uni --all
conda clean --all -y
```
