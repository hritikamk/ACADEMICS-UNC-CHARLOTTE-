[Resources] The Basic Steps of ML
Overview
Before we get into data preparation, we need to quickly review what steps and components are required for a typical ML project. Most ML practitioners will go through some combination of these 7 basic steps given below. As you are reading the below steps, keep in mind that you will most likely follow these, or similar, steps in all your ML projects!

In coming weeks, we'll be applying all these steps to different problem setups like regression and classification. If you don't quite understand all the terms being thrown around below, that's okay. The goal here is just to get the ideas and terms into your head.

Steps	Description
1. Setting up and formulating the problem	
Setting up and formulating the problem you want to tackle allows you to establish a solid direction for your project. Without doing this, you're bound to get lost! Setting up the problem typically entails thinking about and performing the following:

What is the problem and how will you frame your problem?
Think about which type of ML problem you fill be facing (supervised learning, unsupervised, reinforcement learning, ect)
Are there any comparable problems?
What are the current solutions?
Define how your solution will be used
Which performance measuresLinks to an external site. will be best to evaluate your problem?
Performance measures help measure how well your algorithm/model is learning to solve problem. Later, we'll look at loss functions which are a subgroup of performance measures we can differentiate and use for optimization/learning!
Are there any assumptions you have about your problem so far?
Verify these assumptions if possible
2. Gathering data	
While gathering data may sound pretty straight forward, it can honestly be a very tedious step, even more so if you have to collect your own data. Gathering data typically entails thinking about and performing the following:

List the data you need and how much
Find your data or collect it
Compare different potential datasets
Combine multiple datasets
Convert data to a usable format
Identify which feature will act as your labels/targetsLinks to an external site. if you are doing supervised learning.
Figure out how to store the data if you dataset is very large
3. Exploring and visualizing	
In order to gain more insights into our data and to formulate new assumptions about our problem, we need data exploration and visualization. This usually entails thinking about and performing the following:

Study data/feature characteristics
E.g., data types, missing values, noise, outliers, distribution of data
Identify the target feature(s)
Study correlations between features
E.g., Are there any features that correlate well with our target feature(s).
Explore any feature engineering/transformations methods you think might be useful during preprocessing
E.g., deminsionality reduction techniques
4. Preprocessing the data	
Preprocessing the data aims to clean that data such that it is ready to be fed to the model. This entails thinking about and performing the following:

Split data into train and test splits. Add an additional validation split if needed.
Clean data through removing outliers or filling/removing missing values
Feature engineeringLinks to an external site.
Feature selection
Aggregate features
Decompose features
Add new features
Discretize continuous features
Convert categorical variables or strings into numerical representations.
5. Training and exploring models	
This is the  "real" machine learning step.  Here you want to first select the model(s) or algorithm(s) that you think meet your initial assumption about the problem. Once this is done, you want to train each of these models using your training data. This process typically entails thinking about and performing the following:

Select a performance measure that will help evaluate your model(s)
Select any other metrics to help evaluate your model (e.g., accuracy)
Training model(s) using training data and basic/standard hyperparamters
Hyperparameters refers to the parameters that are used to configure the model (external from the parameters the model learns) while model parameters, or just referred to as parameters, refer to the weights the model learns (internal parameters the model learns) (useful post on the differencesLinks to an external site.).
Measure training performance using performance measures and compare algorithms
Analyze significant hyperparamters for each algorithm
If the models are performing poorly, go back to the steps 3 and 4 to further refine data preparation process and try to gain new insights through data exploration .
6. Evaluation, fine-tuning (hyperparamter tuning), and selecting the best model	
Once you think your model(s) are performing well on the training data, it's time to select the best performing model. Optionally, we can do additional things like fine-tuning the hyperparameters of our models to make sure we get the best results! This step typically entails thinking about and performing the following:

(Optional) Fine-tune hyperparamters by changing the values manually or by using automated algorithms like  nested K-fold cross-validationLinks to an external site.
This entails testing different parameters not only for the models you have selected but also for any data transformations that might have parameters  as well.
Use the validation split to compare model performance. Select the model with the highest performance.
You can use methods like K-fold cross-validationLinks to an external site. as well to compare model performance more thoroughly.
Try combing your best models to make a single prediction (referred to as ensemble learningLinks to an external site.)
7.  Prediction	
The final step is making predictions. This is where we finally use our test set (e.g., the unseen data) to see how well our selected model will perform on our simulated unseen data! This step typically entails thinking about and performing the followings:

Compute the prediction using the model you selected to be the best.
Measure the generalization errorLinks to an external site. (also called test error) using your selected performance measures.
Analyze how your model is performing on the unseen data (i.e., test set). Depending on what your findings are about how well your model is performing you may need to start all the way from step 1 again!
Let's take a look at a practical example of how these steps come together using an example. Checkout the below video or the blog post versionLinks to an external site. of the video if you prefer reading! While the steps given above won't match 1-1 with steps given in the below video, the steps in the below video are still relevant and are closely aligned!



Additional Resources (Optional)
Beginner Kaggle Data Science Project Walk-Through (Titanic)Links to an external site.
A longer example of all these steps given above.
If you have the Hands on Machine Learning by Geron check out Chapter 2 and Appendix B
