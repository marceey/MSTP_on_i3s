# MSTP_on_i3s
## Introduction
This work aims to adapt the MSTP model introduced in this [paper](https://openaccess.thecvf.com/content/CVPR2022/papers/Tan_Multi-Grained_Spatio-Temporal_Features_Perceived_Network_for_Event-Based_Lip-Reading_CVPR_2022_paper.pdf)
by Tan et al. (2022); which was used to tackle an automatic event-based lip-reading
problem. This code builds on the Pytorch implementation of the work of Tan et al. (2022).
![image](https://https://github.com/YaoLu314/event-based-lip-reading/tree/main/misc/framework.jpg)

The goal was to adapt this model to a novel dataset of french speakers called 2022_i3s_EventLipReadingDataset.

## Dependencies
* Python 3.7
* Pytorch 1.6.0

## Prepare
1. Create a new folder and name it `log`;
2. Download [2022_i3s_EventLipReadingDataset](https://drive.google.com/file/d/1dBEgtmctTTWJlWnuWxFtk8gfOdVVpkQ0/view) dataset, and put it in `data` folder;

## Training
You can train your model by running
```python
python main.py --gpus=0 --num_bins=1+4 --test=False --alpha=4 --beta=4 --log_dir=debug
```

## References
Tan, G., Wang, Y., Han, H., Cao, Y., Wu, F., & Zha, Z. (2022). Multi-Grained Spatio-Temporal Features Perceived Network for Event-Based Lip-Reading. In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) (pp. 20094-20103).