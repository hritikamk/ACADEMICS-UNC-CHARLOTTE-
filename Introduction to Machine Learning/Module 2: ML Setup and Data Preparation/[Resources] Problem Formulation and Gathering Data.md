[Resources] Problem Formulation and Gathering Data
Overview
Recall that the first thing we need to do before we work with any data or machine learning models is to first setup and  formulate the problem we are trying to solve. Once we have formulated our problem then begins our search for data and in some cases the quest to capture data.

Setting up and Formulating the Problem
With these ideas in mind, let's first take a closer look at how to formulate our problem. This readingLinks to an external site. (sorry there aren't any great videos on this topic) provides a very concise breakdown about how to formulate an ML problem. There are typically three questions you need to answer:

Step 1: What is the problem? 
Describe the problem informally and formally if needed. Start listing assumptions you are making and thinking about similar problems.
Step 2: Why does the problem need to be solved? 
List your motivation for solving the problem, the benefits a solution provides and how the solution will be used (in research oriented fields how the solution might be used isn't always clear and can even be unknown).
Step 3: How would I solve the problem? 
Describe how the problem would be solved (think through each step of the problem almost like pseudo code) to help explore what problems you might run into and help think about potential domain knowledge .
Gathering Data
With the problem formulated, the next step is to begin the search or the process of collecting data. Since collecting data can very time consuming and domain specific we'll leave this for another time. However, there are loads of existing datasets out there. Before you ever collect any data take the time to investigate and see if someone else has already collect the data your interested in! Trust me, using someone else's data can be a headache but it isn't nearly as time consuming as collecting your own data!

So where do we find data? Well, the first places to check are some of the popular machine learning data repositories such as

UC Irvine Machine Learning RepositoryLinks to an external site.
This is classical machine learning data repository and great for finding classical datasets.
Kaggle datasetsLinks to an external site.
Kaggle has only recently become very popular and holds a wide variety of popular and niche datasets. Additionally, Kaggle has a wide assortment of ML challenges and Jupyter Notebooks for data exploration and model training!
Amazon's AWS datasetsLinks to an external site.
AWS datastes is a great repo to find datsets pair with research papers that have used said datasets.
Wikipedia datasetsLinks to an external site.
If you are looking for a popular dataset in a particular field this is a great resource.
Still can't find a particular data? The next best thing is to start scavenging the internet or referring to research papers to see if someone else is doing research surrounding a similar problem and has an open sourced dataset. Instead of using Google search try some of the following data and paper search engines.

Google Dataset SearchLinks to an external site.
If you can't find any datasets on popular sites then give Google's specific dataset search engine a go!
re3dataLinks to an external site.
Searches research papers, institutions, and websites for related datasets. Can be a little confusing to use.
Google ScholarLinks to an external site.
While not a dataset search engine, it is a search engine for finding research papers. Finding a paper related to your problem could mean said paper also has open source data you can use!
Once you have found your data, the next step is loading your data. In this weeks lab, we'll take a closer look at doing just that using the Pandas library/module.

Additional Resources (Optional)
Kaggle CompetitionsLinks to an external site.
These competitions usually offer real cash money!
5 different ways to load dataLinks to an external site.
For those interested in getting a sneak peak into how we might load data using Python see this link!
