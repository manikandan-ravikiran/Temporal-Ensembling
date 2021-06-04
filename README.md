# Temporal Ensembling (PyTorch)

This is the code to reproduce temporal ensembling, which explains and gives implementation details on [Temporal Ensembling for Semi-Supervised Learning](https://arxiv.org/pdf/1610.02242.pdf) from ICLR 2017.

The current code extends to dataset of MNIST, KMNIST, EMNIST and Fashion-MNIST.
Detailed results are as shown in our paper [Investigating the Effect of Intraclass Variability in Temporal Ensembling](https://arxiv.org/pdf/2008.08956.pdf)

## Usage

#### Standard requirements

First, install the requirements in a virtual environment :

```sh
pip install -r requirements.txt
```

#### Regarding PyTorch and torchvision

Install PyTorch>=1.8 and torchvision as shown [here](http://pytorch.org/) according to your specs.

#### Training a model

You can launch a MNIST evaluation from the command line using :

```sh
python mnist_eval.py
```

You can tweak hyperparameters in the config.py file.

To test across different datasets please see utils.py and use modify prepare_dataset functions.

## Misc

This code is not a 100% faithful reproduction of the original paper and should not be used as such.

The Theano-based code released by the paper authors can be found [here](https://github.com/smlaine2/tempens).
 
## Acknowledgement
This repository would not be possible without works and codes of [Ferretj](https://github.com/ferretj/temporal-ensembling) and [smlaine2](https://github.com/smlaine2/tempens).
