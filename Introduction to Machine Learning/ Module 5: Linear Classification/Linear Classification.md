Linear Classification
Overview
Now it's time to change directions and start focusing on some classification algorithms.  Recall that for classification we want to predict discrete categorical values. Similar to how we want to find a line-of-best-fit in regression, in classification, we want to find a line that best separates our data into different classes . See the image below for an example.

Classification Algorithm in Machine Learning - Javatpoint

For example, let's say we have two classes: A and B. Our goal is to predict a given data sample as either A or B then! This is an example of a binary classifier whose labels  would contain the following values 
 and our predictions would also attempt to predict those same label values 
. Here we can say class A corresponds to the label 0, 
, and class B corresponds to the label of 1, 
.

In this module, we'll look at applying a linear classification model to predict a binary labels of 
 using a model called the perceptron.  The class labels are now 
 as these are the specific values the perceptron algorithm requires to work.  Remember that in  linear regression, we make a prediction by taking the dot product of our weights 
 with our input features 
 as given below:

        
 .

However, recall, that taking the dot product outputs a continuous value and not a discrete binary value of 
. So how do we get a discrete value? This is where the idea of activation functions come into play. An activation function is a way of transforming or mapping a set of inputs to new outputs using a function. In particular, the perceptron uses a the sign activation function which squashes the normal continuous predictions value of  
 into either the values  
 based on the sign of the value.

Lastly, keep in mind that the perceptron algorithm is actually the core building block for neural networks, which we'll look at later in the semester.

Perp Material
Please read through the notes while also reviewing any of the required videos at the same time. The goal is to read a section of the notes and then watch the corresponding videos for that section (if there are any)! Videos will be posted on the following pages. Below and on the next page are links to the  notes, download it and open it with Jupyter Notebook.

Lecture_notes_linear_classification.ipynb Download Lecture_notes_linear_classification.ipynb 

Objectives
The objectives of this week's module are 

MO1. Learn how to use a linear model to classifies data into either one of two classes
MO2. Learn how to implement and train the perception algorithm
MO3. Practice the implementation of the perceptron and pocket algorithms. 
M04. Learn and implement various classification metrics.
