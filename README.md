# VIDIT: Virtual Image Dataset for Illumination Transfer

### **Mirror repository; maintained up-to-date version at: [https://github.com/majedelhelou/VIDIT](https://github.com/majedelhelou/VIDIT)**

Contact author: [Majed El Helou](https://majedelhelou.github.io/)

## Getting the CVPR 2021 NTIRE data (with depth maps)
Note: *ground-truth test* data will remain private.

Track 1 is one-to-one relighting: transforming an image from its input illumination settings to the target illumination settings.

Track 2 is any-to-any relighting: unlike track 1, the input illumination is variable, and the target illumination is not fixed but is rather given by another guide image.

**Track 1**: [[Train](https://datasets.epfl.ch/vidit/NTIRE2021/track1_train.zip)] - [[Validation_Input](https://datasets.epfl.ch/vidit/NTIRE2021/track1_validation.zip)] - [[Validation_GT](https://datasets.epfl.ch/vidit/NTIRE2021/track1_validation_gt.zip)] - [[Test_Input](https://datasets.epfl.ch/vidit/NTIRE2021/track1_test.zip)]

**Track 2**: [[Train](https://datasets.epfl.ch/vidit/NTIRE2021/track2_train.zip)] - [[Validation_Input](https://datasets.epfl.ch/vidit/NTIRE2021/track2_validation.zip)] - [[Validation_GT](https://datasets.epfl.ch/vidit/NTIRE2021/track2_validation_gt.zip)] - [[Test_Input](https://datasets.epfl.ch/vidit/NTIRE2021/track2_test.zip)]



## Getting the ECCV 2020 AIM data
Note: *ground-truth test* data will remain private.

**Track 1** (1024x1024): [[Train](https://datasets.epfl.ch/vidit/AIM2020/AIM2020_track1_train.zip)] - [[Validation_Input](https://datasets.epfl.ch/vidit/AIM2020/AIM2020_track1_validation.zip)] - [[Validation_GT](https://datasets.epfl.ch/vidit/AIM2020/AIM2020_track1_validation_gt.zip)] - [[Test_Input](https://datasets.epfl.ch/vidit/AIM2020/AIM2020_track1_test.zip)]

**Track 2** (1024x1024): [[Train](https://datasets.epfl.ch/vidit/VIDIT_train.zip)] - [[Validation_Input](https://datasets.epfl.ch/vidit/AIM2020/AIM2020_track2_validation.zip)] - [[Validation_GT](https://datasets.epfl.ch/vidit/AIM2020/AIM2020_track2_validation_gt.zip)] - [[Test_Input](https://datasets.epfl.ch/vidit/AIM2020/AIM2020_track2_test.zip)]

**Track 3** (512x512): [[Train](https://datasets.epfl.ch/vidit/AIM2020/AIM2020_track3_train.zip)] - [[Validation_Input](https://datasets.epfl.ch/vidit/AIM2020/AIM2020_track3_validation.zip)] - [[Validation_GT](https://datasets.epfl.ch/vidit/AIM2020/AIM2020_track3_validation_gt.zip)] - [[Test_Input](https://datasets.epfl.ch/vidit/AIM2020/AIM2020_track3_test.zip)]

The images are downsampled by 2 for the competition track 3 to ease the computations:
`smallsize_img = cv2.resize(origin_img, (512, 512), interpolation=cv2.INTER_CUBIC)`

If you want to use VIDIT for other purposes, the training images are provided in full 1024x1024 resolution in the "Train" link of **Track 2** above. Also available for download from a Google Drive mirror here: [[Download](https://drive.google.com/open?id=1i_2lIXi-gXgIouDCYnfrdtY3wzTiH1E9)]



## Citations
```bibtex
@article{elhelou2020vidit,
    title   = {{VIDIT}: Virtual Image Dataset for Illumination Transfer},
    author  = {El Helou, Majed and Zhou, Ruofan and Barthas, Johan and S{\"u}sstrunk, Sabine},
    journal = {arXiv preprint arXiv:2005.05460},
    year    = {2020}
}

@inproceedings{elhelou2020aim,
    title     = {{AIM} 2020: Scene Relighting and Illumination Estimation Challenge},
    author    = {El Helou, Majed and Zhou, Ruofan and S{\"u}sstrunk, Sabine and Timofte, Radu and others},
    booktitle = {Proceedings of the European Conference on Computer Vision Workshops (ECCVW)},
    year      = {2020}
}

@inproceedings{elhelou2021ntire,
    title     = {{NTIRE} 2021 Depth Guided Image Relighting Challenge},
    author    = {El Helou, Majed and Zhou, Ruofan and S{\"u}sstrunk, Sabine and Timofte, Radu},
    booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition Workshops (CVPRW)},
    pages     = {566--577},
    year      = {2021}
}
```
