# Hybrid Neural Network with Quantum Annealer Integration
This repository explores a hybrid model for classification that combines a classical neural network with a quantum annealer. The classical neural network optimizes the controls of a quantum annealer to maximize inter-class differences and minimize intra-class differences. While previous research demonstrated the potential of quantum annealers for specific linear datasets, our findings suggest that incorporating a quantum annealer into a classical neural network does not significantly enhance performance across a variety of datasets. However, by tuning hyperparameters and utilizing advanced techniques, we observed improved model accuracy, offering insights into optimizing hybrid quantum-classical models.
Abstract

Our research presents an investigation into hybrid neural network architectures, particularly examining the integration of quantum annealers. Through this work, we:

    Tested different datasets (MNIST, SVHN, Fashion MNIST) to assess the effect of dataset choice on hybrid NN performance.
    Experimented with variations in quantum embedding, such as using quantum gates instead of Hamiltonian evolution.
    Scaled from a 2-qubit to a 10-qubit system, enabling the model to represent a broader state space.
    Tuned hyperparameters, particularly using a StepLR learning rate scheduler, to enhance performance.

Ultimately, we found that hyperparameter tuning, especially in learning rate scheduling, produced positive improvements in the hybrid model’s accuracy.
Key Concepts

Keywords: Quantum Entanglement, Quantum Superposition, Quantum Decoherence, Quantum Error Correction, Quantum Algorithms, Quantum Simulation
Introduction

Quantum computing presents promising enhancements for machine learning, especially through kernel-based methods. Quantum annealers, while less flexible than universal gate quantum computers, offer a more practical tool for heuristic optimization. Our work builds upon previous hybrid quantum-classical classification models by:

    Using a neural network to control the annealing schedule of a quantum annealer.
    Incorporating the quantum state output as a guide for gradient descent, improving parameter optimization.
    Exploring classical datasets, such as MNIST and CIFAR, alongside SVHN and Fashion MNIST.

In our approach, we began with a 2-qubit setup suitable for basic tasks, then scaled to 10 qubits, enhancing the model's capability to represent 1024 simultaneous states. Hyperparameter tuning, particularly with the StepLR learning rate scheduler, emerged as a critical factor in improving our model's accuracy.
Enhancements and Findings

    Dataset Experimentation: Initially used MNIST, then expanded to SVHN and Fashion MNIST for more comprehensive testing.
    Quantum Embedding Variation: Shifted from Hamiltonian evolution to quantum gate embeddings.
    Hyperparameter Tuning: Implemented StepLR learning rate scheduling with the Adam optimizer, beginning with a learning rate of 0.0001.
    Scalability: Transitioned from a 2-qubit to a 10-qubit system, allowing the model to represent a larger state space, thus enhancing its computational capacity.

#Repository Structure

plaintext

├── data/                   # Contains datasets used in the experiments
├── models/                 # Neural network models and quantum annealing layer
├── scripts/                # Training and testing scripts
├── results/                # Experimental results and accuracy logs
├── README.md               # Overview of the project
└── requirements.txt        # Required packages and dependencies

Getting Started
