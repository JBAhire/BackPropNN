# BackPropNN


# Install

## Stable
```julia
Pkg.add("BackpropNeuralNet")
```

## Source

```julia
Pkg.clone(https://github.com/JBAhire/BackPropNN)
```

# Usage

To initialize a network of 2 inputs, 1 hidden layer with 3 neurons, and 2 outputs:

```julia
using BackpropNeuralNet

net = init_network([2, 3, 2])

# To train the network use the form `train(network, input, output)`:
train(net, [0.15, 0.7],[0.1, 0.9])

# To evaluate an input use the form `net_eval(network, inputs)`
net_eval(net, [0.15, 0.7])
```

# History

This is a Julia implementation of a neural network based on Sergio Fierens [ruby version](https://github.com/SergioFierens/ai4r).

