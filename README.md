# Oil Spill Detection Using U-Net

## Overview
This project uses deep learning and satellite imagery to detect and segment oil spills. A U-Net architecture built using PyTorch is trained to identify oil spill regions at the pixel level.

## Objectives
- Detect oil spill regions in satellite images.
- Perform image preprocessing and segmentation using U-Net.
- Evaluate model performance using Dice Score, IoU, Precision, and Recall.

## Technologies Used
- Python
- PyTorch
- Google Colab
- NumPy
- Matplotlib

## Dataset
The project uses the **Refined Deep-SAR Oil Spill Dataset**.

Dataset source: https://zenodo.org/records/15298010

The dataset is not included in this repository. Download it separately before running the notebook.

## Model
A U-Net architecture is used for semantic segmentation of satellite images. The model predicts a segmentation mask identifying the regions containing oil spills.

## Results
The model achieved the following validation metrics at a threshold of 0.55:

| Metric | Score |
|---|---:|
| Dice Score | 0.8563 |
| IoU | 0.7487 |
| Precision | 0.8284 |
| Recall | 0.8861 |
| Pixel Accuracy | 0.9196 |

*These are global pixel-level evaluation results.*

## Project Structure
```text
oil-spill-detection-using-unet/
├── notebooks/
│   ├── oil_spill_detection_using_unet.ipynb
│   └── README.md
├── results/
│   └── sample_predictions.png
├── README.md
└── .gitignore
```

## How to Run
1. Clone this repository.
2. Open the notebook in Google Colab.
3. Download the dataset from the source provided above.
4. Update the dataset path in the notebook if required.
5. Run the notebook cells to train and evaluate the model.

## Future Scope
- Improve segmentation performance and reduce false positives.
- Integrate AIS vessel data for vessel correlation.
- Explore oil spill drift prediction.

## Author
Om Suryavanshi
