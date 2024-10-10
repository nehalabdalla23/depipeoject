Project Title: CAPTCHA Animal Image Translation

Description:

This project focuses on translating CAPTCHA animal images to determine if a user has correctly chosen images belonging to the same class as the suggested image. The dataset consists of 80 classes of animal images, totaling 10GB.

A] Dataset Structure:

train folder: Contains 80 subfolders, each representing a different animal class.
test folder: Contains 80 subfolders, each representing a different animal class.
Each subfolder: Contains a text file with the class label .

B] Data Preprocessing:

1-Undersampling: The dataset was undersampled to 45 classes to balance the classes.
2-Resizing: The dataset was resized to be 225x255 and grey scale with the dimentions (225,225,1)
3-Normalizing: The dataset was normalized so that the value of each pixel vary between (0,1)
4-Positive and Negative Pairs: Images were split into positive and negative pairs for training and testing. Positive pairs contain images from the same class, while negative pairs contain images from different classes.
5-Positive and Negative label Pairs: labels were given to each pair as if they are from the same class label would be 1 other wise it's 0.

C] Model Architecture:

Siamese Network: A Siamese network is used to compare image pairs and determine their similarity.
Contrastive Loss: The contrastive loss function is used to train the network, aiming to minimize the distance between positive pairs and maximize the distance between negative pairs.

D] Usage:

Clone the repository: git clone <[your_repository_url](https://github.com/Toka-source/Captcha_Depi)>
Install dependencies: pip install -r requirements.txt
Train the model: Run the training script (e.g., train.py)
Test the model: Run the testing script (e.g., test.py)

E] Dependencies:

TensorFlow/Keras
os
pandas
seaborn
NumPy
PIL
Matplotlib (for visualization)
zipfile
shutil

Other relevant libraries (specify in your requirements.txt file)



-Colab_Source_Code:https://colab.research.google.com/drive/1LU-Z3aFENVK_iVnmkG3Xajtofiij6J7e?authuser=1#scrollTo=sEHgkWk0lOtm
-Dataset Source:https://www.kaggle.com/datasets/antoreepjana/animals-detection-images-dataset
