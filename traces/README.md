# Traces
## Definition of traces
When we give the trained RNN an input(train or test), it is easy to get a sequence of state vectors, which we call a trace. The large size of inputs can produce a lot of traces.

Utilizing these traces, we can dipict the internal dynamics of a trained RNN.

## Details
> [S10,S11,S12,...,S1n-1]

> [S20,S21,S22,...,S2n-1]

>              ...

> [Sm0,Sm1,Sm2,...,Smn-1]

m is the number of samples, n is the number of timesteps/iterations of RNN.

## PCA Abstraction
### N to K
Due to the large size of n, We choose PCA to reduce the length of sequence from n to k
### Partition



