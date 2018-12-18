Implemented SVM algorithm on recipes dataset for predicting the new value as a cake/pastry recipe, plotted graphs to visualize the same.

Dataset used: Recipes of cakes and pastries dataset for classification of a new recipe as cake/pastry

Using the training dataset(Recipes.csv) containing various features like Refined Flour, Powdered Sugar, Egg etc. as inputs and Type as the class, to predict new recipe to be a cake/pastry.

Algorithm used: Support Vector Machines
This is a classification algorithm. Support Vector Machines are large margin machine learning algorithm. SVMs are binary classifiers, two classes are distinguished. They can be extended to classify more than two classes. In the binary case, samples belonging to one of the two classes are separated by a hyperplane.

Libraries:
Scikit learn for using the Support Vector Machines algorithm 
pandas for reading the data file to analyse the dataset
numpy used for computing purposes
matplotlib, seaborn for plotting and displays

Tools: Built using Jupiter Notebook which helps to define code as well as mention comments in the file itself.

Implementation: Step-by-step explained below
1.	Imported libraries to be used for coding, visuals and analysing the data
2.	Read the file recipes for the model to learn the categories of the recipes
3.	Selected features('Refined Flour', 'Powdered Sugar') as input and also set the target value('Type') field to be fed into the algorithm as input and class from the training dataset(Recipes.csv).
4.	The samples read from the file are plotted to display their positions with respect to the features selected (Powdered Sugar on y axis and Refined flour on x-axis).
5.	Using sklearn, SVM method is called and the features are fed into the instance created.
6.	The separating hyperplane is formed and plotted on the graph. The margins and the parallels of the hyperplane on the support vectors are formed.
7.	a function is defined to predict if a recipe is a cake or a pastry. The prediction values can be verified using the predict method on the svm instance.
8.	A new value is verified to be predicted as cake/recipe by passing the values into the function defined to predict the recipe which gives the classification of the new sample.
9.	The new sample is plotted on the graph to observe its position with respect to the fellow class samples. The process can be repeated to check the classification of the pastry recipe.
