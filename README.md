# BYOL - TensorFlow 2

This is an unofficial implementation of ["Bootstrap Your Own Latent: A New Approach to Self-Supervised Learning"](https://arxiv.org/pdf/2006.07733.pdf) (BYOL). It is uses two networks namely online and target network,and target network parameter, will updated in exponential moving average fashion. It is similar to DQN.


## Architecture

<img src="data:image/png;base64,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" width="90%">

## Dataset
For Pretraining the BYOL, [CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html) is used. Also the Linear Evaluation done using the [CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html).

- Pretraining dataset : [CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html).

- DownStream dataset : [CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html).


## References

* [Jean-Bastien Grill et al., "Bootstrap Your Own Latent: A New Approach to Self-Supervised Learning", 2020](https://arxiv.org/pdf/2006.07733.pdf)
- https://sthalles.github.io/keras-regularizer/ 
- https://github.com/garder14/byol-tensorflow2
- https://www.kaggle.com/code/shilashm/byol-tensorflow-2-0/edit