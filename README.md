``` sh
cd <espnet-root>/tools
$ ln -s <kaldi-root> .
```

``` sh
conda create -n espnet python=3.8
conda activate espnet
pip install -r requirements.txt -i https://pypi.tuna.tsinghua.edu.cn/simple
conda install pytorch=1.10.0 torchvision torchaudio=0.10.0 cudatoolkit=11.1 -c pytorch -c conda-forge
or pip install torch==1.10.0+cu113 torchaudio==0.10.0 -f "https://download.pytorch.org/whl/torch_stable.html"

./installers/install_chainer.sh <cuda_version>
```