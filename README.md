## Rice Classification
[![](Image.jpg)](https://unsplash.com/photos/aerial-view-photography-of-rice-crops-during-daytime-cusz0Bg-5mQ)

### Overview
This project focuses on classifying rice images into five categories (Arborio, Basmati, Ipsala, Jasmine, Karacadag) using deep learning techniques. It leverages a dataset of 15,000 images to train two models: a custom Convolutional Neural Network (CNN) and a fine-tuned ResNet50 model. Implemented with TensorFlow/Keras, the project includes data augmentation, transfer learning, and comprehensive evaluation metrics. The custom CNN achieves **98% accuracy**, while the ResNet50 model reaches **99% accuracy** on test data.

<br>

### Project Workflow
1. **Data Loading & Preprocessing**: 
   - Load dataset from Kaggle and split into training (70%), validation (15%), and test (15%) sets.
   - Resize images to 224x224 pixels and normalize pixel values.
   - Apply data augmentation (rotation, shifts, flip, zoom) to reduce overfitting.

2. **Model Development**:
   - **Custom CNN Architecture**: Built with `Conv2D`, `MaxPooling2D`, `Dropout`, and `Dense` layers.
   - **ResNet50 Transfer Learning**: Pre-trained on ImageNet, fine-tuned with additional dense layers.
   - Both models use `Adam` optimizer and `sparse_categorical_crossentropy` loss.

3. **Training**:
   - Train for 30 epochs with early stopping (`patience=3`) and model checkpointing.
   - Batch size of 64 for efficient training.

4. **Evaluation**:
   - Evaluate accuracy on test data.
   - Generate confusion matrices and classification reports.
   - Visualize training/validation accuracy and loss curves.

5. **Prediction**:
   - Predict rice classes for new images using saved models.

<br>

### Key Features
- **Dual Model Approach**: Compare a custom CNN with a pre-trained ResNet50 model.
- **Data Augmentation**: Enhances generalization using real-time augmentation layers.
- **Visualization Tools**: Plot training history, confusion matrices, and sample predictions.
- **Transfer Learning**: Utilize ResNet50 weights for improved performance.
- **Model Persistence**: Save/load models for deployment or further use.

<br>

### Results
- **Custom CNN**:  
  - Test Accuracy: **98%**  
  - Validation Accuracy: ~97% (at epoch 8/30, early stopping)  
- **ResNet50**:  
  - Test Accuracy: **99%**  
  - Validation Accuracy: ~99% (at epoch 14/30)  
- **Confusion Matrices**: Show minimal misclassifications, with ResNet50 outperforming the custom CNN.  
- Detailed metrics available in classification reports (precision, recall, F1-score).

<br>

### Repository Contents
- **`rice_classification.ipynb`**: Jupyter Notebook with full code, visualizations, and explanations.
- **`Data`:** Contains the [Original Dataset](https://www.kaggle.com/datasets/muratkokludataset/rice-image-dataset/data) and you can see the cleaned dataset in notebook.
- **`README.md`:** Project documentation.

<br>

### How to Contribute
Contributions are welcome! If you'd like to improve the project or add new features:

1. **Fork the repository.**
2. **Create a new branch.**
3. **Make your changes and submit a pull request.**
