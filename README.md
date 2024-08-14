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
<blockquote>
/horseactionrecognition<br>
    /walkpic_mosaic<br>
        /walk0001<br>
            0000001.jpg<br>
            0000002.jpg<br>
            ...<br>
        /walk0002<br>
            0000001.jpg<br>
            0000002.jpg<br>
            ...<br>
        ...<br>
    /trotpic_mosaic<br>
    /canter_mosaic<br>
    /crop_walkpic<br>
    /crop_trotpic<br>
    /crop_canterpic<br>
    /crop_walkpic_noback<br>
    /crop_trotpic_noback<br>
    /crop_canterpic_noback<br>
    /crop_walkpic_noobst<br>
    /crop_trotpic_noobst<br>
    /crop_canterpic_noobst<br>
    /crop_walkpic_nobacklastobst<br>
    /crop_trotpic_nobacklastobst<br>
    /crop_canterpic_nobacklastobst<br>
    /walk_front_rgb<br>
    /trot_front_rgb<br>
    /canter_front_rgb<br>
    /DLCcsv<br>
        /DLCforwalk<br>
            /walk0001<br>
                0000001.csv<br>
                0000002.csv<br>
                ...<br>
        /DLCfortrot<br>
        /DLCforcanter<br>
    /DLCcropcsv<br>
    /DLCcropcsv_noback<br>
    /DLCcropcsv_nobackobst<br>
</blockquote>

