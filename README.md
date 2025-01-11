## Rice Classification
[![](Image.jpg)](https://unsplash.com/photos/aerial-view-photography-of-rice-crops-during-daytime-cusz0Bg-5mQ)

### Overview
This project focuses on classifying five different rice varieties commonly grown in Turkey: Arborio, Basmati, Ipsala, Jasmine, and Karacadag. Using a dataset of 75,000 grain images (15,000 per variety), a Convolutional Neural Network (CNN) model was developed to accurately distinguish between these varieties based on their texture, shape, and color features.  

The project demonstrates the potential of deep learning for agricultural applications, particularly in automating the classification and quality assessment of grains.  

<br>

### **Project Workflow**  
1. **Data Preparation**:  
   - Collected a dataset comprising 75,000 images of rice grains, categorized into five varieties.  
   - Resized all images to a uniform size of 256x256 pixels for consistent input to the CNN model.  
   - Split the dataset into training, validation, and test sets to ensure reliable evaluation of the model.  

2. **Model Development**:  
   - Designed a CNN architecture with three convolutional layers, max-pooling layers, a dense layer, and a dropout layer to prevent overfitting.  
   - Compiled the model using the Adam optimizer and categorical crossentropy loss function.  

3. **Training**:  
   - Trained the CNN model on the prepared dataset for multiple epochs, monitoring accuracy and validation loss to fine-tune performance.  

4. **Evaluation**:  
   - Tested the model on unseen data to assess its generalization ability.  

<br>

### **Key Features**  
- **Extensive Dataset**: Utilized a large dataset with 75,000 images across five rice varieties.  
- **Deep Learning**: Implemented a CNN architecture tailored for image classification tasks.  
- **Automated Classification**: Achieved accurate predictions for rice varieties based on their unique features.  
- **Scalability**: The methodology can be extended to classify other agricultural products.  

<br>

### **Results**  
- The CNN model achieved an accuracy of **`98%`** on the test dataset, effectively classifying the five rice varieties.  
- This result highlights the potential of deep learning in enhancing agricultural automation and quality control processes.  

<br>

### Repository Contents

- **`Data`:** Contains the [Original Dataset](https://www.kaggle.com/datasets/muratkokludataset/rice-image-dataset/data) and you can see the cleaned dataset in notebook.
- **`Notebook`:** Jupyter notebook detailing the entire process, including data cleaning, visualization and modeling.
- **`README.md`:** Project documentation.

<br>

### How to Contribute
Contributions are welcome! If you'd like to improve the project or add new features:

1. **Fork the repository.**
2. **Create a new branch.**
3. **Make your changes and submit a pull request.**
