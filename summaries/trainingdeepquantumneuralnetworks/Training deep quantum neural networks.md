---
layout: page
title: Training deep quantum neural networks
date: 2023-12-18 16:25:42
---

[Back](./)


The authors of this article propose a quantum analogue of classical neurons, creating quantum feedforward neural networks that are capable of universal quantum computation. They describe an efficient training method using fidelity as a cost function, which can be implemented both classically and with quantum methods. This method allows for fast optimization with reduced memory requirements, scaling the number of qubits with only the width of the network. The authors benchmark their proposal for the quantum task of learning an unknown unitary and find remarkable generalization behavior and robustness to noisy training data.

Machine learning has had widespread success in both research and industry, particularly with the use of neural networks and the backpropagation algorithm. However, with the advent of quantum technology, it is important to design quantum neural networks for fully quantum learning tasks. Quantum machine learning is still in its early stages, with various approaches to utilizing quantum computing devices for machine learning tasks. One approach is to use classical machine learning to improve quantum tasks, while another is to use quantum algorithms to speed up classical machine learning. The third approach, which the authors focus on, is using quantum computing devices to carry out learning tasks with quantum data. The authors propose a quantum analogue of classical neurons, which can be combined to form quantum neural networks capable of universal quantum computation.

The building blocks of a quantum neural network are quantum perceptrons, which are quantum analogues of perceptrons used in classical machine learning. A quantum perceptron is an arbitrary unitary operator that acts on input and output qubits, with the parameters incorporating the weights and biases of previous proposals in a natural way. The authors propose a training algorithm for the quantum neural network that only depends on the width of the individual layers and not on the depth of the network. This algorithm allows for efficient calculation of the parameter matrices, reducing the memory requirements of the algorithm.

The authors simulate the learning tasks of the quantum neural network using pilot simulations with small widths of input and output spaces. They study the ability of the network to generalize from a limited set of random training pairs and find that the network matches the theoretical estimate of the optimal cost function. They also evaluate the robustness of the network to corrupted training data and find that the network is extremely robust to this kind of error.

One key feature of the proposed quantum neural network algorithm is the absence of a "barren plateau" in the cost function landscape. The authors attribute this to the nongeneric structure of the network and the fact that the gradient of a weight in the network depends only on the number of paths connecting that neuron to the output.

Overall, the proposed quantum neural network and training algorithm show remarkable capabilities, including generalization, robustness to noisy training data, and absence of a barren plateau in the cost function landscape. These findings suggest that the algorithm can be applied to noisy intermediate-scale quantum devices.

Words: 503