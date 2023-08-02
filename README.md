# CV_Module-Project
The provided code performs a multi-class image classification task using transfer learning with the VGG16 model.
The code reads images from a given folder, extracts faces from the images using bounding box coordinates from a CSV file, and prepares the data for training. 
It then applies oversampling using SMOTE to address class imbalance. 
The pre-trained VGG16 model is loaded without its fully connected layers, and a custom top layer with a global average pooling and dense layers is added.
The model is compiled using the Adam optimizer with a learning rate of 0.001 and categorical cross-entropy loss. 
The model is then trained on the preprocessed data with data augmentation using the ImageDataGenerator. 
After training, the model is evaluated on the test dataset, and the test accuracy is printed.
