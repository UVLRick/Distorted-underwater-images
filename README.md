# Distorted underwater image reconstruction
Pytorch implementation of the paper "Distorted underwater image reconstruction for an autonomous underwater vehicle based on a self-attention generative adversarial network"

Our network takes a distorted underwater image as an input and procude the corresponding sharp estimate. The model we use is GAN framework with group normalization + attention mechanism + RaLSGAN based on the conv3_3 layer before activation in the pre-trained VGG-16. Such architecture also gives good results on other image-to-image translation problems (deblurring, colorization, super resolution, inpainting, dehazing etc.)

# How to run
python 2.7
NVIDIA GPU + CUDA CuDNN (CPU untested, feedback appreciated)
Pytorch

To test the pretrained model, run: python main.py --test --exp-name both_L1VGGAdv3_3before_reluAteRa_gn2

# Datasets
The datasets are from http://www.image-net.org/ and http://cseweb.ucsd.edu/~viscomp/projects/WACV18Water/. 

# Citation
If you find our code helpful in your research or work please cite the paper.

@article{2020Distorted,
  title = {Distorted underwater image reconstruction for an autonomous underwater vehicle based on a self-attention generative adversarial network},
  author = {Tengyue Li, Qianqian Yang, Shenghui Rong, Long Chen, and Bo He},
  journal = {Applied Optics},
  eprint = {Vol.59, No.31},
  year = 2020
}

@inproceedings{2018Learning,
  title={Learning to See Through Turbulent Water},
  author={Zhengqin Li，Zak Murez，David Kriegman，Ravi Ramamoorthi，Manmohan Chandraker},
  booktitle={IEEE Winter Conference on Applications of Computer Vision},
  year={2018},
}

# Acknowledgments
The code borrows heavily from  "Learning to See through Turbulent Water" WACV 2018. The authors thank Dr. Zak Murez for constructive discussions.
