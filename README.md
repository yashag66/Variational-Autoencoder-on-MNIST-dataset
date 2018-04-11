# Variational-Autoencoder-on-MNIST-dataset
Variational Autoencoder Using Keras on MNIST Images

Difference between autoencoder and variational autoencoder(In simple terms):
Instead of just learning a function representing the data ( a compressed representation) like autoencoders, variational autoencoders learn the parameters of a probability distribution representing the data. Since it learns to model the data, we can sample from the distribution and generate new input data samples. So it is a generative model like, for instance, GANs.



Summary(Structure) of variational autoencoder:
_______________________
Layer (type)                        
=======================
input_3 (InputLayer)                                                     
_______________________

Encoder

dense_6 (Dense)                              
_______________________
dense_7 (Dense)                
_______________________
dense_8 (Dense)            
_______________________
lambda_2 (Lambda)                                            
_______________________


Decoder

dense_9 (Dense)                             
_______________________
dense_10 (Dense)                             
=======================

Great resource for further understanding: 
Reference: https://towardsdatascience.com/intuitively-understanding-variational-autoencoders-1bfe67eb5daf
