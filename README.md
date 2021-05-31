# Classify Applauses

Classify applauses and cheering apart from classical music.

The model trained here would be embedded in a client side application which filters applauses at runtime.

# Installation 

Use Anaconda.

```
$ conda install tensorflow-gpu 
```

Then run the Jupyter notebooks.

# Data 

Not included in this repository. It is possible to easily substitute with customized data. Contact the author for data.

# Notebooks

- Preprocessing: converts .wav into .tfrecord
- Spectrogram: performs STFT on the sequential audio data to obtain 2 dimensional spectrograms
- Training: trains a CNN on the spectrograms
- Testing: evaluates precision/recall on test set and tests model on noisy data not in the training set

# Model

- `model`: last Keras checkpoint
- `classify_applauses_model.h5`: Keras saved model (if saved correctly, same as above)
- `tfjs_model`: TF Layers model exported for tfjs use

