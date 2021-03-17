# IBM Data Science Methodology
A Peer-graded Assignment: Final Assignment.


### Topic to apply data science methodology: Email.

This is due to my current role, in my organisation, which include managing the corporate email system. 


### 1. Business Understanding

XYZ Company uses an email form on their website to generate leads for marketing purposes. However, a lot of the emails received using the form turn out to be spam. This generated false leads and degraded the quality of data collected by the email system. The company wants to automatically filter out spams; in order to focus on actual leads.  

Thus, how do we automatically identify spam emails and move it to the spam folder? 


### 2. Analytic Approach

Our task here is to classifiy emails from the online form into spam or not spam!

Looking at some of the emails, we found that they all have the same subject, "feedback form". This is because they all came from the same online form. Consequently, we cannot determine whether a mail is spam or not using the email subject. 

However, the body of the emails revealed that most of the spam messages contain words like; Act Now, Buy, Click here, Order now, free, Unsubscribe, Visit our website, etc. It became apparent that if a mail contains one or more of the above words, it is most likely a spam email!

consequently we will employ decision-tree classification model; to determine if an email contains one or more of the spam email identifiers.


### 3. Data Requirements

We need to identify the data required to solve the problem.

Since the source of the emails is a web form with "feedback form" as subject; we will target all emails on the corparate server that bears "feedback form" as subject.


### 4. Data Collection

Having identified the required data, we will now begin to collect it. We can ask the company to provide the raw data from its server or give us access to the email address that receives the online form messages. We can also write a script to pull the emails from the sever based on subject. 


### 5. Data Understanding and Preparation

After we collect the data, we will begin Exploratory Data Analysis (EDA) - trying to understand whether the collected data can solve our problem. Here we try to generate relationships between the data collected; using charts and visualisations. For instance emails that contains one or more specific keywords, like Buy Now, Click here, Order now, free, Unsubscribe, Visit our website, etc.

Then we proceed to prepare the data. This is the data cleaning stage and it may take most of our time in the methodology stage. We perform a lot of operations on the data such as resolving the issue of missing data, making the data more readable, removing unrequired and duplicates data. 

We can now proceed with Modeling and evaluation.


### 6. Modeling and Evaluation

Here we will generate and evaluate an approprate model that can resolve the problem. Models are either descriptive or predictive. Since we want to accurately classify emails as spam or not spam, we will adopt a predictive model that will determine whether an email is spam or not and then effect the classification. We will try some classification algorithms and select the one that give us the best results.

Once we apply our model, we will evaluate it to see whether it solves our problem. We can keep improving our model until it is able to accurately predict spam emails and classify them as such.


### 7. Deployment

Once we feel that the model will work, we deploy it on a sample dataset or deploy for the client to test.    


### 8. Feedback

We gether feedbacks on the model, from the client or from our testing on the sample dataset. Based on the feedback, we may need to further refine the model, evaluate it and deploy it again. This process goes on and on until we have a final model.
