Repository is about:

Experiment with various types of recurrent neural networks (RNNs) in PyTorch. 
PyTorch is a popular alternative to Keras and TensorFlow that has become quite popular in recent years.
It is more intuitive than TensorFlow, while giving the programmer greater control than Keras. Preliminary steps:

Familiarize yourself with PyTorch by going through the tutorial Get familiar with PyTorch: a 60 minute blitz
Download and install PyTorch on a machine with a GPU or use Google's Colaboratory environment, which allows you to run PyTorch code on a GPU in the cloud.
Colab already has PyTorch pre-installed. The first two parts below do not require a GPU, but the third part can be accelerated with a GPU. 
To enable GPU acceleration, click on "edit", then "notebook settings" and select "GPU" for hardware acceleration. 
It is also possible to select "TPU", but the PyTorch code provided with this assignment will need to be modified in a non-trivial way to take advantage of TPU acceleration.

File description:

1) File "classification" is used to classify sentences into 18 languages using LSTM, RNN and GRUs.

Compare the accuracy of the encoder when varying the type of hidden units: linear units, gated recurrent units (GRUs) and long short term memory (LSTM) units. 
Two graphs that each contain 3 curves (linear hidden units, GRUs and LSTM units). The first graph displays the training loss and the second graph displays the validation loss. In both graphs, the y-axis is the negative log likelihood and the x-axis is the number of thousands of iterations.
For each type of hidden unit, print the test loss and the test confusion matrix of the model that achieved the best validation loss among all iterations (i.e., one best test loss and test confusion matrix per type of hidden unit).
Explanation of the results (i.e., why some hidden units perform better or worse than other units).

2) File "translation" is used to translate French to English and vice versa.

Compare the accuracy of the seq2seq model with and without attention. 
Two graphs that each contain 2 curves (with attention and without attention). The first graph displays the training loss and the second graph displays the validation loss. In both graphs, the y-axis is the negative log likelihood and the x-axis is the number of thousands of iterations.
For each architecture, print the test loss of the model that achieved the best validation loss among all iterations (i.e., one best test loss per architecture).
Explanation of the results (i.e., how does attention affects the results).
