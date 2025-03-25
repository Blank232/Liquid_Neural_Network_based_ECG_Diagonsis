# Liquid Neural Network Based ECG Diagnosis

## Project Overview

This project implements an ECG (Electrocardiogram) classification model using a Liquid Neural Network (LNN) to diagnose various heartbeats. The model is trained on ECG signal data and aims to classify heartbeats into five categories:

- **Class 0**: Normal
- **Class 1**: Supraventricular
- **Class 2**: Ventricular
- **Class 3**: Fusion
- **Class 4**: Unknown

The project involves data preprocessing, training a deep learning model, and evaluating its performance using various metrics such as accuracy, precision, recall, and F1-score.

## Dataset

The dataset consists of ECG signal time-series data collected from multiple patients. Each sample corresponds to a time-sequenced ECG signal labelled into one of the five heartbeat categories.

## Model Training

The model is trained using a deep learning approach with the following key characteristics:

- **Architecture**: Liquid Neural Network (LNN)
- **Loss Function**: Cross-entropy loss
- **Optimizer**: Adam optimizer
- **Epochs**: 10
- **Training Loss Reduction**: The loss gradually decreases over epochs, indicating effective learning.

### Training Loss Curve

The training loss curve shows a steady decline over epochs, confirming that the model is learning effectively and not overfitting.

## Model Evaluation

The model is evaluated using a confusion matrix and classification report.

### Confusion Matrix

The confusion matrix demonstrates the model's classification performance across different heartbeat types. It provides insights into misclassifications and overall accuracy.

### Classification Report

The evaluation metrics include:

- **Accuracy**: 97.54%
- **Precision, Recall, F1-score** for each class
- **Macro and Weighted Averages**

The high accuracy and F1-scores suggest that the model is performing well in identifying ECG patterns.

## Installation & Usage

To run the model and reproduce the results, follow these steps:

### Prerequisites

Ensure you have the following dependencies installed:

```
numpy
pandas
tensorflow
matplotlib
seaborn
sklearn
```

### Running the Model

1. Clone the repository:
   ```
   git clone https://github.com/Blank232/Liquid_Neural_Network_based_ECG_Diagonsis.git
   cd Liquid_Neural_Network_based_ECG_Diagonsis
   ```
2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook:
   ```
   jupyter notebook LNN_based_ECG_Diagnosis.ipynb
   ```

## Results & Visualizations

The project includes several visualizations:

- **Sample ECG signals from the training set**
- **Training loss curve**
- **Confusion matrix and classification metrics**

These visualizations help in understanding the dataset distribution and model performance.

## Future Improvements

- Fine-tuning the model with more advanced architectures
- Increasing the dataset size for better generalization
- Exploring different preprocessing techniques to enhance model accuracy

## Contributing

Contributions are welcome! Feel free to fork this repository, submit issues, and open pull requests.

## License

This project is licensed under the MIT License.


