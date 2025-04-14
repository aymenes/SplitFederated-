# SplitFed Learning with Quantum Neural Networks for Edge IoT Security

## Overview
This repository contains the implementation of a novel SplitFed learning approach combined with Quantum Neural Networks (QNNs) for enhancing security in Edge IoT environments. The work focuses on detecting cyber attacks in IoT networks using a hybrid classical-quantum machine learning framework that leverages federated learning principles while addressing data privacy concerns.

> **Note:** This project is based on code originally cloned from the following repository:  
> [https://github.com/chandra2thapa/SplitFed-When-Federated-Learning-Meets-Split-Learning](https://github.com/chandra2thapa/SplitFed-When-Federated-Learning-Meets-Split-Learning)  
> It provided the foundational architecture and implementation for the SplitFed learning framework used in this work.
## Key Features
- **SplitFed Learning Architecture**: Combines federated learning with split learning to enhance privacy and reduce communication overhead  
- **Quantum-Classical Hybrid Model**: Integrates quantum circuits with classical neural networks for improved attack detection  
- **Edge IoT Security**: Evaluated on real-world IoT network traffic data for attack classification  
- **Privacy-Preserving**: Client data never leaves local devices, only model updates are shared  
- **Communication Efficiency**: Reduced bandwidth requirements compared to standard federated learning  

## Dataset
The model is trained and evaluated on the `Cleaned_EdgeIoT.csv` dataset containing network traffic features with attack labels. Key features include:
- MQTT protocol attributes  
- TCP/IP header information  
- ICMP/UDP characteristics  
- Attack labels for binary classification  

## Model Architecture
The hybrid model consists of:

**Client-side classical neural network:**
- Input layer processing 8 network features  
- Hidden layers with LeakyReLU activation  

**Server-side quantum neural network:**
- 8-qubit quantum circuit with angle embedding  
- Strongly entangling layers for quantum feature extraction  
- Classical output layer with sigmoid activation  

## Results
- High accuracy in detecting IoT network attacks  
- Improved privacy through SplitFed learning framework  
- Efficient quantum-classical feature learning  
- Confusion matrix analysis showing strong performance  

## Requirements
- Python 3.7+  
- PyTorch  
- PennyLane (for quantum circuits)  
- Other standard ML libraries (NumPy, Pandas, etc.)  

## Citation
If you use this work in your research, please cite:

