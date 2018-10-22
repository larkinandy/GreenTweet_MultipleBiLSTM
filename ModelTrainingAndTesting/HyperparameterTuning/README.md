# GreenTweet_MultivariateBiLSTM: Model Training and Testing : Hyperparameter Tuning
text and metadata collection from twitter

**Author:** [Andrew Larkin](http://www.linkedin.com/in/andrew-larkin-525ba3b5/) <br>
**Affiliation:** [Oregon State University, College of Public Health and Human Sciences](http://health.oregonstate.edu/) <br>
**Date Created:** October 15th, 2018 <br>

**TODO:**<br>
[ ] insert link to manuscript once published

### Summary ###
Hyperparameter tuning methodology and results are described here.  This secction if comprised of two documents:

**Readme.md** - describes the tuning methodology, including hyperparameters to tune, range of hyperparameter values, evaluation metrics, and selection strategy <br>
**HParramTuning.py** - Notebook with tf code to tune hyperparams and records results <br>
**HParamTuning.xls** - Excel tables with select tables and graphs from hyperparamter tuning


**Note:** The material here is supplementary rather than superlative of published methods and results (insert link once published).  Please see the published materials for a comprehensive description of the model training and testing process.

### Model hyperparameters ###
Model hyperparameters are shown below in Table 1.  For tunable hyperparameters, the set of candidate parameter values are listed as well.  Tuning the learning rate or "alpha" hyperparameter consisted of two stages, where the first stage consisted of a "coarse search" along 0.01 unit changes in alpha, followed by a more fine search of 0.001 units between the best performing subset alpha candidate values.


Symbol | Description | Tuning? | Test Value Set | 
------------ | ------------- | ------------- | ------------- 
α | learning rate | Yes | {1e-4, 5e-4, 1e-3, 5e-3, 0.01, 0.05, 0.1}* |
τ |  # hidden layers** | Yes | {1,2,3} |
ι | # hidden nodes / layer** | Yes | {7, 16, 32, 64, 128} | 
m | minibatch size | Yes | {64, 128, 256, 512} | 
e | # epochs | Yes | {1000,5000,10000,25000, 50000, 100000, 250000} |
λ | L2 regularization parameter*** | Yes | {1e-4, 5e-4, 1e-3, 5e-3, 0.01, 0.05, 0.1, 0.5}* |
g | activation function**** | Yes | {tanh, relu, leaky relu } |
c | # outcomes | Yes | {1,2,3,4,5,6,7} |
β1 | momentum term of ADAM optimizer | No | 0.9 |
β2 | RMSProp term of ADAM optimizer | No | 0.999 |
ε | small constant of ADAM optimizer | No |1e-8 |
v | # biLSTMs | No | # words in longest Tweet + 1 |


**Table 1.** Hyperparameters in biLSTM model. * Parameters are part of a coarse-to-fine search strategy.  Only coarse search parameters are shown. ** Not including / not applicable to the bidirectional LSTM units.  *** Number of λ parameters to tune is dependent on τ. **** For hidden units only. Sigmoid is the activation function for all output units 

### Evaluation Metrics ###
Two evaluation metrics were used to tune hyperparameters:
- ** Cost function J ** - the unweighted arithmetic mean cost function for all c outcomes in a given candidate model
