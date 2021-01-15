# Recycling Image Classification
This Deep Learning project classifies images of recycleable materials, using CNN, into 6 categories: cardboard, glass, metal, paper, plastic, and e-waste.

The 'recycling image classification project' Jupyter Notebook contains the code to run this project, including data preparation, model construction, training, and testing. (The hyperparameter tuning section takes a while to run, can skip running this section as the best parameters are already determined)
 'dataset-resized.zip' contains 403 cardboard images, 501 glass images, 410 metal images, 594 paper images, 482 plastic images, 319 ewaste images. 
 Download and unzip the file 'dataset-resized.zip' in the same directory as the Jupyter Notebook to generate the dataset from the images.
If you just want to use the model to predict a given image, download CNN.model in the same directory as the Jupyter Notebook. Run the last section in the notebook, "Predicting an image class", and replace the image path with the specific image you want to test with. Run the cell to see the model's prediction.

'model.png' is a line graph of the accuracy of training and validation set at each epoch when fitting the model. 'tuned model.png' is the line graph when fitting after the model is hyperparameter tuned.
'hyperparameter tuning results.png' shows the best parameters printed after hyperparameter tuning. 
