
# Xception Image Classifier (Fine-Tuned)

This repository contains a fine-tuned image classification model built using the **Xception architecture** from TensorFlow/Keras. The model is trained on a custom dataset of images organized into training, validation, and testing directories.

## 📁 Project Structure

```
Xception Classifier-fine tuned.ipynb
├── train/          # Training images (organized by class)
├── validate/       # Validation images (organized by class)
├── test/           # Test images (organized by class)
```

## 🧠 Model Architecture

- Base model: `Xception` pretrained on ImageNet
- Input shape: 299x299 RGB images
- Classification head:
  - `GlobalAveragePooling2D`
  - `Dropout`
  - `Dense` layer with softmax activation (for 5 classes)

## 🚀 Features

- ✅ Transfer learning with `Xception`
- ✅ Image resizing and augmentation
- ✅ Fine-tuned classification layers
- ✅ Model evaluation on test data
- ✅ Accuracy and loss visualization

## 📦 Dependencies

Install required Python libraries:

```bash
pip install tensorflow pillow matplotlib
```

## 📊 Training Parameters

- Input Size: `(299, 299)`
- Batch Size: `32`
- Learning Rate: `0.001`
- Epochs: `10`
- Optimizer: `Adam`

## 🖼️ Dataset Format

Each dataset directory (`train`, `validate`, `test`) must be structured like this:

```
dataset/
├── class_1/
│   ├── image1.jpg
│   ├── image2.jpg
├── class_2/
│   ├── image3.jpg
...
```

## 📈 Results

The notebook includes visualization for:

- Training and validation accuracy/loss over epochs
- Sample predictions

## 🧪 Usage

1. Place your dataset in the appropriate directories (`train`, `validate`, `test`).
2. Run the notebook: `Xception Classifier-fine tuned.ipynb`
3. Monitor outputs and tweak parameters as needed.

## ✍️ Author

Developed by [Your Name] using TensorFlow and Keras.
