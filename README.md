# Lymphocyte segmentation with logistic regression
The purpose of this project is the creation of logistic regression model capable of segmenting lymphocytes in H&E staining of human tissue images. 
The dataset used to train and test model is from MoNuSAC 2020 challenge.

The project is composed of the following files:
- `logistic_regression.ipynb`: Main file detailing the training and testing of the model.
- `Binary_mask_generation.ipynb`: Part of the code given with the MoNuSAC dataset. Used to generate binary masks from the XML files of dataset.
- `lr_model.pkl`: Trained logistic regression model.