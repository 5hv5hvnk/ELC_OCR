### ELC_OCR
ELC activity for July 2021, Optical character recognition of first 10 alphabets using sklearn and SVM and cross validation with kFold. <br>
## OCR <br>
Optical character recognition or optical character reader is the electronic or mechanical conversion of images of typed, handwritten or printed text into machine-encoded text, whether from a scanned document, a photo of a document, a scene-photo or from subtitle text superimposed on an image. <br>
## DATASET <br>
Dataset was provided by the University itself it had first 10 alphabets of English language labled by the directories in which they were present.<br>  <img width="691" alt="Screenshot 2021-08-07 at 1 58 48 PM" src="https://user-images.githubusercontent.com/17161999/128594115-cd42521a-3183-41a2-8bff-080cebb8543b.png">
## IMAGES <br>
Each image was in 32x32 size i.e. 1024 pixels when flattened. Since the images were at center itself and the data was clean there was no problem with flattening of images<br>
## CROSS VALIDATION <br>
Cross-validation, sometimes called rotation estimation or out-of-sample testing, is any of various similar model validation techniques for assessing how the results of a statistical analysis will generalize to an independent data set. <br>
## kFold <br>
Cross-validation is a resampling procedure used to evaluate machine learning models on a limited data sample.<br><br>

The procedure has a single parameter called k that refers to the number of groups that a given data sample is to be split into. As such, the procedure is often called k-fold cross-validation. When a specific value for k is chosen, it may be used in place of k in the reference to the model, such as k=10 becoming 10-fold cross-validation.<br><br>

Cross-validation is primarily used in applied machine learning to estimate the skill of a machine learning model on unseen data. That is, to use a limited sample in order to estimate how the model is expected to perform in general when used to make predictions on data not used during the training of the model.<br><br>

It is a popular method because it is simple to understand and because it generally results in a less biased or less optimistic estimate of the model skill than other methods, such as a simple train/test split.<br>
## GENERAL PROCEDURE <br>
1.Shuffle the dataset randomly.<br>
2.Split the dataset into k groups. <br>
3.For each unique group:<br>
(i)Take the group as a hold out or test data set <br>
(ii)Take the remaining groups as a training data set <br>
(iii)Fit a model on the training set and evaluate it on the test set<br>
(iv)Retain the evaluation score and discard the model<br>
4. Summarize the skill of the model using the sample of model evaluation scores
