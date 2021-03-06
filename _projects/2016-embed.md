---
layout: project
title: Representations from Random Walk Diffusions
subtitle: Understanding the link between random-walk similarities and embeddings.
---

<img style="width: 40%; float: left; border: 1px solid black; margin-top: 10px; margin-right: 10px;" src="{{"/assets/projects/2016-embed.png" | prepend: site.baseurl }}"/>
**Overview:** 
Structured data such as sequences and networks pose substantial difficulty for traditional statistical theory which has focused on data drawn independently from a vector space. A popular and empirically effective technique for dealing with such data is to map elements of the data to a vector space and to operate over the embedding as a summary statistic. Such a vector representation of discrete objects is known as a `continuous representation'.
Continuous space models of words, objects, and signals have become ubiquitous tools for learning rich representations of data, from natural language processing to computer vision. Even in cases that the embedding is not explicit, many algorithms operate over similarity measures which implicitly embed the original dataset. In this line of work, we attempt to understand the intuition behind continuous representations. Can we construct a general theory of continuous representations? Are there general principles for semantically meaningful representations?

In order to answer these questions, we develop a framework for analyzing continuous representations through diffusion limits of random walks. We show that measurable quantities of discrete random walks with a latent metric structure have closed form diffusion limits. These diffusion limits allow us to approximate attributes of the discrete random walk such as the stationary distribution, hitting time, or co-occurrence using closed-form expressions from diffusions. We establish limits which guarantee asymptotic consistency of such estimators, and show they work well in practice.

Using this new approach, we solve three classes of problems: first, we derive principled network algorithms which connect statistical estimation tasks such as density estimation to network algorithms such as PageRank [[Hashimoto+2015](http://proceedings.mlr.press/v38/hashimoto15.html)][[Hashimoto+2016](http://papers.nips.cc/paper/6009-from-random-walks-to-distances-on-unweighted-graph)]. Next, we demonstrated that continuous representations of words are a type of random walk metric estimator with close connections to manifold learning [[Hashimoto+2016](https://transacl.org/ojs/index.php/tacl/article/view/809)]. Finally, we apply our theory to single-cell RNA seq data, and derive a way to learn time-series models without trajectories by using stochastic recurrent neural networks [[Hashimoto+2016](http://proceedings.mlr.press/v48/hashimoto16.pdf)].
