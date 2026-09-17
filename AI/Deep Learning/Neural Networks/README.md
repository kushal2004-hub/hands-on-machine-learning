# MNIST Handwritten Digit Classification with Neural Networks

## 📌 Project Overview
This notebook builds and trains a **neural network classifier** to recognize handwritten digits (0-9) using the MNIST dataset. The model achieves **97% test accuracy** using TensorFlow/Keras.

## 📂 Dataset: MNIST
- **70,000** grayscale images of handwritten digits (28x28 pixels)
- **Training set**: 60,000 images
- **Test set**: 10,000 images
- **Classes**: 10 digits (0-9)

## 🧠 Model Architecture
| Layer | Type | Neurons | Activation | Parameters |
|-------|------|---------|------------|------------|
| 1 | Dense | 128 | ReLU | 100,480 |
| 2 | Dense | 64 | ReLU | 8,256 |
| 3 | Dense | 10 | Softmax | 650 |
| **Total** | | | | **109,386** |

## 🔧 Key Steps
1. **Data Loading**: Load MNIST from Keras datasets
2. **Exploration**: Visualize sample digits
3. **Preprocessing**: Normalize pixels (0-1), reshape (784), one-hot encode labels
4. **Model Building**: Create sequential neural network
5. **Training**: Train for 10 epochs with 20% validation split
6. **Evaluation**: Test accuracy and predictions
7. **Visualization**: Plot training history and results

## 📊 Results
| Metric | Value |
|--------|-------|
| **Test Accuracy** | **97.04%** |
| Training Accuracy | 97.72% |
| Validation Accuracy | 97.04% |
| Training Time | ~2-3 minutes |

### Sample Predictions
First 10 test images:
Predicted: [7 2 1 0 4 1 4 9 5 9]
Actual: [7 2 1 0 4 1 4 9 5 9]

✅ **Perfect accuracy on first 10 samples!**

## 📈 Visualizations
- **Sample digits** from training set
- **Training history** (accuracy & loss curves)
- **Prediction results** with true vs predicted labels

## 🛠️ Technologies Used
| Library | Purpose |
|---------|---------|
| **TensorFlow/Keras** | Deep learning framework |
| **NumPy** | Numerical operations |
| **Matplotlib/Seaborn** | Data visualization |
| **Scikit-learn** | Metrics and utilities |

## 🚀 How to Run
1. Open in Google Colab
2. Run all cells sequentially
3. Training will start automatically (10 epochs)
4. View results at the end

## 🎯 Learning Outcomes
- ✅ Building neural networks with Keras Sequential API
- ✅ Image classification with MNIST dataset
- ✅ Data preprocessing for neural networks
- ✅ Model training with validation split
- ✅ Evaluating model performance
- ✅ Visualizing training history and predictions