# BYOL - TensorFlow 2

This is an unofficial implementation of ["Bootstrap Your Own Latent: A New Approach to Self-Supervised Learning"](https://arxiv.org/pdf/2006.07733.pdf) (BYOL). It is uses two networks namely online and target network,and target network parameter, will updated in exponential moving average fashion. It is similar to DQN.


## Architecture

<img src="https://i.imgur.com/PnwlSmw.png" width="90%">

## Dataset
For Pretraining the BYOL, [CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html) is used. Also the Linear Evaluation done using the [CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html).

- Pretraining dataset : [CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html).

- DownStream dataset : [CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html).


## References

* [Jean-Bastien Grill et al., "Bootstrap Your Own Latent: A New Approach to Self-Supervised Learning", 2020](https://arxiv.org/pdf/2006.07733.pdf)
- https://sthalles.github.io/keras-regularizer/ 
- https://github.com/garder14/byol-tensorflow2
- https://www.kaggle.com/code/shilashm/byol-tensorflow-2-0/edit