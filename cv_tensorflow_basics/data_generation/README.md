# ImageDataGenerator in Tensorflow

- Having too well formated data or too specific data will result in a overfitted network
- Datasets do not always come pre-labeled

ImageDataGenerator in Tensorflow fixes this by 
- labeling images in subdirectories
- resizes test/validation images so they are in uniform size for the neural network


# ConvNet architecture for complex images #1

    Con2D
    MaxPooling2D
    Conv2d
    MaxPooling2D
    Conv2D
    MaxPooling2D
    Flatten
    Dense
    Dense


# Optimizer
RMSProp
- http://www.cs.toronto.edu/~tijmen/csc321/slides/lecture_slides_lec6.pdf
- https://www.tensorflow.org/api_docs/python/tf/keras/optimizers/RMSprop

# Loss Function
Binary Crossentropy
- https://gombru.github.io/2018/05/23/cross_entropy_loss/
- https://www.youtube.com/watch?v=eqEc66RFY0I&t=6s