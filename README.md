SkinAlyze
A CNN-Based Skin Lesion Classifier Using the HAM10000 Dataset

SkinAlyze is a deep learning project that classifies dermoscopic skin images into seven medical diagnostic categories. It leverages a Convolutional Neural Network (CNN) trained on the HAM10000 dataset to assist in identifying both benign and malignant skin conditions.

Features
Organized dataset into class-specific folders for streamlined model input

Trained a CNN model on over 5,000 images of skin lesions

Evaluated model performance using training/validation accuracy and loss

Generated classification reports and confusion matrices for performance analysis

Enabled image upload and real-time prediction with diagnosis output

Displayed full diagnostic labels with prediction confidence

Saved trained model in .h5 format for reuse and deployment

Supported Skin Lesion Types
Code	Diagnosis	Category
nv	Melanocytic nevus (mole)	Benign
mel	Melanoma	Malignant
bkl	Benign keratosis-like lesion	Benign
bcc	Basal cell carcinoma	Malignant
akiec	Actinic keratosis / intraepithelial carcinoma	Malignant
vasc	Vascular lesion	Benign
df	Dermatofibroma	Benign

Usage (Google Colab)
Mount your Google Drive and upload the dataset and metadata

Train the model using the provided code

Upload a dermoscopic image and run the prediction function:

predict_uploaded_image()
Sample output:
Processing file: ISIC_0029305.jpg
Predicted Type: Melanocytic nevus (mole)
Confidence: 0.70
Project Structure
HAM10000_metadata.csv – Metadata including image IDs and diagnostic labels

HAM10000_images_part_1/ – Directory containing dermoscopic images

skin_cancer_model.h5 – Trained model file

skin_lesion_classifier.ipynb – Jupyter Notebook with training and inference code

Future Enhancements
Integrate transfer learning using pretrained models (e.g., MobileNetV2)

Add an interactive web interface (Gradio or Streamlit)

Improve classification accuracy for underrepresented lesion types

Convert the model to TensorFlow Lite for mobile and edge deployment
