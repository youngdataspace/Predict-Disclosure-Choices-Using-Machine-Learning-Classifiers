# Outline
I build supervised machine learning models to predict whether IPO firms choose to disclose less before going public.

This notebook includes the following topics:
- Build Random Forest, Logistic Regression, Naive Bayes, K-Nearest Neighbors, and Support Vector Machine models
- Tune hyperparameters using the Grid Search method 
- Perform the K-Fold Cross-Validation to select the best performing model based on precision and recall values
- Evaluate the best model using precision, recall, and AUC

This notebook explains how I build the prediction models that I use in the first chapter of my UC Berkeley Haas dissertation. Nonetheless, it can be generalized and used to solve many other classification problems. By the way, a part of the first chapter is co-authored with my UC Berkeley PhD advisors and is published in the Critical Finance Review (a top 4 finance journal). Be sure to check the publication <a href = "https://cfr.pub/forthcoming/papers/eventov2021jobs.pdf">here</a>.

Enjoy reading this post!

# Background and Problem Statement
In 2012, the JOBS Act allowed IPO firms to reduce their financial disclosures before going public. In the first chapter of my dissertation, I examine the economic consequences of this Act and find that firms that choose to disclose less (hereafter reduced-disclosure firms) become more overpriced. To explain the channel, I examine whether the reduction in disclosure is the driver of the overpricing or whether certain types of IPOs that are known to be overpriced went public after the JOBS Act. The evidence suggests the latter. 

The analysis in this notebook has a specific purpose: examine whether firm characteristics can explain firm's choice by building 

In order to further support the finding that reduced-disclosure firms are systematically different firms, I examine whether firm characteristics can be used to classify such firms. As shown below, the Random Forest model built using several firm characteristics does a good job of predicting reduced-disclosure firms. This evidence suggests that reduced disclosure firms and other firms are systematically different. As explained in my dissertation,  and thus the disclosure choice per se isn't the driver of my findings.
