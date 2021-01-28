# Recycling Image Classification
This Deep Learning project classifies images of recycleable materials, using CNN, into 6 categories: cardboard, glass, metal, paper, plastic, and e-waste.

The 'recycling image classification project' Jupyter Notebook contains the code to run this project, including data preparation, model construction, training, and testing. (The hyperparameter tuning section takes a while to run, can skip running this section as the best parameters are already determined)
 'dataset-resized.zip' contains 403 cardboard images, 501 glass images, 410 metal images, 594 paper images, 482 plastic images, 319 ewaste images. 
 Download and unzip the file 'dataset-resized.zip' in the same directory as the Jupyter Notebook to generate the dataset from the images.
If you just want to use the model to predict a given image, download CNN.model in the same directory as the Jupyter Notebook. Run the last section in the notebook, "Predicting an image class", and replace the image path with the specific image you want to test with. Run the cell to see the model's prediction.

Line graph of the accuracy of training and validation set at each epoch when fitting the model:

![Hyperparameter tuning best parameters](https://github.com/rli1215/Recycling-Image-Classification/blob/main/docs/model.png)

Line graph of accuracy when fitting after the model is hyperparameter tuned:

![Hyperparameter tuning best parameters](https://github.com/rli1215/Recycling-Image-Classification/blob/main/docs/tuned%20model.png)

Best parameters printed after hyperparameter tuning:

![Hyperparameter tuning best parameters](https://github.com/rli1215/Recycling-Image-Classification/blob/main/docs/hyperparameter%20tuning%20results.png)
