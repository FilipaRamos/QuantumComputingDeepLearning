# Quantum Software Frameworks for Deep Learning

Paper by <a href="https://scholar.google.com/citations?user=lyhWwOIAAAAJ&hl=pt-PT" target="_blank">Filipa Ramos</a>, <a href="https://scholar.google.com/citations?hl=pt-PT&user=fYCE5-sAAAAJ" target="_blank">João Paulo Fernandes</a> and <a href="https://scholar.google.com/citations?hl=pt-PT&user=x25BFgEAAAAJ" target="_blank">Rui Abreu</a> from FEUP, Portugal.

![Target Architectures](https://github.com/FilipaRamos/QuantumComputingDeepLearning/blob/main/resources/QC-archs.png)

### Introduction

This repository holds the supporting code for the Chapter "Quantum Computing for Deep Learning" considered for publication with the following abstract:

"Hybrid quantum-classical deep learning is an emerging area of research that combines the highly effective pattern recognition ability of deep learning with the possibility to generate complex distributions provided by a quantum computer. Further than this, the implementation of hybrid models can already be simplified by the availability of frameworks and tools designed specifically with that goal in mind. However, to enable awareness and provide wide adoption of quantum-classical deep learning, these tools need to reach a significant level of maturity. For this reason, we provide a study of two competing frameworks, _Qiskit_ and _Cirq_, and their respective tools for hybrid model development in the perspective of a newcomer, classical deep learning scientist. We find that _Qiskit_ already has several abstractions that enable fast and swift development of several architectures without the need for profound quantum knowledge. On the other hand, _Cirq_ provides a recent library, _Tensorflow Quantum_, that does not provide many abstractions for the tested architectures. We find, however, that _Cirq_ is well structured and thought-out, easing the introduction of more _Tensorflow_ proficient users in the hybrid quantum-classical world."

DISCLAIMER: All the developed code is merely ilustratory and serves the purpose of testing the interfaces provided by both cirq and qiskit instead of full correctness or efficiency.

### Dependencies

#### Qiskit

For the qiskit notebooks, the qiskit library must be installed, including the following components:

+ qiskit.aqua
+ qiskit.circuit
+ qiskit.visualization

The development versions were:

+ *qiskit-terra*: '0.17.3'
+ *qiskit-aer*: '0.8.2'
+ *qiskit-ignis*: '0.6.0'
+ *qiskit-ibmq-provider*: '0.13.1'
+ *qiskit-aqua*: '0.9.1'
+ *qiskit*: '0.26.0'

For the deep learning interface, [PyTorch](https://pytorch.org/) must be installed as well.

#### Cirq

For the cirq notebooks, the cirq and sympy libraries must be installed.

The development versions were:

+ *cirq*: '0.11.0'
+ *sympy*: '1.5' 

For the deep learning interface, [Tensorflow](https://www.tensorflow.org/), [Tensorflow Quantum](https://www.tensorflow.org/quantum) and [Tensorflow Gan](https://github.com/tensorflow/gan) must be installed as well.

--------------------------------------------------------------------

Standard dependencies are also needed, such as numpy, matplotlib and seaborn. The code was tested with Python 3.8.5, CUDA 11.1 and Ubuntu 20.04.

### Usage

As illustrated in the Figure, this code entails the development of an hybrid quantum-classical GAN and an hybrid convolutional neural network with quantum convolutional layers. The use of abstractions is high when possible in order to test their respective usability within the scope of the investigation.

Each component has its own folder where notebooks for both a qiskit and cirq approach are stored. In order to add the datasets, a root folder must be created with the name **datasets**.
