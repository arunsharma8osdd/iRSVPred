# iRSVPred: A web server for artificial intelligence based prediction of major basmati paddy seed varieties

This repository contains:
1. Sample training set images: train.zip
2. Sample validation set images: validation_set.zip
3. Scripts used to augment the original images: CLoDSA_augmentation_scripts.zip
4. Two iRSVPred prediction models: Model_RICE_WC_251.zip and Model_RICE_WC_502.zip
5. Code used for training the iRSVPred prediction model (251 epochs based): train_model_251_epochs.py
6. Code used for training the iRSVPred prediction model (502 epochs based): train_model_502_epochs.py
7. Code used for validation of the iRSVPred prediction model (251 epochs based): validate_model_251_epochs.py
8. Code used for validation of the iRSVPred prediction model (502 epochs based): validate_model_502_epochs.py

# Frequently asked questions:

# Question. How to train deep learning models using above given codes?

# Answer.

You have to store your training set images in directory named "train" as given in train.zip and run command as given below:

I) To develop 251 epochs based model:
python train_model_251_epochs.py

II) To develop 502 epochs based model:
python train_model_502_epochs.py

The above mentioned codes have all steps in common except the number of iterations and titles of training plots. These will train deep learning models and save. For each epoch, 80% data will be used in training the models and rest 20% for internal validation of trained models. Moreover, training and validation accuracy along with validation loss will be printed on terminal window. After last epoch, model will save automatically (with model's name given within the script) and a figure will also generate. The generated figure will have training and validation accuracy along with validation loss plotted on y-axis while number of epochs on x-axis. 




