# MPC-RNN-Controller
This repository contains code for implementing a Recurrent Neural Network (RNN) Model Predictive Controller (MPC) for a 4-tank coupled system, as part of My Master's degree thesis project.

## Project Overview

The RNN MPC Controller project aims to develop a predictive control system using a recurrent neural network to predict control inputs required by a linear MPC for a 4-tank coupled system. The project leverages data extracted from a simulated plant implemented in Simulink to train the RNN.

## Project Details

- **Formula**: The control inputs are predicted using the formula `U(k+1) = f(U(k-5), ..., U(k), e(k-5), ..., e(k))`, where `U(k)` represents control inputs and `e(k)` represents error signals at time `k`.

- **Neural Network Architecture**: The RNN architecture consists of a single hidden layer with 10 neurons.

- **Training Parameters**:
  - Learning Rate: 0.001
  - Loss Function: Mean Square Error (MSE)
  - Optimizer: Stochastic Gradient Descent (SGD)
  - Number of Iterations: 3000

## Reference

This project is inspired by the paper "Recurrent Neural Network Based Predictive Control Applied to 4 Coupled-tank System" by Elmer Calle and José Oliden, presented at the 2021 IEEE International Conference on Automation/XXIV Congress of the Chilean Association of Automatic Control (ICA-ACCA). [Link to Paper](https://ieeexplore.ieee.org/document/9465192)



## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE.txt) file for details.
