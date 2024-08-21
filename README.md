# Facial Emotion Depth Index

## Project Overview

In this research endeavor, we
embark on a fresh approach aimed at discerning emotions and
gauging their intensity through the utilization of an innovative
emotion depth index. By forecasting continuous values that
mirror the magnitude of emotion, this methodology affords a
heightened level of precision and a more intricate
comprehension of an individual’s emotional state. Furthermore,
this study delves into the potential real-world applications of this
technology, spanning from psychological counseling and
customer service to market research.

## Prerequisites

Before running the project, ensure you have the following installed:

- Python 3.8+
- Jupyter Notebook
- NumPy
- OpenCV
- TensorFlow
- scikit-learn
- Matplotlib

## Methodology

As the dataset is labeled by human raters, there are bound
to be many mis-classed images, and some images may have
multiple emotions. To give a better idea of the
emotion of the person in the image, we implemented an
emotion depth index, which gives a score for each of the
seven classes of emotions for each image.

To evaluate our model's accuracy, we extracted the
probabilities of each emotion class for each image and
provided a score for each of the seven emotions. First, we
obtained the filenames of the validation data. Then, we
passed the obtained predictions through our model. After
which, we used NumPy to obtain the classes with the highest
probability
Next, we created a dataframe to store the filename,
predicted class, true class, and probability scores for each
class. We then calculated the score for each emotion class by
looping through the predictions and appending the
probability scores for each class to a list. Finally, we rounded
the scores to two decimal places and saved them in the
dataframe for each emotion class

## Results and Conclusion

In this study, we introduced a groundbreaking
methodology termed the emotion depth index for discerning
emotions in facial images, departing from conventional
emotion classification methods that typically framed the issue
as a singular classification task. The approach conferred
several notable advantages, facilitating the provision of a
continuous metric for emotional intensity and demonstrating
efficacy in discerning subtle emotional expressions that
challenged traditional classification methodologies.

The model utilized a CNN to assimilate features from
facial images and predict associated emotion labels. Evaluation
of the methodology on the FER 2013 dataset revealed
commendable accuracy in emotion detection. Notably, the
model has a validation accuracy of 65.99%, with a loss of 0.96.
These outcomes underscored the viability of the proposed
methodology for emotion detection in facial images.

A distinctive attribute of the model was its capacity to
provide a continuous measure of emotional depth, rendering it
particularly advantageous for applications necessitating a
nuanced comprehension of human emotions, such as human-computer
interaction and psychological studies.

In conclusion, the proposed methodology offered a
departure from conventional single-class classification
paradigms in facial emotion recognition. Acknowledging the
imperatives for refinement in accuracy and robustness, we
posit the approach as a noteworthy advancement within this
domain, anticipating further refinement through subsequent
research.
