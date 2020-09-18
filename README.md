# Brain_Computer_Interface
BCI IV Dataset Competition

To perform exploratory data analysis in order to get a good feel of the data by
preparing the data for Data Mining, training at least two different classifiers, and assigning
class labels to the test data to indicate which activity the subject was performing while the
data were collected.

Other Collaborators: Dhanupan alias Boss, Izzat Nazmi at The University of Edinburgh, 2019

# Steps

1. Reproduce the results published in 1.(a)
a. Ferran Galan - University of Barcelona1
http://www.bbci.de/competition/iii/results/index.html
b. Method:
i. Use preprocessed data i.e. pre-computed features using canonical
variates transformation (CVT)
ii. Normalise data
iii. Distance Based Discriminant Analysis
iv. Mental Tasks Transitions Detector

2. Plausible other classifiers under consideration
a. Gaussian classifier2
b. Linear Discriminant Analysis

3. Comparing performance with the baseline approach. Using results in (a) to compare
models with simpler dimensionality reduction techniques with different feature
dimensions and multiple classifiers.

4. Once step (3) has been optimized, use the frames approach with a window size as
input to the model in order to realize the time-series data and again evaluate the
achieved accuracies.

# Discussion:

- Working with precomputed features data, since most of the leading existing models
use these features over the raw EEG data, and, moreover, the results are better3.

- The data consists of raw EEG readings from 3 different subjects randomly alternating
between 3 different physical tasks in 4 separate sessions. The tasks are namely
imagining left hand movement, imagining right hand movement, and generation of
words starting from the same letter.

- The EEG potential data are represented in power spectral density (PSD) every
62.5ms in 8 different standard position on the head called the centro-parietal
channels C3, Cz, C4, CP1, CP2, P3, Pz, and P4.

- The measurements were also done with frequency resolution of 2Hz from band 8 to
30 Hz (9 frequencies), and was estimated over the last second of data. As a result,
an EEG sample is a 96-dimensional vector.
