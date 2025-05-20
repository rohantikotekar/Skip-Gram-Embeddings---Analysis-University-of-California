# Skip-Gram Embeddings from Scratch - Analysis: University of California

#### 1. Developed a Skip-Gram model from scratch using NumPy to generate 2-dimensional word embeddings for a custom vocabulary of 10 Californian universities
#### 2. Implemented a negative sampling technique with 2 negative samples per positive pair to improve computational efficiency of the Skip-Gram model by approximating the full softmax, reducing training time for word embedding generation.
#### 3. Engineered forward and backward propagation steps for the Skip-Gram model with negative sampling, enabling iterative optimization of word and context embedding matrices over 200 epochs to capture semantic relationships.
#### 4. Integrated pre-trained GloVe word embeddings (25-dimensional) from the gensim library to compute semantic similarity between sentences, quantitatively demonstrating higher similarity (e.g., 0.9083) for semantically related sentences compared to unrelated ones (e.g., 0.0573).
#### 5. Visualized word embeddings and cosine similarities between word vectors to qualitatively assess the learned semantic relationships and model convergence during training, achieving a visual clustering of related terms (e.g., SoCal universities).


