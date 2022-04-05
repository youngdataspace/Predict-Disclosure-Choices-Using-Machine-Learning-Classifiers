# Currently working on this
# Outline
I build supervised machine learning models to predict whether IPO firms choose to disclose less before going public.

This notebook includes the following topics:
- Build prediction models using Random Forest, Logistic Regression, Naive Bayes, K-Nearest Neighbors, and Support Vector Machine
- Perform the K-Fold Cross-Validation and select the best performing model based on the average precision and recall values
- Tune hyperparameters using the Grid Search method whenever possible
- Evaluate the best model using precision, recall, and AUC

This notebook explains how I build the prediction models that I use in the first chapter of my UC Berkeley Haas dissertation. Nonetheless, it can be generalized and used to solve many other classification problems. By the way, a part of the first chapter is co-authored with my UC Berkeley PhD advisors and is published in the Critical Finance Review (a top 4 finance journal). Be sure to check the publication <a href = "https://cfr.pub/forthcoming/papers/eventov2021jobs.pdf">here</a>.

Enjoy reading this post!

# Background and Problem Statement
In 2012, the JOBS Act allowed IPO firms to reduce their financial disclosures before going public. In the first chapter of my dissertation, I examine the economic consequences of this Act and find that firms that choose to disclose less (hereafter "reduced-disclosure firms") become more overpriced. To explain the channel, I examine whether the reduction in disclosure is the driver of overpricing or whether certain types of IPOs that are known to be overpriced went public after the JOBS Act. The evidence shown in the rest of the chapter suggests the latter. 

The analysis in this notebook has a specific purpose: examine whether firms' choice can be predicted using their characteristics. If so, this analysis will further support the evidence in the rest of the chapter that reduced-disclosure firms are systematically different firms (I show in the paper that the firm characteristic differences are consistent with characteristics that are known to associate with overpricing).
