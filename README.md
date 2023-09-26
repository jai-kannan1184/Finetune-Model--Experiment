# Finetune-Model--Experiment
An experiment to compare if LLMs can identify and suggest hyperparameters based on architectural differences.
## Architecture Comparison

### CNN vs Modified CNN
### Kernel Sizes, Pooling, and Normalization:
- **CNN** uses 3x3 convolutional kernels, max-pooling, and no Batch Normalization.
- **ModifiedCNN** uses 5x5 kernels, introduces average pooling, and includes Batch Normalization layers.

### Complexity and Batch Normalization:
- **CNN** is relatively simpler with only convolutional and fully connected layers.
- **ModifiedCNN** adds complexity with different kernel sizes, pooling types, and Batch Normalization layers.

### MLP vs Modified MLP:

- **MLP**  architecture has three fully connected (linear) layers followed by ReLU activation and dropout. It has one dropout layer with a dropout rate of 0.5.
- **ModifiedMLP** has four fully connected layers with LeakyReLU activations, two dropout layers with different dropout rates (0.4 and 0.6), and three Batch Normalization layers.

### Layer Sizes:
- **MLP** has larger fully connected layers with 4096 units in the first and second layers and 1000 units in the third layer.
- **ModifiedMLP** has smaller fully connected layers with 2048 units in the first and third layers, 4096 units in the second layer, and 1000 units in the fourth layer.

### Activation Functions:
- **MLP** uses ReLU activation throughout the network.
- **ModifiedMLP** employs LeakyReLU activation.

### ResNet vs ModifiedResNet:

### Layer Types and Normalization:
- **ResNet** consists of basic blocks with 3x3 convolutional layers, Batch Normalization, ReLU activation, and skip connections.
- **ModifiedResNet** utilizes dilated blocks with 5x5 dilated convolutional layers, Group Normalization and skip connections.

### Layer Sizes:
- The first convolutional layer in **ResNet** has 64 output channels, whereas **ModifiedResNet** has 128 output channels.

### Activation Functions:
- **ResNet** uses ReLU activation throughout the network.
- **ModifiedResNet** incorporates Tanh activation  which is used for dilated convolutions and Group Normalization instead of Batch in comparision.




