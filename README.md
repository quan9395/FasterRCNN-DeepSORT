# FasterRCNN-DeepSORT


## This project use mmtracking's repository to perform training and evaluation of Faster R-CNN and DeepSORT tracking algorithm. More infomation can be found at: https://github.com/open-mmlab/mmtracking

###Setup:

!pip install torch==1.10.0+cu111 torchvision==0.11.0+cu111 torchaudio==0.10.0 -f https://download.pytorch.org/whl/torch_stable.html

!pip install mmengine==0.1.0

!pip install 'mmcv==2.0.0rc1' -f https://download.openmmlab.com/mmcv/dist/cu111/torch1.10.0/index.html

!pip install 'mmdet==3.0.0rc2'

!git clone -b 1.x https://github.com/open-mmlab/mmtracking.git

%cd mmtracking

!pip install -r requirements/build.txt

!pip install -e .

!pip install git+https://github.com/JonathonLuiten/TrackEval.git

### Usage:
After cloning and install dependencies:

Testing:
#### single-gpu testing\
python tools/test.py ${CONFIG_FILE} [--checkpoint ${CHECKPOINT_FILE}] [--out ${RESULT_FILE}] [--eval ${EVAL_METRICS}]

example:
python tools/test.py configs/mot/tracktor/tracktor_faster-rcnn_r50_fpn_4e_mot17-public-half.py \
    --eval track

Training: 
python tools/train.py ${CONFIG_FILE} [optional arguments]\\


