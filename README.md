# image_classification_cnn

## Use
Just to save my progress I made in learning image classification this is from a tutorial I saw.

This code uses a pre-trained VGG16 model, available in the Keras deep learning library, to classify an input image.

First, the VGG16 model is loaded with pre-trained weights from the ImageNet dataset. The summary of the model architecture is printed to the console using the model.summary() method.

Next, an input image is loaded using the load_img() function from Keras' preprocessing module. The image is loaded in RGB format and resized to 224x224 pixels, which is the required input size for VGG16. The image is then converted to a 3D NumPy array using img_to_array().

Since the VGG16 model expects input data in a 4D array with the first dimension representing the number of images, a new dimension is added to the array using np.expand_dims().

Before feeding the input image to the VGG16 model, the preprocess_input() function from Keras' applications module is applied to center the pixel values with respect to the ImageNet dataset.

Finally, the preprocessed image is passed through the VGG16 model using the predict() method, and the top 5 predicted classes with their probabilities are printed to the console using the decode_predictions() function from Keras' applications module.

Overall, this code demonstrates how to use a pre-trained deep learning model to classify images with high accuracy.
