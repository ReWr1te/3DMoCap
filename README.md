# 3DMoCap

This is an integration of methods to predict 3D human pose from ordinary videos and translate the poses into BVH MoCap files.

![result](mocap-data/result.gif)

Currently only support videos that the camera set at the front of (parallel with the ground) only 1 person, and no actions which contain depth.

Basic codes from:

https://github.com/facebookresearch/VideoPose3D

https://github.com/Dosomecrazy/video2bvh

# Requirements

GPU: > RTX2060S, CUDA10.0, 10.1, 10.2 recommended.

1. Linux (Ubuntu1604 tested)
2. Python 3.6
3. CUDA, cuDNN and corresponding PyTorch >=1.4 (CUDA10.2, CUdnn7.6.5, PyTorch1.6 tested)
4. detectron2
5. conda environment, Python3.6, ffmpeg, h5py, opencv-python, jupyter, (nb_conda_kernels)

# PyTorch

See https://pytorch.org/get-started/locally/ for installation guides for various environments.

# detectron2

See https://github.com/facebookresearch/detectron2/blob/master/INSTALL.md for installation guides for various environments.

# conda environment

`conda create -n 3DMoCap python=3.6 pip -y`

`conda activate 3DMoCap`

`pip install torch torchvision` (for CUDA10.2, PyTorch1.6)

```
python -m pip install detectron2 -f 
  https://dl.fbaipublicfiles.com/detectron2/wheels/cu102/torch1.6/index.html
```

(for PyTorch1.6)

`conda install ffmpeg -y`

`pip install h5py opencv-python jupyter`

# Installation

Download or git clone this repo.

# Get Started

Follow demo.ipynb.