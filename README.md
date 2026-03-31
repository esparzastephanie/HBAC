                                          ## **Project Proposal**

In this project, we aim to analyze electroencephalography (EEG) brain signal data to determine
whether machine learning methods can accurately classify harmful brain activity, such as seizures. EEG
data represents electrical activity in the brain over time and is commonly used in medical diagnosis for
neurological conditions. However, interpreting EEG signals is extremely complex because the data is
highly variable, noisy, and often difficult to distinguish even for trained experts. In many cases, different
medical professionals may disagree on how to classify the same brain activity pattern, which highlights
both the difficulty and importance of this problem.

The dataset we will use is the HMS Harmful Brain Activity Classification dataset, which includes
EEG recordings along with expert-labeled brain activity patterns. These labels identify whether a segment
of EEG data corresponds to harmful activity such as seizures or normal brain function. Unlike typical
datasets organized in simple rows and columns, EEG data is time-series data, meaning it must first be
transformed before it can be used for machine learning. This adds an additional layer of complexity, as the
signals must be processed carefully to extract meaningful features.
The goal of this project is to determine whether we can take raw EEG signals, convert them into
useful features, and use those features to build models that can accurately classify harmful brain activity.
This problem is especially meaningful because early detection of seizures can significantly improve
patient outcomes, and a reliable model could support medical professionals in making faster and more
consistent decisions.

To approach this problem, we will begin by carefully exploring and preprocessing the dataset.
Since EEG signals are continuous and high-dimensional, we will segment them into smaller time
windows and extract relevant features from each segment. These features will include statistical measures
such as mean, variance, and standard deviation, as well as frequency-based characteristics obtained
through signal processing techniques. We will also normalize the data and address any missing or
inconsistent values. Because EEG data is often noisy, we will examine the presence of outliers and apply
methods such as Z-score or interquartile range analysis to understand their impact on the dataset.
After preprocessing, we will build and compare multiple machine learning models, including
Logistic Regression, K-Nearest Neighbors, Random Forest, and Support Vector Machines. Each of these
models offers different strengths in handling complex patterns and high-dimensional data. In addition to
these traditional approaches, we will also explore deep learning methods, such as neural networks, to
determine whether they can better capture the underlying structure of EEG signals. By comparing a range
of models, we aim to identify which techniques are most effective for this type of problem.

For evaluation, we will use several performance metrics to ensure a complete and realistic
assessment of our models. While accuracy and F1-score are commonly used, we recognize that the
F1-score alone may not be sufficient for this problem. EEG datasets are often imbalanced, with far fewer
instances of harmful brain activity compared to normal signals. Additionally, in a medical context, failing
to detect a seizure is significantly more serious than producing a false alarm. Because the F1-score treats
these errors equally, it may not fully reflect the real-world importance of model performance. Therefore,
we will also focus on metrics such as recall, precision, and area under the ROC and precision-recall
curves to experiment with the possibility of using these models to predict harmful activity at earlier
stages.

Finally, we will analyze and compare the results of all models, interpret their performance, and
discuss the limitations of our approach. We will consider how noise, variability, and uncertainty in EEG
data affect the results and explore how different modeling choices influence performance. Through this
project, we aim to gain a deeper understanding of how data mining techniques can be applied to complex,
real-world problems and how machine learning can potentially contribute to improving medical diagnosis
and decision-making.
