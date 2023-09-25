# FasterRCNN-DeepSORT
Setup
# install pytorch
!pip install torch==1.10.0+cu111 torchvision==0.11.0+cu111 torchaudio==0.10.0 -f https://download.pytorch.org/whl/torch_stable.html

# install MMEngine
!pip install mmengine==0.1.0
# install MMCV
# !pip install mmcv-full
!pip install 'mmcv==2.0.0rc1' -f https://download.openmmlab.com/mmcv/dist/cu111/torch1.10.0/index.html

# install MMDetection
!pip install 'mmdet==3.0.0rc2'

# clone the MMTracking repository
!git clone -b 1.x https://github.com/open-mmlab/mmtracking.git
%cd mmtracking

# install MMTracking and its dependencies
!pip install -r requirements/build.txt
!pip install -e .
# used to MOT evaluation
!pip install git+https://github.com/JonathonLuiten/TrackEval.git
