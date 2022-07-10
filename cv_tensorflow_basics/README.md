# Tensorflow Computer Vision

### Dataset example for computer vision 
**Fashon MNIST**
- Details
    - 70k images
    - 10 categories
    - images are 28x28
- This dataset has low iow data per image but you can still distinguish the category
    - Minimizing input data improves perfomance and training speed
- labels are numeric insted of in a particular language to avoid biasing to a particular language
- this dataset is available in the tensorflow library under tensorflow.datasets.fashion_mnist
- https://github.com/zalandoresearch/fashion-mnist

### How to load dataset from tensorflow
`fashion_mnist = tf.keras.datasets.fashion_mnist`
`(train_images, train_labels), (test_images, test_labels) = fashion_mnist.load_data()`

### Avoiding Bias
- Bias is important to avoid because it can cause harm
- NN can get bias from the training data
- Some info on how to combat bias is found here:
- https://ai.google/responsibilities/responsible-ai-practices/

### Layers Types
- Flatten layer
    - this layer takes a multi demension array (like an image) and flattens it into a 1D array so a NN can use it.
- Dense layer
    - a layer of just neurons

### Activations
**relu**
    - rectified linear unit function.
    - it is just y=x for terms greater than x=0 and for x<0, y=0
**softmax**
    - an s curve function
    - like a sine wave centered on 0,0 and x is between -1 and 1

### Callback in training
- each training loop calls on_epoch_end()
- if you define the function you can end the training when metrics are met.

### Where to get Images
Pixabay