# Self-Pruning Neural Network

This project implements a neural network that learns to prune its own weights during training using learnable gate parameters.


Each weight is multiplied by a sigmoid gate.
L1 regularization is applied on these gates to encourage sparsity.


| Lambda | Accuracy | Sparsity |
| ------ | -------- | -------- |
| 0.001  | ~49%     | ~0%      |
| 0.01   | 43%      | 60%      |
| 0.1    | 35%      | 60%      |

* Higher lambda → more pruning
* Trade-off between accuracy and model size
* Model learns to remove unnecessary connections

* Python
* PyTorch
* CIFAR-10


```bash
pip install torch torchvision matplotlib
```

Run the notebook step by step.

Aryan Raj
