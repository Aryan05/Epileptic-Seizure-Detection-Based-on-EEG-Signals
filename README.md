# Epillepsy-Detection-Using-EEG-signals

<p align="center">
    <img src="EEG Brain Module.jpg" alt="Image"/>
</p>


### Epilepsy
Epilepsy may occur as a result of a genetic disorder or an acquired brain injury, such as a trauma or stroke.
During a seizure, a person experiences abnormal behaviour, symptoms and sensations, sometimes including loss of consciousness. There are few symptoms between seizures.
Epilepsy is usually treated by medication and in some cases by surgery, devices or dietary changes.
### Seizure
A seizure is a sudden surge of electrical activity in the brain.
A seizure usually affects how a person appears or acts for a short time.
Many different things can occur during a seizure. Whatever the brain and body can do normally can also occur during a seizure.

## Detection 
If the prediction is 1 then the signal is epileptical otherwise the class is made 0 and signal is non epileptical.
Eplileptical - 1 Not Epileptical - 0

Model.ipynb :
First i visualised the data, for all the 5 classes. (i) Then defined a Recurrent Neural Network architecture , that has 2 layers of LSTMs
(ii)Then defined the optimiser as 'adam' and loss as 'binary_crossentropy' which gave better results than 'categorical_crossentropy'
(iii)Then I processed the data , by :
taking 1 in every 4 samples,then normalising the data and used the previously splitted test data as validation data.
(iv) Saved the model after training it for 50 epochs
(v) Plotted the rate at which the loss and accuracy are changing.
Product_Final.ipynb
The trained model is loaded then its used for prediction on the validation set. Now the prediction are changed for binary class, i.e., if the prediction is 1 then the signal is epileptical otherwise the class is made 0 and signal is non epileptical. Same procedure is followed for trainig set.
