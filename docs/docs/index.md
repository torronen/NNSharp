# Welcome to NNSharp

This is the full documentation of NNSharp which is a lightweight library for running pre-trained neural networks. The training should be done in [Keras](https://keras.io/), [TensorFlow](https://www.tensorflow.org/), [Pytorch](http://pytorch.org/docs/) or [Sonnet](https://github.com/deepmind/sonnet) then the weights and the network architecture should be saved into a file (json). NNSharp is able to read and run the network especially on Windows and Visual Studio. 

## Current abilities

NNSharp recently supports Keras models with both Tensorflow and Theano backend. The list of the supported *Keras layers*:

* **Core layers**: Dense, Flatten, Reshape (2D), Permute, RepeatVector. 
* **Convolution layers**: Conv1D, Conv2D, Cropping1D, Cropping2D. 
* **Pooling layers**: AveragePooling1D, AveragePooling2D, MaxPooling1D, MaxPooling2D, GlobalAveragePooling1D, GlobalAveragePooling2D, GlobalMaxPooling1D, GlobalMaxPooling2D.
* **Activations**: softmax, elu, softplus, softsign, relu, tanh, sigmoid, hard_sigmoid. 
* **Recurrent layers**: SimpleRNN, LSTM, GRU.
* **Normalization**: BatchNormalization.

The *data format* supports 2-dimensional data. 

## The structure of the documentation

The purpose of the documentation is twofold:

1. As a user guide to show how to use the package.
2. Providing some further insight how the kernels work in a concise manner. Therefore developers and researchers can immediately understand what the kernel does without inspecting the code or looking for other sources on the net. This can be helpful for contributors as a developer documentation too. On the other hand users can understand what to feed into the network and how to use (and construct) the output.

The structure of the documentation is the following:

* **Installation** shows how to get access to the package.
* **Models** introduces the model types and methods to access information about the model like the contained layers or nodes, execution time etc.
* **Keras** shows the implemented Keras layers. Each layer introduced with its input, output and its underlying process.
* **TensorFlow** shows how to use pre-trained TensorFlow models in NNSharp.

## Future 

In the future the library should provide the following features:

* Supports the whole Keras API.
* Supports TensorFlow models.
* Supports Sonnet.
* Multi-threading for faster kernels.
* Keras-like API over TensorFlow (and may be CNTK) for building, training and running networks. This requires an extended C++ API in TensorFlow and reliable compilation for Windows.

**Contributions are always welcomed!** For the current purposes see the [github repository](https://github.com/adamtiger/NNSharp) of the project.

## Contact

You can do contact me via email if you have questions: adam.8.budai at gmail dot com

