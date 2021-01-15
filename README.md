# Transfer-Learning-Projects
This repo will contain all the experiments/investigations of pre-trained models in the tensorflow hub.Transfer learning makes it possible to save training resources and to achieve good model generalization even when training on a small dataset.

To obtain question vectors, we have two alternatives that have been used for several text classification problems in NLP:

* word-based representations
* context-based representations

Word-based Representations
A word-based representation of a question combines word embeddings of the content words in the question. We can use the average of the word embeddings of content words in the question. Average of word embeddings have been used for different NLP tasks.
Examples of pre-trained embeddings include:
* Word2Vec: These are pre-trained embeddings of words learned from a large text corpora. Word2Vec has been pre-trained on a corpus of news articles with 300 million tokens, resulting in 300-dimensional vectors.
* GloVe: has been pre-trained on a corpus of tweets with 27 billion tokens, resulting in 200-dimensional vectors.

Context-based representations may use language models to generate vectors of sentences. So, instead of learning vectors for individual words in the sentence, they compute a vector for sentences on the whole, by taking into account the order of words and the set of co-occurring words.
Examples of deep contextualised vectors include:
* Embeddings from Language Models (ELMo): uses character-based word representations and bidirectional LSTMs. The pre-trained model computes a contextualised vector of 1024 dimensions. ELMo is available on Tensorflow Hub.
* Universal Sentence Encoder (USE): The encoder uses a Transformer architecture that uses attention mechanism to incorporate information about the order and the collection of words. The pre-trained model of USE that returns a vector of 512 dimensions is also available on Tensorflow Hub.
* Neural-Net Language Model (NNLM): The model simultaneously learns representations of words and probability functions for word sequences, allowing it to capture semantics of a sentence. We will use a pretrained models available on Tensorflow Hub, that are trained on the English Google News 200B corpus, and computes a vector of 128 dimensions for the larger model and 50 dimensions for the smaller model.

## Quora questions dataset
objectives:
* Use various pre-trained NLP text embedding models from TensorFlow Hub
* Perform transfer learning to fine-tune models on your own text data
* Visualize model performance metrics with TensorBoard

(Will be updated soon)

