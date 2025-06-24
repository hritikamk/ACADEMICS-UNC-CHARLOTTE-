<img width="780" alt="Screenshot 2025-06-24 at 12 07 05 PM" src="https://github.com/user-attachments/assets/8a644b99-6138-4faf-bb28-6defa9ace52e" />


Overview
The last data preparation step, before we finally get to work with an actual model, is data preprocessing. Recall that this step involves everything from splitting our data to cleaning data to transforming our features. Data preprocessing is crucial as it helps us prepare our data for the model and helps us to confirm we have "good" data.  If you can't tell by now, data is the most important aspect of any machine learning problem. No matter how good your model is, if your data is garbage you will only get garbage output! Let's take a closer look at just a few frequently used preprocessing steps to make sure we using the best version of our data!

What are features?
Before we get started let's review what features and labels are. Recall, features refer the input data that a model takes in. For instance, if we were using housing data to predict the price of a house, some features that might be included in the data are floor space, rooms, lot size, ect. Features are often represented using the notation 
. Meanwhile, the targets/labels refer to values we want to predict from the dataset. In the case of the housing data, the labels would be the price of each house. Labels are often represented using the notation 
. See the below video to learn more!



Data Cleaning
Data cleaning is the basic processes of removing missing data, outliers, erroneous data, irrelevant data, and formatting our data. Without this step, most data would be no where close to be readying to be fed to a machine learning model. Check out the video below to learn more about data cleaning!



Feature Transformation/Engineering
The next important step of preprocessing is transforming our features. This entails things such as scaling our features or encoding categorical variables into numerical representations. There are much more ideas like decomposing features, combing features, and selecting important features. However, we don't have time to all these cover here and have instead elected to cover the most common methods. However, Jason Browniee has a very good and more in-depth post hereLinks to an external site. on feature engineering, I highly recommend you check out. Further, we'll try to introduce more feature engineering/transformation techniques as the semester goes on.

Feature Scaling
The goal of feature scaling is to allow all your features to be operating under the same data range or "scale". Most of the time, each feature in a dataset is operating using it's own dataset range. For instance, features with different units such as feet verses kilometers or minutes verse hours contain different scales. Differences in the scales across features often increases the difficulty for the machine learning model to learn properly.

As well soon see, if a feature has a large scale (meaning its values differ by hundreds or thousands of units) this can result in a model that learns large weights. Likewise, if a feature has a small scale the model will learn small weights. Thus, if we have a feature with a large scale and a small scale then the model might learn a large weight for the large scale and a small weight for the small scale. This is often an issue as weights are associated with the importance of a feature (at least for linear models).  Additionally, models with large weight values are often more unstable, meaning they may suffer from poor performance due to being very sensitive to changes in the weights. However, we'll discuss this more when we get to linear modeling!

By applying featuring scaling we constrain each features range to operate under the same scale. Now, how do we do this? Well, there are two popular methods: normalization and standardization. Normalization entails constraining your feature range between 0 and 1 while standardization entails constraining your feature ranges to have a mean of 0 and a standard deviation of 1. With that in mind, there are many different types of normalization and standardization methods. A popular normalization method is MinMax scaling while a popular standardization methods is Z-score standardization.  Let's take a look at these methods in the video(s) below.



The next question most people usually have is, "which one do I choose?" It turns out there actually isn't a straightforward answer as the answer largely depends on your data features, problem, and model you are using. One easy but naive way to to figure out which is better is to simply try a few and see how your model's performance changes (if any). Another rule of thumb is that most ML practitioners default to using standardization for most problems due to the Central Limit TheoremLinks to an external site.. This theorem basically says that most distributions tend towards normal distributions when said distributions follow certain assumptions.

Less naive choices require making some more assumptions. For instance, normalization is a good technique to use when you do not know the distribution of your data or when you know the distribution is not normal or GaussianLinks to an external site. (a bell curve). Likewise, standardization is a good choice when you can make the assumption that your data follows a Gaussian distribution.

Encoding Categorical Data
Another feature transformation we need to apply before our data can get to the model is transforming all categorical (i.e., textual) data into numerical data. Recall, machine learning models can only use numerical representations for learning! Let's take a quick look at the below video to learn about the two different types of encoding for ordinal and non-ordinal categorical data.



Data Splitting
Recall that we need to have separate datasets when performing machine learning. Thus, we usually have a training set for training our model and a testing set, which acts as unseen data, for testing our model. We usually split these datasets using the 80-20 split rule where 80% is used for training and 20% is used for testing. Only when we are finally ready to deploy our model, do we want to actually test our model on the test set using our performance measures. Recall, when we do evaluate our test set this is referred to as measuring the the generalization error or test error. Doing allows us to gauge how well our model performs on unseen data. However, what do we do if we want to fine tune our model before testing on the test set?

Further recall that we want to fine-tune our model on a validation set. The validation set is a small part of the training set that we set aside (maybe 20% more of the training data) and test on once our model is done training. Using our selected performance measures we can assess how well our model is doing and begin fine-tuning hyperparamters to try and improve the model. Once we finally finished fine-tuning, we can finally test our model on the test set.

Let's take a closer look at the concept data splitting in the video below. While watching, keep in mind that we will be using our validation and tests sets VERY similar to the way Kaggle does as discussed in the video for our mini projects!



Additional Resources (Optional)
Normalization for Neural NetworksLinks to an external site.
Ideas of normalization here still applies to most machine learning algorithms!
How to Use StandardScaler and MinMaxScaler Transforms in PythonLinks to an external site.
More useful information about scaling features.
