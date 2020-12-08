# smc_rnn
While deep learning has been widely used in recent years, many critical security issues start to emerge at the same time, which has to make people rethink how to ensure the security of deep neural networks, especially in safety-critical applications.

There have been a great amount of work in property specification and robustness verification on Feed-Forward Neural Networks. However, RNN has different behaviour and structure compared with common FNN, which makes the fact that property specification on common FNN can not transfer to RNN without change.

The verification of RNN is important but the work of it is rare. We try to extract **Probabilistic Abstract Model** from the original RNN. 

## Experiment Steps
1. Prepare the vehicle trajectory datasets
2. Design the input and output structure
3. Train the lstm model
4. Design the Probabilistic Abstract Model
5. Run lstm model to get trace
6. Extract probabilistic abstract model : MDP
7. Property definition
8. Run. Use smc to run probabilistic abstract model

## File & Folder Description
- *data/* trajectory datasets
- *train/* LSTM training process, get rnn model from data.
- *rnn_model/* RNN model, stored by .h5 file
- *traces/* traces run by rnn, stored by .txt file
- *abstract_model/* probabilistic abstract model, getting from traces
- *properties/* property definition
- *tests/* tests

## Usage of the project
### Installation
> https://github.com/MarkKobs/smc_rnn.git


## Thinkings
we found that the explanation of abstract model is highly related to the rnn_data input type, such as video,images,texts,etc. What drives transition is important, we choose the vehicle trajectory data as input, which belongs to the type of time series, unlike other series. 


## Contributors
