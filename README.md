# Federated Learning

This repository explores the concept of Federated Learning and compares it with traditional machine learning techniques using the Flower framework. The main focus is on demonstrating the differences between these two approaches through practical implementations and analysis.

[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1bOIk6g8tfGBx0m1XAurTijnVFPbZYbEt?usp=sharing)

<img width="842" alt="Screenshot 2024-04-15 at 7 39 13 PM" src="https://github.com/mounishvatti/federated-learning/assets/76279858/346a51c9-e387-4570-8229-72aa779b8732">


## Table of Contents

- [Introduction](#introduction)
- [Comparison](#comparison)
- [Tech Stack](#tech-stack)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Federated Learning is a decentralized machine learning approach that enables model training across multiple devices or servers holding local data samples without exchanging them. This technique offers privacy benefits as it allows training models without centralizing data. 

Traditional machine learning techniques, on the other hand, typically involve centralizing data on a single server or location for training. This approach may raise privacy concerns and scalability issues, especially when dealing with large datasets or sensitive information.

In this repository, we delve into implementing Federated Learning using the Flower framework and compare its performance with traditional machine learning techniques. 

## Comparison

| Feature               | Traditional ML | Federated Learning |
|-----------------------|----------------|--------------------|
| Data Centralization   | Centralized    | Decentralized      |
| Privacy               | Concerns        | Enhanced           |
| Scalability          | Limited        | Improved           |
| Communication Overhead| High           | Low                |
| Data Dependency       | High           | Low                |

## Tech Stack

- Google Colab: A cloud-based platform for executing Python code with access to GPUs and TPUs.
- Python: Programming language used for implementing machine learning models and scripts.
- [Flower Framework](https://flower.ai): An open-source framework for federated learning.

## Our hybrid framework

![image](https://github.com/mounishvatti/FedCustom/assets/76279858/4bdb2a44-7c01-4961-9bba-03ebe48ce630)


## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to improve this project.

## Results

| Methodology           | Accuracy in (%) | Model used |
|-----------------------|----------------|-------------|
| Centralized Approach  | 98.5           | CNN                               |
| FedAvg                | 95.4           | Logistic Regression + 2 Layer CNN |
| FedCustom (Hypertuned)| 98.24          | Custom Hypertuned FedAvg          |

## License

This project is licensed under the [MIT License](LICENSE).

## References
- https://flower.ai/docs/framework/

```python  
@article{beutel2020flower,
  title={Flower: A Friendly Federated Learning Research Framework},
  author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and Qiu, Xinchi and Fernandez-Marques, Javier and Gao, Yan and Sani, Lorenzo and Kwing, Hei Li and Parcollet, Titouan and Gusmão, Pedro PB de and Lane, Nicholas D},
  journal={arXiv preprint arXiv:2007.14390},
  year={2020}
}
```
