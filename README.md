# mnist-autoencoder
Autoencoder for MNIST digits dataset

For this task I have build classifier with train/test accuracy ~0.99 (only for demonstration of the autoencoder's effect).
For the autoencoder, I have tried couple different architectures like:
-Flatten + Dense (1);
-Conv + Flatten + Dense (2);
-Conv + DeConv (3);
-Conv + DeConv with skip connections (4).

(1) made great on test images, but it could not deal with noise at all. This model only decreased accuracy of the classifier.
(2) showed better results than (1), but it still reduced the accuracy of the classifier.
(3) is the best architecture, after some hyperparameter-tuning it increased accuracy of the classifier from 0.70 to ~0.90.
(4) showed awesome results on train/test set, but it has a minor weakness - it does not clear noise at all)

All architectures can be found in 'task2.ipynb' notebook.
