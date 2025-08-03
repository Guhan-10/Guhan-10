SkinAlyze: Skin Lesion Classification Using CNN
SkinAlyze is a deep learning-based skin lesion classification tool built on the HAM10000 dataset. It uses a Convolutional Neural Network (CNN) to categorize dermoscopic images into seven distinct types of skin conditions, including both benign and malignant lesions.

Features:
>> Preprocesses and organizes the HAM10000 dataset by lesion class
>> Trains a CNN on over 5,000 curated dermoscopic images
>> Evaluates model performance using accuracy, loss, and classification metrics
>> Accepts user-uploaded images for on-the-fly diagnosis
>> Outputs the full lesion name and confidence score
>> Saves the trained model in .h5 format for later use or deployment

Supported Skin Lesion Types:
Code	   Diagnosis	Category
nv	     Melanocytic nevus (mole)	Benign
mel	     Melanoma	Malignant
bkl	     Benign keratosis-like lesion	Benign
bcc	     Basal cell carcinoma	Malignant
akiec	   Actinic keratosis / intraepithelial carcinoma	Malignant
vasc	   Vascular lesion	Benign
df	     Dermatofibroma	Benign

Usage (Google Colab):
Mount Google Drive and upload the HAM10000 metadata and image files.

Train the model using the provided notebook.

Upload a dermoscopic image using files.upload().

Call the prediction function:


predict_uploaded_image()

Example output:
Processing file: ISIC_0029305.jpg
Predicted Type: Melanocytic nevus (mole)
Confidence: 0.70

File Structure:

=> HAM10000_metadata.csv – Metadata with diagnosis labels
=> HAM10000_images_part_1/ – Folder containing image dataset
=> skin_cancer_model.h5 – Saved trained model
=> skin_lesion_classifier.ipynb – Jupyter notebook with full workflow

<!---
Guhan-10/Guhan-10 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
