# Gradual Learning of Deep Recurrent Neuarl Networks

This repository is a self-contained code of the work in the Gradual Learning of Deep Recurrent Neural Networks.
The package contains a python implementation of the model as depicted in (https://arxiv.org/abs/1708.08863).

### Penn TreeBank
The file ptb_config.py contains all the configurations that were tested in the article. Choosing one of them is done by the model flag from the command line. 

The possible models names are:

+ GL - two-layered LSTM trained gradually.
+ LAD - two-layered LSTM trained with Layer-wise Adjusted Dropout.
+ GL_LAD - two-layered LSTM trained gradually with Layer-wise Adjusted Dropout.
+ Deep_GL_LAD - five-layered LSTM trained gradually with Layer-wise Adjusted Dropout.

To evaluate one of the configurations run the following:

`python ptb_model.py --model <model_name>`
