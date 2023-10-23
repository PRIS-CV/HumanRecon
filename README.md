# HumanRecon
Official PyTorch implementation of the paper HumanRecon: Neural Reconstruction of Dynamic Human Using Geometric Cues and Physical Priors. 

# Datasets
Download the Human3.6M datase from [here](https://github.com/zju3dv/animatable_nerf/blob/master/INSTALL.md#human36m-dataset) and ZJU-Mocap dataset from [here](https://github.com/zju3dv/animatable_nerf/blob/master/INSTALL.md#zju-mocap-dataset).

# Environment
```python
python==3.7
torch==1.4.0+cu100
```

# Traning
Take the training on S9 as an example.
```python
python train_net.py --cfg_file configs/aninerf_s1p.yaml exp_name aninerf_s1p resume False
```

# Testing
Take the testing on S9 as an example.
```python
python run.py --type evaluate --cfg_file configs/aninerf_s9p.yaml exp_name aninerf_s9p resume True
```

# Acknowledgments
Some components of this code implementation are referenced from [NeuralBody](https://github.com/zju3dv/neuralbody) and [Animatable-NeRF](https://github.com/zju3dv/animatable_nerf). We sincerely appreciate their valuable contributions.
