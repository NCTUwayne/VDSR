# VDSR
NCTU VRDL HW4
## Hardware
* Ubuntu 16.04 LTS
* Intel(R) Core(TM) i7-6700 CPU @ 3.40GHz
* NVIDIA TitanX
## Dataset
* 291 trianing images
* 14 testing images
## Requirements
* torch
* torchvision
* matplotlib
* numpy
* sicpy=1.3.1
## Data preprocessing
Run generate_train.m in data file. If the process is too slow try to split your training data.
## Training
    python main_vdsr.py --cuda --gpus 0    
## Generate output
Resize the test images by 3x

    python eval.py --model model/model_epoch_50.pth --imgname --cuda
## Reference
https://github.com/twtygqyy/pytorch-vdsr
