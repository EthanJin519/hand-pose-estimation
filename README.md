
# Domain Adaptative hand pose Estimation Based on self-looping adversarial training strategy


# Installation

 python_requires='>=3.6'

 Install_requires:

  	 'torch>=1.7.0',
  	 'torchvision>=0.5.0',
  	 'numpy',
  	 'prettytable',
 	  'tqdm',
 	  'scikit-learn',
 	  'webcolors',
 	  'matplotlib'.
     
# Datasets

 [Rendered Handpose Dataset](https://lmb.informatik.uni-freiburg.de/resources/datasets/RenderedHandposeDataset.en.html) (synthetic dataset)
 
 [Hand-3d-Studio Dataset](https://www.yangangwang.com/papers/ZHAO-H3S-2020-02.html) (real-word dataset)
 
 [Stereo Hand Pose Tracking Benchmark](https://www.dropbox.com/sh/ve1yoar9fwrusz0/AAAfu7Fo4NqUB7Dn9AiN8pCca?dl=0) (real-world dataset) 



 #  Trained models
 
 The trained models can be found [here](https://drive.google.com/drive/folders/1xLc20jBd5cchIysYYEN6mXKZZN2u0fAa?usp=sharing).

 
 
 # Run the code
 
 1. Evaluate on real-world dataset (H3D or STB).
    ```
    python test.py data/H3D -t Hand3DStudio --checkpoint  models/H3D_test.pth,
    python test.py data/STB -t STB --checkpoint  models/STB_test.pth
    ```
   
   
 2. Training.
    
    Run the following script:
    ```
    python train.py data/H3D -t Hand3DStudio
    python train.py data/STB -t STB
    ```
   
  
