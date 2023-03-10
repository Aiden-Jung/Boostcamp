# [Day 5] AI Math - CNN & RNN

## 1. CNN

- CNN (Convolutional Neural Network)
  - In deep learning, a convolutional neural network (CNN, or ConvNet) is a class of artificial neural network (ANN), most commonly applied to analyze visual imagery. CNNs are also known as Shift Invariant or Space Invariant Artificial Neural Networks (SIANN), based on the shared-weight architecture of the convolution kernels or filters that slide along input features and provide translation-equivariant responses known as feature maps. [1]
- Kernel
  - A kearnel is a small matrix of weights that is used to convolve over an input matrix. The kernel slides over the input matrix in a series of operations called convolutions, which involve element-wise multiplication of the kernel with a local region of the input, followed by summing up the products to produce a single output value.
- Why?

  - Parameter Efficiency: Traditional neural networks have a very large number of parameters, which makes them difficult to train and prone to overfitting. CNNs, on the other hand, have a smaller number of parameters due to the use of convolutional and pooling layers. This makes them more parameter-efficient and easier to train on large datasets.

  - Translation Invariance: In traditional neural networks, a small change in the input can result in a large change in the output, which can be a problem for visual data that often has small variations due to changes in lighting, orientation, or position. CNNs, however, are designed to be translation-invariant, meaning they can recognize the same pattern regardless of its location in the input image.

  - Feature Learning: CNNs are capable of automatically learning features from raw data, without the need for manual feature extraction. This is especially important for visual data, which can have complex and high-dimensional feature spaces that are difficult to analyze by humans.

  - Hierarchical Representation: CNNs use a hierarchical representation of features, where each layer learns increasingly complex and abstract features from the previous layer. This allows CNNs to capture the spatial relationships and context between different features in the input, which is important for visual recognition tasks.

  - State-of-the-art Performance: CNNs have achieved state-of-the-art performance on a wide range of visual recognition tasks, such as image classification, object detection, semantic segmentation, and facial recognition. This makes them essential for applications such as self-driving cars, medical image analysis, and security systems.

- Backpropagation
  - Similar as MLP(Multi-Layer Perceptron) but with a kernel

## 2. RNN

- RNN
  - A recurrent neural network (RNN) is a class of artificial neural networks where connections between nodes can create a cycle, allowing output from some nodes to affect subsequent input to the same nodes. This allows it to exhibit temporal dynamic behavior. [2]
- Why?

  - Variable Input/Output Lengths: RNNs can handle variable-length input sequences and generate variable-length output sequences, making them useful for tasks such as speech recognition, natural language processing, and time series prediction.

  - Memory: RNNs have memory capabilities, which allows them to remember information from previous time steps and use it to make predictions at the current time step. This is particularly useful for tasks that require a contextual understanding of the input, such as machine translation or sentiment analysis.

  - Feedback Loop: RNNs have a feedback loop that allows information to flow from the output back into the input. This allows the network to make predictions based on the previous output, which can be important for tasks such as handwriting recognition or music generation.

  - Hierarchical Representation: Like CNNs, RNNs use a hierarchical representation of features, where each time step learns increasingly complex and abstract features from the previous time step. This allows RNNs to capture the temporal dependencies between the input data points.

  - State-of-the-art Performance: RNNs have achieved state-of-the-art performance on a wide range of sequential data tasks, such as language modeling, machine translation, speech recognition, and music generation.

- Most Important Reason
  - Sequence Data
- Backpropagation
  - BPTT (BackPropagation Through Time)
- Problem
  - Gradient Vanishing
    - Solution
      - LSTM (Long Short-Term Memory)
      - GRU (Gated Recurrent Unit)

<!-- Reference -->

[1]: https://en.wikipedia.org/wiki/Convolutional_neural_network
[2]: https://en.wikipedia.org/wiki/Recurrent_neural_network
