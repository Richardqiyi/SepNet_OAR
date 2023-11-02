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
|-- Task01_BrainTumour
|   |-- imagesTr
|   |-- imagesTs
|   `-- labelsTr
|-- nnformer
|   |-- __pycache__
|   |-- dataset_conversion
|   |-- dataset_json
|   |-- evaluation
|   |   |-- __pycache__
|   |   `-- model_selection
|   |-- experiment_planning
|   |   |-- __pycache__
|   |   |-- alternative_experiment_planning
|   |   |   |-- normalization
|   |   |   |-- patch_size
|   |   |   |-- pooling_and_convs
|   |   |   `-- target_spacing
|   |   `-- old

```


# Code

For training
Change the `data_root` in `config/train.txt` to your data root;
```
python train.py
```

For inference

```
inference code here, if there is config, write down how to write config
```




