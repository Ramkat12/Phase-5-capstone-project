# Phase-5-capstone-project
# 1 ) INTRODUCTION 
This is the phase 5 capstone project repository.In this repository , we will  be performing sentiment analysis on sentiments by Redda.it users.The datset is sourced from Kaggle.This project was done by a team of five people , namely : </br>
1) Anthony Ngatia.</br>
2) Elsie Nduta.</br>
3) Jessyca Aperi.</br>
4) Joy Kipkemboi.</br>
5) Naomi Rotich.</br>
# 2) BUSSINESS UNDERSTANDING.
## 2.1) Business overview.
Getting feedback from application users is a crucial aspect of growth as it gives a deeper understanding of user sentiment, improves content moderation, and informs product and service improvements. Our project utilizes the Google AI GoEmotions dataset to expand emotion classification datasets, improving chatbot sensitivity, online behavior detection, and customer support. By training neural networks and SVM models to analyze text tonality, we advance emotion analysis in NLP, benefiting stakeholders such as chatbot system providers, online platforms, and customer support departments. Our project's enhanced emotion analysis addresses this real-world problem of limited sensitivity and understanding, leading to more empathetic interactions, improved content moderation, and optimized customer support, ultimately enhancing user experiences.
## 2.2) Business objectives.
Expand emotion classification datasets by training models to analyze text tonality using the Google AI GoEmotions dataset.</br>
**Specific Objectives**</br>
a) Develop a model to classify text data into different sentiment categories, such as positive, negative, neutral, or mixed sentiments.</br>
b) To establish the most appropriate model amongst the ones chosen, to accurately predict sentiments.</br>
c) Improve customer support by recognizing and addressing user emotions in textual communication.</br>
**Business Success Criteria**
To make accurate predictions on sentiments from the text data.
# 3 ) DATA UNDERSTANDING
The dataset was sourced from [Kaggle](https://www.kaggle.com/datasets/shivamb/go-emotions-google-emotions-dataset?select=go_emotions_dataset.csv), [hover above to go to the dataset.].The dataset has 31 columns, the *id,text,example_very_unclear and various emotions*.The Google AI GoEmotions dataset contains labeled comments from Reddit users expressing diverse emotions. This dataset is suitable for training neural networks to analyze text tonality, as it provides a comprehensive emotional spectrum and allows for subtle differentiation among various emotions. The dataset includes detailed emotional annotations and descriptive statistics, facilitating the analysis of emotions in text. While there may be limitations such as potential biases and subjective categorization, the GoEmotions dataset remains valuable for enhancing chatbot sensitivity, detecting online hazards, and improving customer support through the analysis of diverse emotions.
# 4) DATA EXPLORATION.
We  did various analysis for our EDA , below are some of the visualizations from our analysis.</br></br>
**a )A visualizations of the emotions and the counts of how they appear.** </br></br>
<img width="390" alt="Screenshot 2023-07-27 153407" src="https://github.com/learn-co-curriculum/dsc-data-visualization-with-pandas/assets/109750154/9be14307-30ee-4792-9aec-aee7b7e7f0b0"> </br></br>
</br>
**b) A visualization of the emotions categories and their counts.** </br>
So we have three emotion categories,  namely:
1) Positive emotions.
2) Negative emotions
3) Neutral emotions.</br></br>

<img width="404" alt="Screenshot 2023-07-27 153525" src="https://github.com/learn-co-curriculum/dsc-data-visualization-with-pandas/assets/109750154/d3944bbf-6772-4251-985c-27f544392ab9">   </br></br>
**c) A visualisation of the positive emotions and their counts.** </br></br>
<img width="396" alt="go_emotions" src="https://github.com/learn-co-curriculum/dsc-data-visualization-with-pandas/assets/109750154/57a5c2fe-29cc-4033-91f7-e8a4620619f7">
</br></br>
**d ) A Visualisation of the negative emotions and their counts.** </br></br>
<img width="393" alt="negative" src="https://github.com/learn-co-curriculum/dsc-data-visualization-with-pandas/assets/109750154/16a1298a-b173-4848-947a-cc4765ea8ae8">
</br></br>
**e) A visualization of the Top ten used emoji's.** </br></br>
<img width="629" alt="emoji's" src="https://github.com/learn-co-curriculum/dsc-data-visualization-with-pandas/assets/109750154/b4eaf0bc-c3f5-4da6-91a5-647c52fdda07">
</br></br>
**f) A visualization of the word counts before the removal of stop words.** </br></br>
<img width="433" alt="word_count" src="https://github.com/learn-co-curriculum/dsc-data-visualization-with-pandas/assets/109750154/36a3e0e8-8d0f-42b0-ac76-1cb8332ec9a7">
</br></br>
**g) A visualization of a word cloud we created.** </br></br>
<img width="578" alt="Screenshot 2023-07-27 153947" src="https://github.com/learn-co-curriculum/dsc-data-visualization-with-pandas/assets/109750154/7ce721ad-2504-44cf-85c4-c9dd8ad25797"> 
</br></br>
# 5) DATA PREPROCESSING.
In this stage, we seek to get the dataset in a format that is ready for the modeling , in our analysis , we did the following preprocessing steps.
1) Lowercasing the text column.
2) Removing punctuations.
3) Removing emoji's.
4) Performing word tokenization.
5) Removing stop words.
6) Lemmatization.
7) Emotions categorization.
8) Label encoding our emotions.
# 6) MODELLING AND EVALUATION.
In our sentiment analysis quest, we decided to model using four different models,these  models include:
1) Support Vector Machine models(SVM).
2) Recurrent Neural Networks(RNN).
3) Convolutional Neural Networks (CNN).
4) Transformer Models.(Specifically the BERT model).

After performing our analysis , we were to choose the best performing model and proceed with it to the deployment of the model, in our case the SVM model was the best performing model, with an accuracy of 0.97.
Below is how each model performed.</br></br>
**a) The SVM model.** </br></br>
Below is how our SVM model performed.</br>
<img width="334" alt="svm model" src="https://github.com/learn-co-curriculum/dsc-data-visualization-with-pandas/assets/109750154/2b68fea1-e445-42e5-84df-bb22273b3e15">
</br></br>
**b) The RNN model.** </br></br>
Below is how the RNN model performed. </br>
![image (1)](https://github.com/learn-co-curriculum/dsc-data-visualization-with-pandas/assets/109750154/eb91c687-1029-44b8-a93a-619a51a93a7f)
</br>
**c) The CNN model.** </br> </br>
Below is how the CNN model worked.</br>
![image (2)](https://github.com/learn-co-curriculum/dsc-data-visualization-with-pandas/assets/109750154/7c4d339d-28d1-487d-8575-29b72f0ddff3)
</br>
**d) The transfomer models(BERT model).** </br>
Below is how the bert model performed.
 From the above results, we can conclude that the best performing model was the SVM model hence this is what we shall use in the deployment stage.</br>
 # 7 ) MODEL DEPLOYMENT.
 There is really not much to get into, we deployed our best model (SVM) in the streamlit app.
 # 8) CONCLUSION.
 Reddit data shows predominantly positive sentiments towards the company.
The sentiment analysis model demonstrates high accuracy, precision, and recall for positive and neutral sentiments, making it reliable for sentiment analysis.
# 9) RECOMENDATIONS.
We would recomend that the from all the models the SVM model be used highly when performing this task of sentiment analysis as its results have proven to be quite high.
