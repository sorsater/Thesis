# Thesis
My Master's thesis.


## Abstract
In recent years, development of Convolutional Neural Networks has enabled high performing semantic segmentation models. Generally, these deep learning based segmentation methods require a large amount of annotated data. Acquiring such annotated data for semantic segmentation is a tedious and expensive task.

Within machine learning, active learning involves in the selection of new data in order to limit the usage of annotated data. In active learning, the model is trained for several iterations and additional samples are selected that the model is uncertain of. The model is then retrained on additional samples and the process is repeated again. In this thesis, an active learning framework has been applied to road segmentation which is semantic segmentation of objects related to road scenes.

The uncertainty in the samples is estimated with Monte Carlo dropout. In Monte Carlo dropout, several dropout masks are applied to the model and the variance is captured, working as an estimate of the model’s uncertainty. Other metrics to rank the uncertainty evaluated in this work are: a baseline method that selects samples randomly, the entropy in the default predictions and three additional variations/extensions of Monte Carlo dropout.

Both the active learning framework and uncertainty estimation are implemented in the thesis. Monte Carlo dropout performs slightly better than the baseline in 3 out of 4 metrics. Entropy outperforms all other implemented methods in all metrics. The three additional methods do not perform better than Monte Carlo dropout.

An analysis of what kind of uncertainty Monte Carlo dropout capture is performed together with a comparison of the samples selected by baseline and Monte Carlo dropout. Future development and possible improvements are also discussed.
