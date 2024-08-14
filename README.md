# Horse Action Recognition Dataset

This repository contains the link to the **Horse Action Recognition Dataset**, which is a dataset focused on horse movements. The dataset is labeled with three categories: `walk`, `trot`, and `canter`. It is designed for use in machine learning models for action recognition.

## Dataset Overview

The dataset includes video sequences of horses performing three different actions:

- **Walk**: A four-beat gait where the horse moves forward one leg at a time.
- **Trot**: A two-beat gait where diagonal pairs of legs move simultaneously.
- **Canter**: A three-beat gait where the horse moves in a specific sequence of legs.

Each folder within the dataset is named according to the action label and contains the corresponding image sequences.

## Download the Dataset

The dataset can be downloaded from the following link:

[Download Horse Action Recognition Dataset](https://keio.box.com/s/dbxcdlhe4a6ugibur7hse12anyslcr65)

## File Structure

The dataset is organized as follows:
### 〇〇pic_mosaic (where 〇〇 can be walk, trot, or canter)

This directory contains a sequence of images extracted from videos at 24fps. The subfolders within are separated by video, for example, the `walk0001` folder contains a sequence of images derived from the same video, meaning the images within have a temporal relationship. However, there is no temporal relationship between images in different folders.


