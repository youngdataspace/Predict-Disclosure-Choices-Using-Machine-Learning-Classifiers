# Outline and Introduction
In this post, I explain how to build and evaluate supervised machine learning models in Python.

The outline of this post is summarized as follows:
- Build classification models using Naive Bayes, Random Forest, AdaBoost, Logistic Regression, K-Nearest Neighbors, and Support Vector Machine 
- Tune hyperparameters using the Grid Search method
- Evaluate the models and select the best model using precision, recall, and AUC

As a working example, I will explain how we can predict whether IPO firms choose to reduce pre-IPO disclosures using firm characteristics. I use these predictions in the first chapter of my UC Berkeley Haas dissertation (<a href = "https://sites.google.com/view/young-yoon-brief-abstracts/home">link</a>). Nonetheless, it can be generalized and used to solve many other classification and prediction problems. By the way, a part of the first chapter is co-authored with my UC Berkeley PhD advisors and is published in the Critical Finance Review (a top 4 finance journal). Be sure to check the publication <a href = "https://cfr.pub/forthcoming/papers/eventov2021jobs.pdf">here</a>.

# Background and Problem Statement
In 2012, the JOBS Act allowed IPO firms to reduce their financial disclosures before going public. In the first chapter of my dissertation, I examine the economic consequences of this Act and find that firms that choose to disclose less (hereafter "reduced-disclosure firms") become more overpriced. To explain the channel, I examine whether the reduction in disclosure is the driver of overpricing or whether certain types of IPOs that are known to be overpriced went public after the JOBS Act. The evidence shown in the rest of the chapter suggests the latter. 

The analysis in this notebook has a specific purpose: examine whether firms' choices can be predicted using their characteristics. If I can indeed predict firms' choices, then it confirms the evidence in the rest of the chapter that it is not the reduced-disclosure choice per se leading to more prevalent overpricing but rather the firm characteristics of reduced-disclosure firms.
