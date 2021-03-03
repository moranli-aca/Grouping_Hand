# LearnableGroups-Hand

The code for the paper **Exploiting Learnable Joint Groups for Hand Pose Estimation** (Accepted by AAAI2021).

[Paper](https://arxiv.org/abs/2012.09496)


#### Overall network: 

<p align="middle">
    <img src="assets/overall_network.png", width="780">
</p>

#### Qualitative Results 
> some qualitative results on the RHD/STB/FHD dtasets. 
> In each triplet, from left to right:  imgs (input), predictions, GT. 

- RHD:  you can obtain this dataset via [hand3d](https://github.com/lmb-freiburg/hand3d).
<p align="middle">
    <img src="assets/RHD_qualitative_1.png", width="780">
</p>

-  FHD:  you can obtain this dataset following this instruction [FreiHand](https://lmb.informatik.uni-freiburg.de/projects/freihand/) .
<p align="middle">
    <img src="assets/FHD_qualitative_1.png", width="780">
</p>


- STB:  you can obtain this dataset via [STB](https://github.com/zhjwustc/icip17_stereo_hand_pose_dataset) .
<p align="middle">
    <img src="assets/STB_qualitative_1.png", width="780">
</p>

### Citing LearnableGroups-Hand
If this repository is helpful to your research, please cite the [paper](https://arxiv.org/abs/2012.09496):
```
@inproceedings{li2020exploiting,
      title={Exploiting Learnable Joint Groups for Hand Pose Estimation}, 
      author={Moran Li and Yuan Gao and Nong Sang},
      year={2021},
      booktitle={AAAI}
}
```

### Usage 
The code is built on Python3 and Pytorch 1.6.0.

#### Install dependencies 
```bash
pip install -r requirements.txt
```
#### Run the code 
- evaluate on the RHD: 
```bash
python eval_RHD.py --data_dir 'your RHD_published_v2 dataset path'
```
#### Comparison with SOTA methods
- Plot AUC curve on RHD/STB/DO
    - obtain AUC curve for comparison with other SOTA methods (as shown in Fig.3 in main paper). 
    <p align="middle">
        <img src="assets/overall_auc.png", width="780">
    </p>

- Ours User Name on the [FreiHand CodaLab website](https://competitions.codalab.org/competitions/21238#results) is 'anonymous15'


