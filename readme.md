#  Texture-based Error Analysis for Image Super-Resolution (CVPR 22).


#### First DIV2K LR_bicubic using https://github.com/sanghyun-son/bicubic_pytorch
Since we are using python and need to use bicubic upsampling for some of our experiments, we regenerate the low resolution DIV2K images. When you download the original DIV2K images, you will find the matlab corrupted LRs. Ignore those. Instead use the [preprocessing notebook]() to regenerate the LRs using a python bicubic downsampler.   
Otherwise, if we try to use any of the available bicubic interpolators in Python, there will be inconsitency issues because Matlab has different interpolation implmenation. 




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


