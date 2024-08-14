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

/horseactionrecognition  
  /walkpic_mosaic  
    /walk0001  
      0000001.jpg  
      0000002.jpg  
      ...  
    /walk0002  
      0000001.jpg  
      0000002.jpg  
      ...  
    ...  
  /trotpic_mosaic  
  /canter_mosaic  
  /crop_walkpic  
  /crop_trotpic  
  /crop_canterpic  
  /crop_walkpic_noback  
  /crop_trotpic_noback  
  /crop_canterpic_noback  
  /crop_walkpic_noobst  
  /crop_trotpic_noobst  
  /crop_canterpic_noobst  
  /crop_walkpic_nobacklastobst  
  /crop_trotpic_nobacklastobst  
  /crop_canterpic_nobacklastobst  
  /walk_front_rgb  
  /trot_front_rgb  
  /canter_front_rgb  
  /DLCcsv  
    /DLCforwalk  
      /walk0001  
        0000001.csv  
        0000002.csv  
        ...  
    /DLCfortrot  
    /DLCforcanter  
  /DLCcropcsv  
  /DLCcropcsv_noback  
  /DLCcropcsv_nobackobst

