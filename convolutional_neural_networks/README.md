# Convolutiona Neural Networks (AKA ConvNets)

Simply checking every pixel in an image is naive and it can require a lot of processing

Using ConvNets and Pooling we can create algorithms that can better identify features of a particular object to classify.

**ConvNets**
- A matrix operation that can highlight important features in an image.
- A Convolution will reduce the size of the matrix by the window size - 1.
https://www.tensorflow.org/api_docs/python/tf/keras/layers/Conv2D

Conv2D(number_of_filters=64, fliter_size=(3,3), activation=`relu`, input_shape(28,28,1))
- filters start with a set of known good filters and are improved over time
- each filter is good for detecting different features like vertical lines, horizontal lines, cuvers...
- a conv layer tests the filters to see which produce the best results for the training data.

more details: https://bit.ly/2UGa7uH
https://lodev.org/cgtutor/filtering.html

**Pooling**
- a way of compressing an image to reduce the processing required.
https://www.tensorflow.org/api_docs/python/tf/keras/layers/MaxPool2D

MaxPooling2D(2,2)
- max means that the max pixel will survive in the window