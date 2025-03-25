# LNN-based ECG Diagnosis

## Overview
This project implements a **Liquid Neural Network (LNN)** for **Electrocardiogram (ECG) signal classification**. The model classifies ECG signals into five categories:
- **Normal**
- **Supraventricular**
- **Ventricular**
- **Fusion**
- **Unknown**

The project includes preprocessing, training, and evaluation of the model using a dataset of ECG signals.

## Dataset
The dataset consists of ECG signals labelled into five different classes. The signals are preprocessed and fed into a neural network for classification.

## Model Architecture
The model is a **Liquid Neural Network (LNN)** designed for efficient ECG classification. It is trained using a supervised learning approach and optimized to minimize loss while maintaining high classification accuracy.

## Training Results
### Loss Progression
The model was trained for **10 epochs**, and the loss steadily decreased:
```
Epoch 1/10, Loss: 0.0925
Epoch 2/10, Loss: 0.0893
Epoch 3/10, Loss: 0.0862
Epoch 4/10, Loss: 0.0835
Epoch 5/10, Loss: 0.0808
Epoch 6/10, Loss: 0.0776
Epoch 7/10, Loss: 0.0753
Epoch 8/10, Loss: 0.0738
Epoch 9/10, Loss: 0.0714
Epoch 10/10, Loss: 0.0698
```
A plot of training loss over epochs shows a clear downward trend.

### Classification Performance
The model achieved **97.54% accuracy** on the test dataset.

#### Confusion Matrix
A confusion matrix illustrates the classification performance, showing high accuracy in predicting normal and other categories.

#### Classification Report
```
Precision  Recall  F1-score  Support
----------------------------------
0   0.98     1.00    0.99     18118
1   0.90     0.63    0.74      556
2   0.94     0.92    0.93     1448
3   0.80     0.62    0.70      162
4   0.99     0.96    0.97     1608
----------------------------------
Accuracy: 97.04%
```

## Installation & Usage
1. Clone this repository:
   ```bash
   git clone https://github.com/Blank232/Liquid_Neural_Network_based_ECG_Diagonsis.git
   cd Liquid_Neural_Network_based_ECG_Diagonsis
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook:
   ```bash
   jupyter notebook LNN_based_ECG_Diagnosis.ipynb
   ```

## Visualizations
- **ECG signal samples** from the training set
- **Loss curve over epochs**
- **Confusion matrix**

## Future Improvements
- Implement **data augmentation** for better generalization.
- Optimize model architecture for **real-time applications**.
- Deploy the model as a **web or mobile application**.

## License
This project is licensed under the MIT License.

