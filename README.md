# Emotion Detection using Facial Expressions

## Paper
Submitted to FTNCT 2021.
Cite as:
"to be included"

## Datasets
### CK+

Emotion | #Images
--- | ---
Angry | 45
Contempt | 18
Disgust | 59
Fear | 25
Happy | 69
Sadness | 28
Surprise | 83

P. Lucey, J. F. Cohn, T. Kanade, J. Saragih, Z. Ambadar and I. Matthews.
"The Extended Cohn-Kanade Dataset (CK+): A complete dataset for action unit and emotion-specified expression," 2010 IEEE Computer Society Conference on Computer Vision and Pattern Recognition - Workshops, 2010, pp. 94-101.
doi: 10.1109/CVPRW.2010.5543262.

### JAFFE
Emotion | #Images
--- | ---
Angry | 30
Disgust | 29
Fear | 32
Happy | 30
Neutral | 31
Sadness | 30
Surprise | 30

Michael J. Lyons, Shigeru Akamatsu, Miyuki Kamachi, Jiro Gyoba.
Coding Facial Expressions with Gabor Wavelets, 3rd IEEE International Conference on Automatic Face and Gesture Recognition, pp. 200-205 (1998).
http://doi.org/10.1109/AFGR.1998.670949
Open access content available at: https://zenodo.org/record/3430156

## Proposed Methods
### PCA+SVM
Model available in pca_svm_model.ipynb
#### JAFFE
For JAFFE we used the first 130 principal components.
#### CK+
For CK+ we used the first 120 principal components.
### CNN
The same model was used on both the datasets. The trained model and prediction for CK+ and JAFFE datasets can be found in <tt>fer_cnn_ck+.ipynb<\tt> and fer_cnn_jaffe.ipynb respectively.
  
## Resuts
Method | Dataset | Accuracy(%)
--- | --- | ---
PCA+SVM | JAFFE | 95.35
PCA+SVM | CK+ | 81.81
CNN | JAFFE | 87.50
CNN | CK+ | 83.84
