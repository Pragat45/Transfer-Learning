TensorFlow Model Implementation 


First we need to input the words in the model as they are the labels and features to be trained. The words here are extracted from the tweets. After this we are embedding the layers of TensorFlow, as there would be some relative meaning for each layer. Limit of maximum words, input of previous layer and length of the words. LSTM (long short term memory) network saves the word and predicts the next word based on previous assumption. This layer is a sequence predictor of upcoming words. After this we introduce one more layer which is called as Dense Layer, in this all the outputs are getting reduced from the inputs from Fatten layer. Moving ahead, there is an Activation function which is used as a node in the end of all layers of neural network model. It is a crucial function as its decide which neuron should be passed for further evaluation and which neuron should get eliminated. The final layer we apply is a Dropout Layer in this we drop some neurons from the previous layer to avoid overfitting problems in the data. Overfitting might give better accuracy in the training phase, but would compromise in testing phase, so it’s better to avoid this and add a dropout layer. So, we designed a TensorFlow based model and all the layers are added and trained in this model. We are going to use two classes in this model for sentiment analysis, we set binary crossentropy. 
As an optimizer RMSprop() would be used as we need to reduces are losses due to learning rate.

Implementation of BERT Model. 

For this implementation I have created a new kernel and imported all the libraries which satisfy our conditions again. Moreover, I have installed wordcloud and spacy in the note- book, before performing all the steps. After this all the data pre-processing are performed and ensured it has evaluated smoothly. Once, all this done we define the train and test vali- dation samples. BertForSequenceClassification model is being defined and all the layer have been introduced and evaluated. Then the fine-tuned BERT is used to extract sentiment features from a tweet’s text. Tweets are not selected based on specific topics, and the features are extracted for all tweets related to a specific user regardless of the tweet’s topic [14]. After this the embedded layer, first transformer and output layer is created in the kernel. We have used AdamW as an optimizer for the training and testing of the data.
After this, I have also trained an image dataset regarding to human emotion and performed some pre analysis on it. It would be useful for us to see the sentiment of the tweets through the images of human emotion and give us the en- hanced efficiency of the results. This emotions here are divided into 7 different class. We have to import all the pre-requisite libraries in the notebook to perform this research. As the dataset we have it’s in image format so we cannot perform and train the dataset in the model, we need to first change the data into array form and then perform all the data processing steps. I performed DecicionTreeClassifier,
KNN Classifier and Random Forest Classifier on it, giving us the accuracy of it. After that, I have applied the Bert Transformer on the image dataset as same.
