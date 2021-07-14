# Neural_Network_Charity_Analysis
## **Overview**
In this project, using Python TensorFlow library and Deep Learning Neural Network, we interpreted big datasets to assist AlphabetSoup, a non-profit foundation, with analyzing their fund applications. Within the project, the data was preprocessed, trained and optimized using Neural Network methods, activation functions and training models.
## **Results**

In the data preprocessing part of the project:
* `IS_SUCCESSFUL` column was used as the target;
* The categorical data columns `APPLICATION_TYPE`, `AFFILIATION`, `CLASSIFICATION`, `USE_CASE`, `ORGANIZATION`, `INCOME_AMT`, `SPECIAL_CONSIDERATIONS` were used as feature variables for the model;
* Moreover, two identification columns, `EIN` and `NAME` were dropped.

For compiling, training, and evaluating part of the model, different parameters were examined. By modifying the values, the model was trained and tested to get the best performance. However, the Deep Learning Neural Network modeling did not reach the satisfying accuracy which is %75.
* Different number of neurons selected during both the initial design and the optimization was different for each hidden layer. The model contains two hidden layers with 60 and 20 neutrons respectively for the first model initialization. In addition, multiple activation functions were applied. Best results were achieved when ReLU activation function was selected for the two hidden layers and Sigmoid activation function for the output. However, during the optimization process, other combinations such as ReLU and Tanh were examined as well. The results are displayed in the following screen shots of the code:
	* Initial model

	![initial_model.png](https://github.com/zkt2018/Neural_Network_Charity_Analysis/blob/main/Resources/initial_model.png)

	* First optimization

	![first_optimization.png](https://github.com/zkt2018/Neural_Network_Charity_Analysis/blob/main/Resources/first_optimization.png)
	
	* Second optimization

	![second_optimization.png](https://github.com/zkt2018/Neural_Network_Charity_Analysis/blob/main/Resources/second_optimization.png)

	* Third optimization

	![third_optimization.png](https://github.com/zkt2018/Neural_Network_Charity_Analysis/blob/main/Resources/third_optimization.png)

	* Setting Tanh activation function in the output layer
	
	![train_model_tanh_30_ep_results.png](https://github.com/zkt2018/Neural_Network_Charity_Analysis/blob/main/Resources/train_model_tanh_30_ep_results.png)
	
	* Increasing the number of epochs with the initial model neurons
	
	![initial_50_epochs.png](https://github.com/zkt2018/Neural_Network_Charity_Analysis/blob/main/Resources/initial_50_epochs.png)
* Using the Neural Network Model, we were not able to achieve the target model performance.
* To increase the performance, different number of neurons and epochs, classifications, and activation functions were put to the test.

## **Summary**
For this project, performance of Deep Learning Neural Network Model on the dataset did not achieve the target level and was overfitted. In such a case, we are required to select a different model that outperforms the Neural Network Model. A better option could be Random Forest Classification which has more robust algorithms against overfitting and is able to handle a great number of input variables.
