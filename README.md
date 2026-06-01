# Lung Cancer Detection from Chest X-Rays

A deep learning project that uses DenseNet121 to classify chest X-ray images for potential lung cancer indicators.

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/lung-cancer-detection.git
cd lung-cancer-detection
```

Install dependencies:

```bash
pip install tensorflow pandas numpy scikit-learn matplotlib kaggle
```

## Dataset Setup

1. Download the NIH Chest X-Ray dataset:
   https://www.kaggle.com/datasets/nih-chest-xrays/sample

2. Extract the dataset.

3. Update the dataset paths inside the notebook if necessary.

## Running the Project

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```bash
CNNCancer.ipynb
```

Run all cells from top to bottom.

The notebook will:

* Load the dataset
* Generate cancer labels
* Preprocess images
* Train DenseNet121
* Evaluate performance
* Save the trained model

## Using the Trained Model

After training, a model file will be created:

```bash
lung_cancer_densenet_model.h5
```

Load it using:

```python
from tensorflow.keras.models import load_model

model = load_model("lung_cancer_densenet_model.h5")
```

Predict on a new image:

```python
prediction = model.predict(image)
print(prediction)
```

## Example Output

```text
Prediction: 0.87
Result: High probability of cancer-related findings
```

## Demo

YouTube Demonstration:

https://www.youtube.com/watch?v=m2duKg8ghXc

Google Colab Notebook:

https://colab.research.google.com/drive/1uztKCFPJkKrWcEkmuPXnn_sIa1SLSQAu

## Author

Aayush Katoch

## Disclaimer

This project is for educational and research purposes only and should not be used for clinical diagnosis.
