# FasterRCNN-DeepSORT
Setup

!pip install torch==1.10.0+cu111 torchvision==0.11.0+cu111 torchaudio==0.10.0 -f https://download.pytorch.org/whl/torch_stable.html
!pip install mmengine==0.1.0
!pip install 'mmcv==2.0.0rc1' -f https://download.openmmlab.com/mmcv/dist/cu111/torch1.10.0/index.html
!pip install 'mmdet==3.0.0rc2'
!git clone -b 1.x https://github.com/open-mmlab/mmtracking.git
%cd mmtracking
!pip install -r requirements/build.txt
!pip install -e .
!pip install git+https://github.com/JonathonLuiten/TrackEval.git
