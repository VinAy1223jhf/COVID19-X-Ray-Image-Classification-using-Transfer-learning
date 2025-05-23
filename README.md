# COVID19 X-Ray Image Classification

## 🎯 Goal
The main purpose of this project is to classify COVID-19 from X-Ray images using various image detection/recognition models and compare their accuracy.

## 🧵 Dataset
The dataset used is available on Kaggle:  
[COVID19 Image Dataset](https://www.kaggle.com/datasets/pranavraikokte/covid19-image-dataset)

## 🧾 Description
This project involves a comparative analysis of five Keras image detection models applied to the dataset:  
- MobileNetV2  
- VGG16  
- InceptionV3  
- DenseNet121  
- Xception  

The project includes training, evaluating, and comparing these models based on accuracy and performance metrics. Additionally, exploratory data analysis (EDA) techniques were used to understand dataset characteristics, label distributions, detect imbalances, and identify improvement areas. The methodology includes data preparation, model training, evaluation, comparative analysis, and visualization of EDA insights.

## 🧮 What I Did
1. **Data Loading and Preparation:**  
   Loaded image paths and labels into a pandas DataFrame for manipulation and analysis.

2. **Exploratory Data Analysis (EDA):**  
   - Created bar and pie charts to visualize label frequency distribution.  
   - Analyzed unique image paths and categorical data variety.  
   - Visualized missing values using heatmaps.  
   - Summarized label counts.

3. **Image Preprocessing and Model Training:**  
   - Preprocessed test images with pixel normalization.  
   - Iterated through models (VGG16, ResNet50, Xception) for predictions.  
   - Saved predictions for further analysis.

4. **Model Prediction Visualization:**  
   - Loaded models and visualized predictions on sample test images.  
   - Adjusted preprocessing for model-specific input sizes (e.g., 299x299 for Xception).

## 🚀 Models Implemented

### Xception
- Pre-trained on ImageNet with 22.9M parameters.  
- Lightweight (88 MB), high accuracy, and fast inference speed.  

### MobileNetV2
- Very lightweight (14 MB), with 3.5M parameters.  
- Uses transfer learning for faster training with limited data.

### VGG16
- Deep architecture with 16 layers.  
- Highest accuracy (~90.1%), but larger size and slower inference.

### InceptionV3
- Moderate size (92 MB), 23.9M parameters.  
- Good accuracy and balanced inference speed.

### DenseNet121
- Lightweight (33 MB) and efficient with 8M parameters.  
- High accuracy and moderate inference speed.

## 📚 Libraries Needed
- NumPy  
- pandas  
- scikit-learn  
- Matplotlib  
- Keras (TensorFlow backend)  
- tqdm  
- seaborn  

## 📊 Exploratory Data Analysis Results
- Bar and pie charts illustrating label distribution.  
- Distribution analysis of top 20 image paths by label.  
- Heatmaps for missing data visualization.

## 📈 Model Performance (Validation Accuracy)
| Model       | Accuracy |
|-------------|----------|
| DenseNet121 | 90%      |
| Xception    | 86%      |
| VGG16       | 80%      |
| MobileNetV2 | 80%      |
| InceptionV3 | 78%      |

## 📢 Conclusion
DenseNet121 and Xception performed best on this dataset. However, the dataset is imbalanced and relatively small, which may affect model generalization.
