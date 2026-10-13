# Surface EMG-Based Hand Gesture Recognition

**Farzan Aghaei · Sanaz Mazrae**  
Sharif University of Technology · Sensing and Measurements

Classification of 17 hand and wrist gestures using 12-channel surface EMG from NinaPro DB2 (Subject 14, Exercise 1). Signal preprocessing, feature extraction, classification, plots, and evaluation are implemented in one executable Jupyter notebook.

## Results

| Model         |  Accuracy  | Balanced accuracy |  Macro-F1  |
| :------------ | :--------: | :---------------: | :--------: |
| Random Forest | **74.26%** |    **75.09%**     | **75.17%** |
| SVM (RBF)     |   67.72%   |      70.31%       |   70.29%   |
| LDA           |   62.77%   |      65.69%       |   66.04%   |
| KNN (k=5)     |   61.45%   |      64.65%       |   65.49%   |

Results are from within-subject evaluation, with gesture repetitions 2 and 5 held out for testing. Details are provided in the [project report](EMG_Hand_Gesture_Recognition_Report.pdf).

## Run

1. Install dependencies: `pip install -r requirements.txt`.
2. Obtain `S14_E1_A1.mat` from the [NinaPro DB2 dataset](https://ninapro.hevs.ch/instructions/DB2.html) and place it in a `data/` folder.
3. Open `EMG_Hand_Gesture_Recognition.ipynb` and select **Run All**.

The notebook contains the complete pipeline and its output visualizations. The dataset is not redistributed in this repository.
