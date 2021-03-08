# TSP Transformer
Feb, 2021
<br>
<br>



<img src="pic/tsp100.jpg" align="right" width="200" /> 


### Description
PyTorch implementation of "The Transformer Network for the Traveling Salesman Problem"<br>
Xavier Bresson and Thomas Laurent<br>
ArXiv : [https://arxiv.org/pdf/2103.03012.pdf](https://arxiv.org/pdf/2103.03012.pdf) <br>
Talk : [https://ipam.wistia.com/medias/0jrweluovs](https://ipam.wistia.com/medias/0jrweluovs) <br>
Slides : [https://t.co/ySxGiKtQL5](https://t.co/ySxGiKtQL5)<br>
<br>
<br>


### Installation

```
# Install conda
curl -o ~/miniconda.sh -O https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh 
chmod +x ~/miniconda.sh  # install conda  
./miniconda.sh  
source ~/.bashrc  

# GitHub repo
conda install git
git clone https://github.com/xbresson/TSP_Transformer.git # clone repo
cd TSP_Transformer
conda env create -f environment_gpu.yml # install python environment (CUDA 10.1)
conda activate tsp_transformer # activate environment
jupyter notebook # start jupyter notebook
```
<br>




### Results
1. Network Training (with RTX 2080 Ti 11GB) <br>
TSP50 (1 GPU) : Run notebook 'train_tsp_transformer_TSP50.ipynb'<br>
TSP100 (2 GPUs) : Run notebook 'train_tsp_transformer_TSP100.ipynb'<br>
2. Network Testing <br>
TSP50 : Run notebook 'test_tsp_transformer_beamsearch_TSP50.ipynb'. Optimality gap: -0.004%.<br>
TSP100 : Run notebook 'test_tsp_transformer_beamsearch_TSP100.ipynb'. Optimality gap: 0.371%.<br>
3. Visualization <br>
TSP50 : Run notebook 'visualization_TSP50.ipynb'<br>
TSP100 : Run notebook 'visualization_TSP100.ipynb'<br>
<br>



<br>
<br>
<br>


