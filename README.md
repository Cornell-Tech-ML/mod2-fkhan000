[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/YFgwt0yY)
# MiniTorch Module 2

<img src="https://minitorch.github.io/minitorch.svg" width="50%">


* Docs: https://minitorch.github.io/

* Overview: https://minitorch.github.io/module2/module2/

This assignment requires the following files from the previous assignments. You can get these by running

```bash
python sync_previous_module.py previous-module-dir current-module-dir
```

The files that will be synced are:

        minitorch/operators.py minitorch/module.py minitorch/autodiff.py minitorch/scalar.py minitorch/scalar_functions.py minitorch/module.py project/run_manual.py project/run_scalar.py project/datasets.py

## Task 2.5: Training

For Task 2.5, in order to test that we implemented autodifferentiation with tensors correctly, we were instructed to train an MLP on four classification datasets. Each dataset consists of a grid of points on a 2D plane, which we need to classify into two categories.

---

### Simple Dataset

For the Simple dataset, after some experimentation, I achieved **100% accuracy** by configuring my model with:

- **5 nodes** in each hidden layer
- **Learning rate**: 0.05
- **Epochs**: 500

The figure below shows the training log, the loss function over training epochs, and the decision boundary found.

<img width="1010" alt="simple_train" src="https://github.com/user-attachments/assets/7ba22e3a-2213-49ed-8d89-bd2bfbd2eb96">

---

### Diag Dataset

For the Diag dataset, I used the same configuration:

- **11 nodes** per hidden layer
- **Learning rate**: 0.1
- **Epochs**: 500

The figure below shows the training log, the loss function over training epochs, and the decision boundary found.



---<img width="980" alt="diag_train" src="https://github.com/user-attachments/assets/079f1e1d-f651-4928-ae16-65640518b4ca">


### Split Dataset

For the Split dataset, I used the same configuration:

- **11 nodes** per hidden layer
- **Learning rate**: 0.1
- **Epochs**: 500

The figure below shows the training log, the loss function over training epochs, and the decision boundary found.

<img width="1197" alt="split_train" src="https://github.com/user-attachments/assets/ed1e16b2-0ed5-4669-a66c-792e19c4434b">


---

### XOR Dataset

For the XOR dataset, I again used the configuration with:

- **20 nodes** per hidden layer
- **Learning rate**: 0.05
- **Epochs**: 800

The figure below shows the training log, the loss function over training epochs, and the decision boundary found.


<img width="1196" alt="xor_train" src="https://github.com/user-attachments/assets/484812e5-67de-49e6-9b98-90ce797f996b">

---



