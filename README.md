# SepNet
For original repo, see [SepNet](https://github.com/HiLab-git/SepNet/tree/master)

# Requirements
Pytorch >= 1.4, SimpleITK >= 1.2, scipy >= 1.3.1, nibabel >= 2.5.0 and some common packages.

# Docker

```
docker pull qiyi007/sepnet
```

# File Directory
```
.
|-- DATASET
|-- train
|   |-- case_01
        |--
|   |-- case_02
        |-- 
|   |-- ...
|   
|-- valid
|   |-- case_xx
|   |-- ...


```


# Code
For Preprocessing

```
cd data_process
python Preprocess.py
```

For training

Change the `data_root` in `config/train.txt` to your data root;
```
python train.py
```

For inference

```
python Segmentation.py
```
Notise the you may need to padding Seg.nii.gz to keep consistent with the shape of your test data. See `padded.py` as an example.

