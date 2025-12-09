# Horse Action Recognition Dataset

This repository provides an overview and documentation for the **Horse Action Recognition Dataset**, a collection of horse locomotion image sequences categorized into three actions: `walk`, `trot`, and `canter`.  
This dataset is intended for machine learning research in action recognition and related fields.

## Dataset Access

The dataset is **not publicly downloadable** in this repository.  
If you wish to use the dataset for academic or research purposes, please contact the dataset authors.

📩 **Request access:** kotoka@keio.jp

Access will be granted to researchers or institutions upon request.

## Dataset Overview

The dataset includes image sequences of horses performing three different actions:

- **Walk**: A four-beat gait where the horse moves forward one leg at a time.  
- **Trot**: A two-beat gait where diagonal pairs of legs move simultaneously.  
- **Canter**: A three-beat gait with a characteristic three-beat sequence.

Each top-level folder corresponds to an action label and contains multiple subfolders, each representing a temporally coherent image sequence extracted from a single video.

## File Structure

### `〇〇pic_mosaic` (〇〇 = `walk`, `trot`, `canter`)
Contains image sequences extracted at 24 fps.  
Each subfolder (e.g., `walk0001`) contains temporally continuous frames.  
There is **no temporal relationship across different folders**.

### `crop_〇〇pic`
Images from `〇〇pic_mosaic` cropped to 640×640 using YOLOv8 horse bounding boxes.

### `crop_〇〇pic_noback`
Derived from `crop_〇〇pic` with sequences removed where the horse faces forward or backward.  
Remaining images preserve intra-folder temporal continuity.

### `crop_〇〇pic_noobst`
Derived from `crop_〇〇pic` with sequences removed where obstacles appear in front of the horse.

### `crop_〇〇pic_nobacklastobst`
Derived from `crop_〇〇pic` with both backward-facing and obstacle-containing sequences removed.

### `〇〇_front_rgb`
Derived from `crop_〇〇pic`, retaining only sequences where the horse is not facing forward or backward.

**Note:** Starting indices within folders are not guaranteed to begin at `0000001`.

## Citation

If you use this dataset in your research, please cite:

```bibtex
@inproceedings{10.1145/3689061.3689065,
author = {Matsunaga, Kotoka and Saito, Hideo},
title = {Comparison and Evaluation of Action Recognition Methods in Equestrian Videos},
year = {2024},
isbn = {9798400711985},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3689061.3689065},
doi = {10.1145/3689061.3689065},
booktitle = {Proceedings of the 7th ACM International Workshop on Multimedia Content Analysis in Sports},
pages = {35–39},
numpages = {5},
location = {Melbourne VIC, Australia},
series = {MMSports '24}
}
