# NLP: ABSA: Aspect Category Sentiment Classification

## Description of SemEval 2014 Task 4 - Aspect Based Sentiment Analysis
Subtask 1: Aspect term extraction
Given a set of sentences with pre-identified entities (e.g., restaurants), identify the aspect terms present in the sentences.

An aspect term names a particular aspect of the target entity (e.g., "I liked the service and the staff, but not the food”, “The food was nothing much, but I loved the staff”).

Subtask 2: Aspect term polarity
Given one or more aspect terms within a sentence, determine whether the polarity of each aspect term is positive, negative, neutral or conflict (i.e., both positive and negative).

For example:
“I loved their fajitas” → {fajitas: positive}
“I hated their fajitas, but their salads were great” → {fajitas: negative, salads: positive}
“The fajitas are their first plate” → {fajitas: neutral}
“The fajitas were great to taste, but not to see” → {fajitas: conflict}

Subtask 3: Aspect category detection
Given a predefined set of aspect categories (e.g., price, food), identify the aspect categories discussed in a given sentence. Aspect categories are typically coarser than the aspect terms of Subtask 1, and they do not necessarily occur as terms in the given sentence. For example, given the set of aspect categories {food, service, price, ambiance, anecdotes/miscellaneous}:
“The restaurant was too expensive”  → {price}
“The restaurant was expensive, but the menu was great” → {price, food}

Subtask 4: Aspect category polarity
Given a set of pre-identified aspect categories (e.g., {food, price}), determine the polarity (positive, negative, neutral or conflict) of each aspect category. For example:
“The restaurant was too expensive” → {price: negative}
“The restaurant was expensive, but the menu was great” → {price:negative, food: positive}

# References
SemEval 2014 Task 4 - Aspect Based Sentiment Analysis: https://www.aclweb.org/portal/content/semeval-2014-task-4-aspect-based-sentiment-analysis
Solving Aspect Category Sentiment Analysis as a Text Generation Task: https://aclanthology.org/2021.emnlp-main.361/
Codes: https://github.com/lgw863/acsa-generation
