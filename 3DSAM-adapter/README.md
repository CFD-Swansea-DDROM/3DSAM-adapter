# Training

Type the command below to train the 3DSAM-adapter:
```sh
python train.py --data kits --snapshot_path "path/to/snapshot/" --data_prefix "path/to/data folder/"  --rand_crop_size 256
```
The pre-trained weight of SAM-B can be downloaded [here](https://dl.fbaipublicfiles.com/segment_anything/sam_vit_b_01ec64.pth) 
and shall be put under the folder ckpt. Users with powerful GPUs can also adapt the model with [SAM-L](https://dl.fbaipublicfiles.com/segment_anything/sam_vit_l_0b3195.pth) or [SAM-H](https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth).

# Evaluation

Type the command below to evaluate the 3DSAM-adapter:
```sh
python test.py --data kits --snapshot_path "path/to/snapshot/" --data_prefix "path/to/data folder/"  --rand_crop_size 256 --num_prompts 1
```

# Pre-trained Checkpoint

Our pretrained checkpoint can be downloaded through [OneDrive](https://mycuhk-my.sharepoint.com/:f:/g/personal/1155187960_link_cuhk_edu_hk/EgSZwTonMG1Cl_PA7wTP5zgBe-DU4K5rb0woDt3i8U22SA?e=0jmfkq).
For KiTS and MSD-Colon, the crop size is 256. For LiTS and MSD-Pancreas, the crop size is 128.