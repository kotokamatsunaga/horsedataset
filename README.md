# Horse Action Recognition Dataset

This repository contains the Horse Action Recognition Dataset, which focuses on horse movements. The dataset is labeled with three categories: `walk`, `trot`, and `canter`. It is designed for use in machine learning models for action recognition.

## Dataset Overview

The dataset includes image sequences of horses performing three different actions:

- **Walk**: A four-beat gait where the horse moves forward one leg at a time.
- **Trot**: A two-beat gait where diagonal pairs of legs move simultaneously.
- **Canter**: A three-beat gait where the horse moves in a specific sequence of legs.

Each folder within the dataset is named according to the action label and contains the corresponding image sequences.

## Download the Dataset

The dataset can be downloaded from the following link:

[Download Horse Action Recognition Dataset](https://keio.box.com/s/dbxcdlhe4a6ugibur7hse12anyslcr65)

## File Structure

The dataset is organized as follows:

### 〇〇pic_mosaic (where 〇〇 can be `walk`, `trot`, or `canter`)

This directory contains sequences of images extracted from videos at 24fps. The subfolders are organized by video; for example, the `walk0001` folder contains a sequence of images derived from the same video, meaning the images within the folder have a temporal relationship. However, there is no temporal relationship between images in different folders.

### crop_〇〇pic

These folders contain images from 〇〇pic_mosaic, cropped to 640x640 using YOLOv8 to create bounding boxes around the horse.

### crop_〇〇pic_noback

These folders are derived from crop_〇〇pic, with sequences of images manually removed where the horse is facing forward or backward. The remaining sequences within each folder maintain a temporal relationship, but there is no longer a folder-to-folder correspondence with crop_〇〇pic.

### crop_〇〇pic_noobst

These folders are derived from crop_〇〇pic, with sequences of images manually removed where there are obstacles in front of the horse.

### crop_〇〇pic_nobacklastobst

These folders are derived from crop_〇〇pic, with sequences of images manually removed where the horse is facing forward or backward, as well as sequences with obstacles in front of the horse.

### 〇〇_front_rgb

These folders are derived from crop_〇〇pic, retaining only the sequences where the horse is not facing forward or backward.

**Note:** Not all image sequences within the folders start with 0000001.

## Citation

If you use this dataset in your research, please cite it as follows:

```bibtex
@inproceedings{
matsunaga2024comparison,
title={Comparison and Evaluation of Action Recognition Methods in Equestrian Videos},
author={Kotoka Matsunaga and Hideo Saito},
booktitle={7th Int. Workshop on Multimedia Content Analysis in Sports (MMSports'24) @ ACM Multimedia 2024},
year={2024},
url={https://openreview.net/forum?id=SJPtl9gpkS}
}
```

## Contact

For any questions or inquiries, please contact [kotoka@keio.jp](mailto:kotoka@keio.jp).
