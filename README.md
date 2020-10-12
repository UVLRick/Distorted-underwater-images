# Distorted-underwater-images
The datasets are from http://www.image-net.org/ and http://cseweb.ucsd.edu/~viscomp/projects/WACV18Water/. 

To test the pretrained model, run: python main.py --test --exp-name both_L1VGGAdv3_3before_reluAteRa_gn2

If you find our code helpful in your research or work please cite the paper.

@article{2020,
  title = {Distorted underwater image reconstruction for an autonomous underwater vehicle based on a self-attention generative adversarial network},
  author = {Tengyue Li, Qianqian Yang, Shenghui Rong, Long Chen, and Bo He},
  journal = {Applied Optics},
  eprint = {Vol.59, No.31},
  year = 2020
}

@inproceedings{2018,
  title={"Learning to See through Turbulent Water",},
  author={ Kriegman, D },
  booktitle={IEEE Conference on Computer Vision & Pattern Recognition},
  year={2018},
}

Code borrows heavily from  "Learning to See through Turbulent Water" WACV 2018

The authors thank Dr. Zhen Zhang and Dr. Zak Murez for constructive discussions.
