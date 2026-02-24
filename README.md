# ml-deeplearning-notebooks

This is a series of Jupyter notebooks introducing machine learning and deep learning concepts, developed for the workshop [Introduction to Machine Learning in Python](https://carpentry.library.ucsb.edu/workshop/2026/02/02/ucsb-ml.html), offered by the [Carpentry @ UCSB Library](https://carpentry.library.ucsb.edu/) in Winter 2026. 

These notebooks take you from ML fundamentals through convolutional neural networks.

Authors: Tian Qiu, Jose Nino Muriel

## Notebooks

### [1. Introduction to Machine Learning](1_intro.ipynb)
Covers the foundations of machine learning, including:
- ML vs rule-based programming; classification, regression, and clustering
- 10-step ML workflow and problem formulation
- **Project:** Penguin species classification (Seaborn penguins dataset)
  - Logistic regression and hyperplane-based decision boundaries
  - Confusion matrices and accuracy evaluation
- Introduction to neural networks: single neurons, ReLU/GELU activation functions, one-hot encoding

### [2. Neural Network Classification](2_classification.ipynb)
Builds a full neural network classifier using Keras/TensorFlow:
- **Project:** Penguin species classification (continued)
- Keras Sequential API: `Input`, `Dense`, `softmax` output layer
- Categorical crossentropy loss, Adam optimizer
- Training for 100 epochs, loss curve visualization
- Predictions, confusion matrix heatmap

### [3. Monitoring Training & Regression](3_monitor_training.ipynb)
Extends to regression tasks and introduces training best practices:
- **Project:** Predicting Basel sunshine hours from European weather data ([Zenodo dataset](https://zenodo.org/record/5071376), 11 cities, 3654 days)
- 70/15/15 train/validation/test split strategy
- Gradient descent, batch training, and epoch concepts
- RMSE metric, baseline model comparison
- Overfitting detection using validation loss
- `EarlyStopping` callback

### [4. Image Classification with CNNs](4_image_classification.ipynb)
Introduces convolutional neural networks for image data:
- **Project:** MNIST handwritten digit classification (60,000 training images, 28×28 grayscale)
- Image normalization and channel dimensions
- `Conv2D` filters, kernel size, stride, padding
- `MaxPooling2D` for dimensionality reduction
- Full CNN architecture: Conv → Pool → Conv → Pool → Flatten → Dense → Softmax
- Visualizing learned filters and intermediate layer outputs

## Key Learning Objectives

| Notebook | Task | Key Concepts |
|----------|------|--------------|
| 1 | Classification | ML fundamentals, neurons, activations |
| 2 | Classification | Keras model building, training loop |
| 3 | Regression | Train/val/test split, overfitting, early stopping |
| 4 | Classification | CNNs, filters, pooling |

## Technologies

- **TensorFlow / Keras** — model building and training
- **scikit-learn** — classical ML, metrics, train/test split
- **pandas / NumPy** — data manipulation
- **Matplotlib / Seaborn** — visualization
