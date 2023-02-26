#  Texture-based Error Analysis for Image Super-Resolution (CVPR 22).
[Paper](https://openaccess.thecvf.com/content/CVPR2022/papers/Magid_Texture-Based_Error_Analysis_for_Image_Super-Resolution_CVPR_2022_paper.pdf)

#### First generate the corrupted DIV2K LR_bicubic using this [bicubic interpolator implementation](https://github.com/sanghyun-son/bicubic_pytorch). 
Since we are using python and need to use bicubic upsampling for some of our experiments, we regenerate the low resolution DIV2K images. When you download the original DIV2K images, you will find the matlab corrupted LRs. Ignore those. Instead use the [preprocessing notebook](https://github.com/sabdelmagid/CVPR22-TextureBasedError-SR/blob/main/%5BPRE%5D%20Preprocessing%20Datasets%20-%20post%20to%20github%20version.ipynb) to regenerate the LRs using a python bicubic downsampler.   
Otherwise, if we try to use any of the available bicubic interpolators in Python, there will be inconsitency issues because Matlab has a slightly different bicubic interpolation implementation. 

#### Figure 3 in the paper, Entropy of Gradients vs. Bicubic PSNR
See this [notebook](https://github.com/sabdelmagid/CVPR22-TextureBasedError-SR/blob/main/____Figure3-Entropy%20vs%20PSNR%20-%20post%20to%20github%20version.ipynb)

#### TODO 
add citation for GradientNet code

### Citation
If you find the code helpful in your resarch or work, please cite the following papers:

Our paper:
```

@inproceedings{magid2022texture,
  title={Texture-based Error Analysis for Image Super-Resolution},
  author={Abdel Magid, Salma and Lin, Zudi and Wei, Donglai and Zhang, Yulun and Gu, Jinjin and Pfister, Hanspeter},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
  pages={2118--2127},
  year={2022}
}
```


### Acknowledgements
This code is built on [EDSR (PyTorch)](https://github.com/thstkdgus35/EDSR-PyTorch). 
We thank the authors for sharing their codes of EDSR [Torch version](https://github.com/LimBee/NTIRE2017) and [PyTorch version](https://github.com/thstkdgus35/EDSR-PyTorch).


