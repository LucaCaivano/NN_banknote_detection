# NN_banknote_detection
The dataset contains some features extracted from the images of some banknotes and their classification. Data were extracted from images taken from genuine and forged banknote-like specimens. For digitization, an industrial camera usually used for print inspection was used. The final images have 400x400 pixels. Due to the object lens and to the distance from the investigated object, gray-scale pictures with a resolution of about 660 dpi were obtained. Wavelet Transform tool were used to extract features from the images. In particular:
1. The first column contains the variance of Wavelet Transformed image.
2. The second contains the skewness of Wavelet Transformed image.
3. The third contains the curtosis (a measure of the "tailedness" of the probability distribution of a real-valued random variable) of Wavelet Transformed image.
4. The fourth contains the entropy of the image.

In the notebook an artificial neural nerwork is trained: this simple neural network is capaple to correctly classify almost all samples in the validation set even with a small number of neurons and with only one hidden layer. Moreover with a deeper network all the samples (training, validation and test set in the real case scenario) are correctly classified. Those results are confirmed even by a more robust evaluation method like k-fold crossvalidation.
