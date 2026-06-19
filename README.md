# Multimodal_Deepfake_Detection
Yuan Ze University AI Applications course project

## How to Run on Kaggle

1. In [Kaggle](https://kaggle.com) and create a new notebook
2. Click **+ Add Data** and add the FakeAVCeleb dataset from `shreyaty08/fakeavceleb`
3. Upload `deepfake detection kaggle.ipynb`
4. Set accelerator to **GPU T4 x2** under Settings
5. Click **Run All**

## How to Run on Colab
1. Go to https://colab.research.google.com
2. Click File, then Open notebook.
3. Select the GitHub tab.
4. Paste your GitHub repository URL and press Enter.
5. Click on `deepfake detection colab.ipynb` to open it.
6. Click Runtime, then Change runtime type, and select GPU as the hardware accelerator.
7. Add this code as a new cell at the top of the notebook and run it.


## Dataset

FakeAVCeleb is a multimodal deepfake detection dataset containing real and fake videos of celebrities with synchronized audio.

The dataset contains 4 categories based on which modality was manipulated.

1. RealVideo-RealAudio — original unmodified videos, label 0 (REAL)
2. FakeVideo-RealAudio — face-swapped video with original audio, label 1 (FAKE)
3. FakeVideo-FakeAudio — face-swapped video with synthesized audio, label 1 (FAKE)
4. RealVideo-FakeAudio — original video with synthesized audio, label 1 (FAKE)

The videos were collected from YouTube and feature 500 subjects. Fake videos were generated using state-of-the-art deepfake generation methods including FaceSwap, FSGAN, and SimSwap for video, and SV2TTS for audio synthesis.

In this project we use a synthetic subset of the dataset for training. The data is split as follows.

1. Training set — 80% of the data
2. Validation set — 10% of the data
3. Test set — 10% of the data

For more information about the original dataset visit https://github.com/DASH-Lab/FakeAVCeleb
