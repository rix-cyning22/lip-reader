A Jupyter notebook for creating a model that reads lip motion and generates caption.

Trained the data on the LipNet dataset.
Used a cascade classifier to extract the mouth in every frame.
The model used 3D convolutional neural networks to encode each frame.
Used bidirectional LSTM to generated the tokens.
Used characters as embedding.

CTC is used as a loss function.

Future Work:

1. Use better mouth extraction models. There are better classifiers than CascadeClassifiers
2. Using attention models for token generation. LSTM models are good to an extent. However, it has the following problems:
   a. It may not capture the context in long sentences.
   b. It is difficult to parallelize and is slow.
