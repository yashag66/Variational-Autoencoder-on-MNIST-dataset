# Variational-Autoencoder-on-MNIST-dataset
Variational Autoencoder Using Keras on MNIST Images

Difference between autoencoder and variational autoencoder(In simple terms):
Instead of just learning a function representing the data ( a compressed representation) like autoencoders, variational autoencoders learn the parameters of a probability distribution representing the data. Since it learns to model the data, we can sample from the distribution and generate new input data samples. So it is a generative model like, for instance, GANs.



Summary(Structure) of variational autoencoder:
_____________________________________________
Layer (type)                    Output Shape         
=============================================
input_3 (InputLayer)            (None, 784)                                              
_____________________________________________
dense_6 (Dense)                 (None, 256)                      
_____________________________________________
dense_7 (Dense)                 (None, 2)        
_____________________________________________ 
dense_8 (Dense)                 (None, 2)    
_____________________________________________
lambda_2 (Lambda)               (None, 2)           
                                                  
_____________________________________________
dense_9 (Dense)                 (None, 256)                     
_____________________________________________
dense_10 (Dense)                (None, 784)                      
=============================================

Great resource for further understanding: 
Reference: https://towardsdatascience.com/intuitively-understanding-variational-autoencoders-1bfe67eb5daf
