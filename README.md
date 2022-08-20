# NLP: Aspect Category Sentiment Analysis (ACSA)

## Project Description
This project aims to solve the Subtask 4 in SemEval 2014 Task 4 - Aspect Based Sentiment Analysis
The Subtask 4 is Aspect category polarity or Aspect category sentiment analysis (ACSA): 
Given a set of pre-identified aspect categories (e.g., {food, price}), determine the polarity (positive, negative, neutral or conflict) of each aspect category. For example:
- “The restaurant was too expensive” → {price: negative}
- “The restaurant was expensive, but the menu was great” → {price:negative, food: positive}

## Methodology 
For ACSA task, I used BART pre-training model. I took references from the great paper Solving Aspect Category Sentiment Analysis as a Text Generation Task (Liu, 2021)

## Data
The dataset I used in this task is SemEval 2016

## Model result:
My model achieved 87.4% accuracy on the validation test and 85.5% on the test set.

## Future works:
- I detected some errors of the labels in the training dataset. I believe the model test accuracy can be improved with data of better annotation. 
- In addition, the training dataset is very imbalanced, with less data for neutral polarity. We can consider oversampling methods in the future training.  
- I notice the model tends to performe worst in predicting the opinion of a sentence with both positive and negative meanings. Therefore, if the model is trained with more of such sentences,  the model can be more generalized and achieve a better performance. 

# References
- SemEval 2014 Task 4 - Aspect Based Sentiment Analysis: https://www.aclweb.org/portal/content/semeval-2014-task-4-aspect-based-sentiment-analysis
- Solving Aspect Category Sentiment Analysis as a Text Generation Task: https://aclanthology.org/2021.emnlp-main.361/
- Paper: Jian Liu et.al, 2021, Solving Aspect Category Sentiment Analysis as a Text Generation Task (including codes: https://github.com/lgw863/acsa-generation)
