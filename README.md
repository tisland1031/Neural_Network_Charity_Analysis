# Neural Network Charity Analysis
## Overview of Analysis
The project entailed performing data analysis for Alphabet Soup, a non-profit organization that funded 34,000 organizations over the years. Unfortunately, not all organizations have spent money on their cause, and Alphabet Soup requests a deeper dive into their funded charities.   

### Purpose
This data analysis aims to predict whether applicants will be successful if funded by Alphabet Soup. The study will be using deep learning neural network with a TensorFlow parameter to classify the success of charitable donations.

## Results
### Data Preprocessing
- The following are considered the targets for the model:

![target_1](https://user-images.githubusercontent.com/96746207/176256791-8a6bde91-22b4-42b8-af70-bc7ba84ec7db.png)

- The following are considered to be the features of the model:
![feature_2](https://user-images.githubusercontent.com/96746207/176256359-9298b279-0eb3-445e-9d39-afc4297a6a20.png)
- The following variables are neither targets nor features and should be removed from the input data:

![drop_3](https://user-images.githubusercontent.com/96746207/176257780-883f23ec-973f-466a-936d-1beb52bdf14a.png)
	
### Compiling, Training, and Evaluating the Model

### Initial Model
- Neural network model had a performance rate (.725) 73%.
- 42 input features into three processing layers:
  - First layer: 80 neurons
  - Second layer: 30 neurons
  - Third layer: 1 neuron

![Dev_1](https://user-images.githubusercontent.com/96746207/176256049-f6366a1d-3459-4a2c-ae8a-87c4172bdc04.png)
![dev_2](https://user-images.githubusercontent.com/96746207/176256064-7e00c6fb-8f6c-4f3c-9a76-a17bb6e8bc59.png)

### Automated Optimizer
- In this analysis, many different neurons, layers, and activation functions were not needed; instead, the automated optimizer did the work. Autoencoder allowed for one attempt to find the best model hyperparameters.
- 42 input features into six processing layers with varying neurons in each layer.

Code listed below:

![auto_1](https://user-images.githubusercontent.com/96746207/176256072-cb40b6af-6342-4b3b-a040-22e804ceb50e.png)
![Auto_3](https://user-images.githubusercontent.com/96746207/176256159-ba45dcce-266b-4c60-84fb-68f8f319c762.png)

- Target model performance of 75% or above wasn’t reached. It barely increases the performance accuracy, .0726.


![auto_2](https://user-images.githubusercontent.com/96746207/176256112-1373d663-f314-4705-9d4d-ee862afcc4e5.png)


## Summary
-	The starting attempt for the neural network model was 73% accuracy. After applying the automated optimizer, the maximum accuracy achieved was 73%. The automated optimizer performed a few decimals higher than the original model. The target accuracy of 75% or higher wasn’t met by utilizing a neural network model. 

### Recommendation:
- Recommend using a supervised machine learning random forest algorithm for this analysis. 
- Decision trees will generate the classification problem into smaller models for a more accurate model by combing many trees into one ensemble model. Due to this, random forests are less prone to overfitting. 
- Neural network can work with many data types. However, a random forest can only work with tabular data. This data type is tabular data.
- Random forest is more robust due to the multiple decision trees, and missing values don’t cause an issue.    
  
	
 
