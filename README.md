# Notes about code

Both ffnn.py and rnn.py have been updated with the correct parts filled in in the forward pass of each.

Both can be run on a terminal (as is expected), but both also include a line in the args function in the if name... section that allow the code to be run in Google Colab or Jupyter Notebook, as this was the way I found most useful for editing these files. This line has been commented out and should not affect terminal execution, but can be uncommented to allow execution in Colab if preferred. Note that this repository must be linked to Colab and the word_embedding file must be uploaded directly onto Colab if run this way.

In the rnn.py file, summing the outputs of the rnn function seemed unnecessary, as focusing on the final hidden layer was all that mattered for my architecture. Thus, this part has been left blank but should not affect the execution.

The word_embedding.pkl file was too large to be uploaded directly to this repository, so the file has been uploaded to my personal Drive and the link to access this file is here: https://drive.google.com/file/d/1Wca7kbLNLS6dtmvQyXIauCRKSBkuS1pU/view?usp=sharing
. I assume the TA already has this file on his computer, but I figured it would still be good to add the file regardless.

Thank you!

---

One example on running the code:

**FFNN**

``python ffnn.py --hidden_dim 10 --epochs 1 ``
``--train_data ./training.json --val_data ./validation.json``


**RNN**

``python rnn.py --hidden_dim 32 --epochs 10 ``
``--train_data training.json --val_data validation.json``

