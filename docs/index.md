## Summary
Recycling can be difficult and confusing, which is why many people skip this step when discarding waste. Instead of taking the time to differentiate and separate each type of recyclable waste, I agree that it is much easier to just toss everything in the same garbage pile. However, with landfills causing harm to our environment and the increase in single-use plastics, waste is one of the largest environmental issues even though it's often ignored. In the US, less emphasis is put on recycling, and many households don't put in the effort to properly recycle waste. I wanted to see if machine learning can make recycling easier with image classification. Previously, I have worked with machine learning and classification using supervised learning. However, I wanted to learn how to classify images, and through research and helpful websites, I was able to complete this project. For the dataset, I used images (from https://github.com/garythung/trashnet) of cardboard, plastic, paper, glass, and metal items. 
Electronic waste is also a prevalent issue that should be addressed. Especially with planned obsolescence shortening the life-span of phones, tablets, and other electronics, an increasing amount of "older model" electronics are ending up in landfills. This e-waste not only is harmful to the environment and workers by emitting and producing deadly chemicals, but it is also contributing to the overabundance of waste on our planet. The amount of worldwide e-waste generation is expected to exceed 50 million tons by 2020. However, e-waste can be recycled and reused in manufacturing electronics, since it is made of valuable metals like copper and gold. Recycling e-waste needs to be prioritized and awareness needs to be raised. Thus, I also included e-waste as a category of classification in this project.

## Data preparation
The dataset of images of recyclable materials includes a couple of thousand images of cardboard, plastic, paper, glass, and metal. I also collected 319 images of e-waste from the internet, like pictures of broken phones, old televisions, broken laptops, e-waste piles, circuit board parts, and other electronics. In Jupyter Notebook, I converted these images into 2-D arrays containing the RGB values per pixel per row. The values are then scaled and split into training and testing sets.

## Model training
I used a Sequential model and added 3 convolutional layers and 2 dense hidden layers with dropout and batch normalization after each layer. Lastly, I added the output layer with 6 neurons for the 6 classes. To decrease overfitting, used Early Stopping to stop training when accuracy is getting worse with each epoch, decreased the size and complexity of the network, and add 2 max pooling layers. 

The model had an average accuracy of 0.412. The accuracies of the training sets were high, but not for the validation sets.
The graph below shows the accuracy changes during the training phase.

![Model accuracy graph](https://github.com/rli1215/Recycling-Image-Classification/model.png)

I used a KerasClassifier to hyperparameter tune the model. The best parameters were determined to be batch size of 16 and 'relu' activation function.
 
![Hyperparameter tuning best parameters](https://github.com/rli1215/Recycling-Image-Classification/hyperparameter%20tuning%20results.png)

After using these parameters, the model had an average accuracy of 0.472. This is slightly better than the model's performance before tuning.

![Tuned model accuracy graph](https://github.com/rli1215/Recycling-Image-Classification/tuned%20model.png)

## Model Testing
When evaluating the model's performance on the testing set, the accuracy was 56.05%. 
Although this is not a high accuracy level, it was higher than when I first started this project. After much research and tweaking to reduce overfitting, I was able to greatly increase accuracy performance. Since this is my first project with image classification and CNN, I am satisfied with this result. I learned a lot about the techniques used and the process of and deep learning. I will continue to my skills in deep learning and image classification and hope to improve the model performance in the future.

Thanks for reading :) I hope you found this interesting!
