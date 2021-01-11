We will need to have these packages installed:

* tensorflow==2.3.1
* nltk==3.5
* colorama==0.4.3
* numpy==1.18.5
* scikit_learn==0.23.2


Firstly, we need to define messages which are asked by user and their intentions, along with some responses.

## The next step is to import the libraries.

* Numpy for data manipulation
* Keras for importing models, tokenizers and encoders
* Sequential is a class which will built a neural network model.
* Dense, Embedding, GlobalAveragePooling1D are the types of layers that will be used in the model.
* Tokenizer is used for text preprocessing like creating the vocabulary index based on word frequency, taking each word in the text and replacing it with its corresponding integer value from the dictionary
* Pad_sequences is used to ensure that all sequences in a list have the same length
* LabelEncoder can be used to normalize labels. It can also be used to transform non-numerical labels to numerical labels.

Then we will read and process the JSON file.

We will then vectorize the data using the tokenizer.

Then we will train and create a neural network to train our chatbot.

We will also save the neural network, encoder and tokenizer.

When the message from the user will be received, the chatbot will compute the similarity between the sequence of the new text and the training data.
Taking into account the trust scores obtained for each category, it categorizes the user’s message according to an intention with the highest trust score.
