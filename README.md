![alt text](https://imgur.com/nmUzYQ9.jpg)

An unsupervised learning project that clusters benchmark results from 3DMark's Time Spy results.

## Summary

In conjunction with the predecessor of this project, I wanted to see what labels I would be able to decipher from the different clustering methods that I will be using. This can give a lot of businesses insights on whether how to properly categorize their consumer offerings without primarily considering much about offering the best in the price point. In a way, this is mostly exploratory and naïve considering the non-existence of the labels I wanted to see.

## Rationale

While it is easy to categorize desktop parts and laptop computers by their respective price points and known tiering, it would be more interesting to see other labels machine learning can provide or give an insight to. With those potentials, it would be possible to further group computers beyond the known labels and understand more of the unseen data.

## Process

Utilizing my trusty 3DMark scraper again, I was able to collect over 2 million results with varying GPUs with Time Spy data alone. Ranging from laptops to workstation-class GPUs, the data that I was able to collect is overly sufficient and might I say a little too much for unsupervised learning limits. I have not explored the path of using Spark to do this yet but the current limits presented by just using Pandas and known libraries with clustering can be limiting if I were to not do an inferential research.

I have utilized two dimensionality reduction techniques for this project - PCA and FAMD. PCA was troublesome to work with, if at all, since the initial sparseness it presented if I were to use all categorical variables was not accounted for during the making of this project.

Visualization was done through TSNE and UMAP.

## Changelogs

02.07.21 - Finally added a proper readme.

## Stack

Research is in Python on Jupyter Notebook.
Data was collected in Python with BS4.
Clustering methods used: UMAP, TSNE, K-Means, DBSCAN, Agglomerative Clustering, GMM, K-Medoids
