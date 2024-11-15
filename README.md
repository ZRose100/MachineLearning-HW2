# Notes about code

Both ffnn.py and rnn.py have been updated with the correct parts filled in in the forward pass of each.

Both can be run on a terminal (as is expected), but both also include a line in the args function in the if name... section that allow the code to be run in Google Colab or Jupyter Notebook, as this was the way I found most useful for editing these files. This line has been commented out and should not affect terminal execution, but can be uncommented to allow execution in Colab if preferred.

In the rnn.py file, summing the outputs of the rnn function seemed unnecessary, as focusing on the final hidden layer was all that mattered for my architecture. Thus, this part has been left blank but should not affect the execution.

Thank you!

---

One example on running the code:

**FFNN**

``python ffnn.py --hidden_dim 10 --epochs 1 ``
``--train_data ./training.json --val_data ./validation.json``


**RNN**

``python rnn.py --hidden_dim 32 --epochs 10 ``
``--train_data training.json --val_data validation.json``

