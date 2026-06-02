
# Bangladeshi License Plate Detection Dataset

This repository contains the datasets used in our research on Bangladeshi vehicle license plate detection and recognition.

## Original Dataset Sources

The final dataset was constructed by merging and refining the following publicly available Roboflow datasets:

1. [Dataset Format Conversion](https://universe.roboflow.com/my-dataset-lb91e/dataset-format-conversion-9mgzb)
2. [NumberPlate-LS32N](https://universe.roboflow.com/numberplatedetection-4ihhs/numberplate-ls32n)
3. [Bangla License Plate Dataset](https://universe.roboflow.com/nameplate/bangla)
4. [LPD4K](https://universe.roboflow.com/license-plate-recognition-ud5va/lpd4k)

After merging, duplicate inspection, annotation verification, and correction of missing or broken annotations were performed to create a unified dataset.

## Dataset Downloads

### Clean Dataset

Merged and manually refined dataset after annotation correction.

🔗 https://drive.google.com/file/d/1gSsMpfNEqHwJRd_wk_3y2WezsjQTqgDJ/view?usp=sharing

### Proposed Augmentation Dataset

Training set augmented using the proposed adverse-condition augmentation framework.

🔗 https://drive.google.com/file/d/1G2pMB-_pxQOcp5mxns8mtyRD4jt5l5oM/view?usp=sharing

### Traditional Augmentation Dataset

Training set augmented using conventional augmentation techniques.

🔗 https://drive.google.com/file/d/1iLM5hgouDyzYAUUb2FeBaSfE973JrV4b/view?usp=sharing

### Adverse-Condition Test Dataset

Independent test set containing fog, rain, shadow, glare, night, and motion-blur conditions used for augmentation benchmarking.

🔗 https://drive.google.com/file/d/1OdvWovMzVzTpeBgSWtaMSpRjK3V5x_W6/view?usp=sharing

## Experimental Usage

### Augmentation Benchmark

Baseline YOLOv11s models were trained separately using:

* Clean Dataset ([Click](https://drive.google.com/file/d/1gSsMpfNEqHwJRd_wk_3y2WezsjQTqgDJ/view?usp=sharing))
* Traditional Augmentation Dataset ([Click](https://drive.google.com/file/d/1iLM5hgouDyzYAUUb2FeBaSfE973JrV4b/view?usp=sharing))
* Proposed Augmentation Dataset ([Click](https://drive.google.com/file/d/1G2pMB-_pxQOcp5mxns8mtyRD4jt5l5oM/view?usp=sharing))

All models were evaluated on the same Adverse-Condition Test Dataset ([Click](https://drive.google.com/file/d/1OdvWovMzVzTpeBgSWtaMSpRjK3V5x_W6/view?usp=sharing)).

### Detection Benchmark

All detection architectures were trained and evaluated using the Proposed Augmentation Dataset ([Click](https://drive.google.com/file/d/1G2pMB-_pxQOcp5mxns8mtyRD4jt5l5oM/view?usp=sharing)). 

