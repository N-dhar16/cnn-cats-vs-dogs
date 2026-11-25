Cats vs Dogs: a CNN image classifier in TensorFlow/Keras

The aim of this project is to train a convolutional neural network (CNN) to classify photos of dogs and cats. The TensorFlow Cats vs Dogs dataset is used for training, validation and testing the model. Corrupt files/images are cleaned, and the remaining images are split into 70% for training, 15% for validation, and 15% for testing. A baseline logistic regression analysis is done as well. The CNN model achieves an accuracy of 84%, and with data augmentation, the accuracy goes up to 90% by reducing overfitting. 

The model is then tested with mirrored, grayscale and darker images. The accuracy fell to 72% for rotated images and 63% for upside-down images. It also wrongly classified images of other animals as dogs or cats. Grad-CAM heatmaps helped show which parts of each image it relied on. The main lesson: a model can score well on familiar data and still be confidently wrong on anything different.

To run it, install TensorFlow, TensorFlow Datasets, scikit-learn, pandas, NumPy and Matplotlib. Then set data_dir in the notebook to the folder containing the Cat and Dog images.

