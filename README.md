 # Lymphocyte segmentation with logistic regression
The purpose of this project is the creation of logistic regression model capable of segmenting lymphocytes in H&E staining of human tissue images. 
The dataset used to train and test model is from MoNuSAC 2020 challenge.

The project is composed of the following files:
- `logistic_regression.ipynb`: Main file detailing the training and testing of the models.
- `Binary_mask_generation.ipynb`: Code given with the MoNuSAC dataset. The imports have been modified to work on a Windows machine. Used to generate binary PNG masks from the XML files of dataset.
- `lr_model.pkl`, `lr_model_total`, `lr_model_ws`: Trained logistic regression models.
- `MoNuSAC_masks`, `MoNuSAC_test_masks`: folders containing the binary masks for the training and test set respectively

==Remarks==
- Although they are not present in the repository, the code assumes the presence of the training and test sets in the same directory. The sets should be stored in folders named `MoNuSAC_images_and_annotations` and `MoNuSAC_test` respectively.
- Some XML files from the test set were not correctly formated. This caused the binary mask generation code to return errors. The corresponding images were thus not used for the testing of the model. It is thus advised to simply run the code with binary masks present in the `MoNuSAC_masks` and `MoNuSAC_test_masks` folders.