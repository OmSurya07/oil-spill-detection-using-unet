## How to Run the Project (Google Colab)

1. Download the Refined Deep-SAR Oil Spill Dataset from [Zenodo](https://zenodo.org/records/15298010).
2. Upload the downloaded ZIP file to your Google Drive.
3. Open the notebook from the `notebooks` folder using Google Colab.
4. Mount your Google Drive when prompted.
5. Update the dataset ZIP path in the notebook to match its location in your Drive, if required.
6. Run the notebook cells sequentially.

The notebook handles dataset extraction, preprocessing, U-Net model training, and evaluation.

**Note:** Google Colab is the recommended environment. GPU acceleration can be enabled through Runtime → Change runtime type → T4 GPU (when available).
