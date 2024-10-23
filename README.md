# Fashion-MNIST Classification with Feed-Forward Neural Networks

A comprehensive comparison of different feed-forward neural network architectures for classifying the Fashion-MNIST dataset.

## Dataset
The Fashion-MNIST dataset consists of 60,000 training images and 10,000 test images of fashion items, categorized into 10 classes:
- T-shirt/Top
- Trouser
- Pullover
- Dress
- Coat
- Sandal
- Shirt
- Sneaker
- Bag
- Ankle Boot

Each image is a 28x28 grayscale image, making the input dimension 784 (flattened).

## Model Architectures
I implemented and compared three different feed-forward neural network architectures:

1. Narrow Model (Simple)
   - Input Layer: 784 neurons
   - Hidden Layer 1: 128 neurons with ReLU
   - Hidden Layer 2: 64 neurons with ReLU
   - Output Layer: 10 neurons

2. Wide Model
   - Input Layer: 784 neurons
   - Hidden Layer 1: 512 neurons with ReLU + Dropout(0.3)
   - Hidden Layer 2: 256 neurons with ReLU + Dropout(0.3)
   - Output Layer: 10 neurons

3. Deep Model
   - Input Layer: 784 neurons
   - Hidden Layer 1: 256 neurons with ReLU + Dropout(0.2)
   - Hidden Layer 2: 128 neurons with ReLU + Dropout(0.2)
   - Hidden Layer 3: 64 neurons with ReLU + Dropout(0.2)
   - Hidden Layer 4: 32 neurons with ReLU + Dropout(0.2)
   - Output Layer: 10 neurons

Each architecture was trained with three different optimizers:
- SGD (lr=0.01)
- Adam (lr=0.001)
- RMSprop (lr=0.001)

## Using the code
-have main.py in the same folder as the codes in src
-run main.py
