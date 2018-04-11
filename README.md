# Variational-Autoencoder-on-MNIST-dataset
Variational Autoencoder Using Keras on MNIST Images

Difference between autoencoder and variational autoencoder(In simple terms):
Instead of just learning a function representing the data ( a compressed representation) like autoencoders, variational autoencoders learn the parameters of a probability distribution representing the data. Since it learns to model the data, we can sample from the distribution and generate new input data samples. So it is a generative model like, for instance, GANs.



Summary(Structure) of variational autoencoder:
__________________________________________________________________________________
Layer (type)                    Output Shape         Param #     Connected to                     
==================================================================================================
input_3 (InputLayer)            (None, 784)          0                                            
__________________________________________________________________________________________________
dense_6 (Dense)                 (None, 256)          200960      input_3[0][0]                    
__________________________________________________________________________________________________
dense_7 (Dense)                 (None, 2)            514         dense_6[0][0]           z_mean ---]      
__________________________________________________________________________________________________ |probability distribution
dense_8 (Dense)                 (None, 2)            514         dense_6[0][0]        z_log_var ---]
__________________________________________________________________________________________________
lambda_2 (Lambda)               (None, 2)            0           dense_7[0][0]            
                                                                 dense_8[0][0]      
__________________________________________________________________________________________________
dense_9 (Dense)                 (None, 256)          768         lambda_2[0][0]                   
__________________________________________________________________________________________________
dense_10 (Dense)                (None, 784)          201488      dense_9[0][0]                    
==================================================================================================


Great resource for further understanding: 
Reference: https://towardsdatascience.com/intuitively-understanding-variational-autoencoders-1bfe67eb5daf
