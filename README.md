#### Alzheimers Detection

- Total of 4 notebooks, each for different parts of the project
- Notebooks has different sections to organize codes

#### Notebooks 
+ Generate_Transcripts.ipynb
    + Contains the code used to generate text transcripts using HuBERT
	
+ Audio_Classification.ipynb
    + Install dependencies:
		Install openSMILE
		
	+ File preprocessing functions
		Change labels to integer

	+ Functions to extract features:
		Functions extract eGeMAPS features

	+ Extracting features:
		Extracting eGeMAPS features and saving to a csv file

	+ Load features and data preprocessing:
		Loading features from csv file and performing normalization

	+ Machine Learning classifiers:
		This section has functions to train different classifiers with 10 fold grid search cv 				(Decision Tree, Decision Tree Bagger, Random Forest, Random Forest Bagger, 					Support Vector, Logistic Regression)

	+ Neural Network:
		This section contains codes used to create the 4-layer network and do 10 fold grid 			search cv
	
+ Text_Classification.ipynb
    + Load text transcripts:
		Load the generated text transcripts
		
	+ Data Preprocessing:
		Text data preprocessing, to lowercase all text
		
	+ Doc2Vec:
		Contains codes used to perform grid search 10 fold cross validation for machine learning classifiers and a neural network using Doc2Vec embeddings
		
	+ BERT:
		Contains codes to load BERT model, extract embeddings, training and tuning of neural network model
	
+ Fusion_Mechanisms.ipynb
    + Load pre-trained text model:
		Loading the text data and some preprocessing, and loading the text model
		
    + Load pre-trained audio model:
		Loading audio data and audio model
		
	+ Get audio and text inputs:
		More data preprocessing and to get audio and text data inputs
		
	+ Bilinear Pooling:
		Has classes to create a bilinear pooling layer, function to create the bilinear pooling model, and training of the model with 10 fold cv
		
	+ Concatenation:
		Has function to create the model with concatenate layer and training of the model with 10 fold cv
