# Nike vs Adidas Shoe Image Classifier 👟

A deep learning-based image classification project that uses a Convolutional Neural Network (CNN) to classify basketball shoe images into two categories: Nike and Adidas.

## 📌 Project Overview

The Nike vs Adidas Shoe Image Classifier is a computer vision project developed using Python and deep learning techniques.

The main objective of this project is to train a CNN model that can recognize basketball shoe images and classify them as either Nike or Adidas.

The project includes image preprocessing, grayscale conversion, image resizing, dataset preparation, CNN model development, model training, and image classification.

## 🎯 Objectives

- Classify basketball shoe images into Nike and Adidas categories.
- Apply deep learning techniques to image classification.
- Preprocess images using the PIL library.
- Build and train a Convolutional Neural Network.
- Evaluate the model using a validation dataset.
- Predict the brand of unseen shoe images.

## ✨ Features

- Nike and Adidas shoe image classification.
- Image preprocessing using PIL.
- Grayscale image conversion.
- Image resizing to 120 × 120 pixels.
- Dataset labeling using one-hot encoding.
- CNN-based feature extraction.
- Model training using the Adam optimizer.
- Image prediction using the trained model.

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Programming language |
| TensorFlow | Deep learning framework |
| TFLearn | Neural network modeling |
| NumPy | Numerical operations and data processing |
| PIL | Image loading and preprocessing |
| Matplotlib | Image visualization |
| tqdm | Progress tracking |
| CNN | Image classification |

## 📂 Project Structure

```text
nike-vs-adidas-shoe-image-classifier/
│
├── NIKE_ADIDAS_Classifier.ipynb
│
├── NIKEADIDAS/
│   ├── TRAIN/
│   │   ├── NIKE_1.png
│   │   ├── ADIDAS_1.png
│   │   └── ...
│   │
│   └── TEST/
│       ├── NIKE_1.png
│       ├── ADIDAS_1.png
│       └── ...
│
├── train_data.npy
├── test_data.npy
├── README.md
└── requirements.txt
```

> **Note:** The dataset folders and generated `.npy` files are optional and should be included only if they are available in the project repository.

## ⚙️ How the Project Works

### 1. Dataset Preparation

The dataset contains basketball shoe images from two brands:

- Nike
- Adidas

The images are organized into separate training and testing directories.

### 2. Image Preprocessing

The images are processed using the PIL library.

The preprocessing steps include:

- Loading images from the dataset.
- Converting images to grayscale.
- Resizing images to 120 × 120 pixels.
- Converting images into NumPy arrays.
- Assigning labels to the images.

The labels are represented using one-hot encoding:

```text
Nike   → [1, 0]
Adidas → [0, 1]
```

### 3. CNN Model Development

A Convolutional Neural Network is developed using TFLearn and TensorFlow.

The model consists of:

- Convolutional layers
- Max-pooling layers
- Fully connected layers
- Dropout regularization
- Softmax output layer

The final output layer contains two classes:

- Nike
- Adidas

### 4. Model Training

The model is trained using:

- Adam optimizer
- Categorical cross-entropy loss
- Learning rate of 0.001
- 100 training epochs

A validation dataset is used during training to monitor model performance.

### 5. Prediction

After training, the model generates predictions for shoe images.

The predicted output represents the probability of each image belonging to the Nike or Adidas class.

## 📊 Model Information

| Parameter | Value |
|-----------|-------|
| Problem Type | Binary Image Classification |
| Model | Convolutional Neural Network |
| Classes | Nike and Adidas |
| Image Size | 120 × 120 pixels |
| Image Format | Grayscale |
| Optimizer | Adam |
| Learning Rate | 0.001 |
| Loss Function | Categorical Cross-Entropy |
| Training Epochs | 100 |
| Output Layer | Softmax |
| Framework | TensorFlow and TFLearn |

## 📈 Training Results

The notebook contains a training output showing the following values:

| Metric | Value |
|--------|-------|
| Training Accuracy | Approximately 92.75% |
| Validation Accuracy | 100% |
| Training Loss | Approximately 0.30079 |
| Validation Loss | Approximately 0.09011 |

> **Note:** These values are from the training output recorded in the notebook. They should not be considered a reliable measure of real-world performance without further testing on an independent dataset.

## 🚀 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Sananadaf03/nike-vs-adidas-shoe-image-classifier.git
```

### 2. Navigate to the Project Directory

```bash
cd nike-vs-adidas-shoe-image-classifier
```

### 3. Install the Required Libraries

```bash
pip install numpy pillow matplotlib tqdm tensorflow tflearn
```

### 4. Open the Jupyter Notebook

```bash
jupyter notebook NIKE_ADIDAS_Classifier.ipynb
```

### 5. Run the Notebook

Execute the notebook cells in sequence to:

1. Load the dataset.
2. Preprocess the images.
3. Create the training data.
4. Build the CNN model.
5. Train the model.
6. Evaluate the validation results.
7. Generate predictions.

## 🔍 Sample Prediction

The model produces prediction values for the two shoe categories.

Example:

```text
Input Image: Basketball Shoe

Predicted Brand: Nike
```

The prediction depends on the image provided to the model.

## 💡 Applications

- Sports shoe image classification.
- Fashion brand recognition.
- Product image categorization.
- Computer vision learning.
- Deep learning experimentation.
- Image-based product identification.

## 🔮 Future Improvements

- Increase the size and diversity of the dataset.
- Use color images instead of grayscale images.
- Add more footwear brands.
- Improve the model using data augmentation.
- Use modern CNN architectures such as ResNet or MobileNet.
- Add confusion matrix and classification reports.
- Develop a web application for image prediction.
- Deploy the model using Flask or Streamlit.

## 👩‍💻 Author

**Sana L. Nadaf**

Computer Science and Engineering Graduate

GitHub: [Sananadaf03](https://github.com/Sananadaf03)

LinkedIn: [Sana Nadaf](https://www.linkedin.com/in/sana-nadaf-073950268/)

## 📄 License

This project is intended for educational and portfolio purposes.
