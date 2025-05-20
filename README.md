# Skip-Gram Embeddings from Scratch - Analysis: University of California

This project is a part of Advanced Natural Language Processing. As an introduction to word embeddings, Prof, Dong taught us this neural network arhitecture. Word embedding are dense vectors and they capuptre semantic and syntactic relationships. Given a target word, it takes into consideration the surrounding 

### Objective 
- Objective: Instead of predicting a target word from its context the Skip-Gram model aims to predict the surrounding context words given a target (center) word.

### Training data
- It trains on (target word, context word) pairs extracted from a corpus. For example, in the phrase "Rohan studies at UC Riverside," if "UC" is the target word, "at," "Riverside,",  are its context words, if the defined window size is 1. It predicts: The likelihood of the actual context word being a context word. 

### Architecture
Input Layer: it takes the one-hot encoded vector of the target word
Hidden layer (projection): It contains the word embeddings, it projects the one-hot input into a dense vector space of a predefined embedding dimension.
Output Layer: For each context word, it predicts its likelihood of being a context word for the given target word.
Loss Function (with Negative Sampling): To make training computationally efficient, especially with large vocabularies, the Skip-Gram model often uses negative sampling. The likelihood of several randomly chosen incorrect (negative) words not being context words.

1. Developed a Skip-Gram model from scratch using NumPy to generate 2-dimensional word embeddings for a custom vocabulary of 10 Californian universities
2. 2. Implemented a negative sampling technique with 2 negative samples per positive pair to improve computational efficiency of the Skip-Gram model by approximating the full softmax, reducing training time for word embedding generation.
3. Engineered forward and backward propagation steps for the Skip-Gram model with negative sampling, enabling iterative optimization of word and context embedding matrices over 200 epochs to capture semantic relationships.
4. Integrated pre-trained GloVe word embeddings (25-dimensional) from the gensim library to compute semantic similarity between sentences, quantitatively demonstrating higher similarity (e.g., 0.9083) for semantically related sentences compared to unrelated ones (e.g., 0.0573).
5. Visualized word embeddings and cosine similarities between word vectors to qualitatively assess the learned semantic relationships and model convergence during training, achieving a visual clustering of related terms (e.g., SoCal universities).


