---
layout: post
title:  Introducing PAUSE - A deep natural language model for the private markets
date:   2021-11-26 15:05:00 +0300
image:  /assets/images/blog/pause.jpg
author: Lele Cao, Sonja Horn
tags:   EQT
---

**[Motherbrain](https://eqtgroup.com/motherbrain) is a digital platform that leverages Big Data and Machine Learning to give EQT a unique edge. Motherbrain started in 2016 as a platform for EQT Ventures to be truly data-driven in finding the best tech start-ups to invest in.** 

Recently, [an academic paper](https://aclanthology.org/2021.emnlp-main.791/) authored by the data science team at Motherbrain has been accepted for publication by the [EMNLP 2021](https://2021.emnlp.org/). The conference is acknowledged as one of the best NLP (Natural Language Processing) academic conferences in the world, with papers previously published from the likes of Google, Facebook and Stanford.

#### Data and deep learning in private capital

Investors in financial markets have traditionally relied on personal networks to find the best opportunities. While private capital investors still rely heavily on this strategy, investors in public markets have turned their heads towards a more data driven and algorithmic approach that promotes automation, objectiveness, consistency and adaptability.

Machine learning is commonly used in public markets for applications such as asset pricing, quantitative investing and portfolio optimization. The technical developments on the public market have been facilitated by the availability of large amounts of data on publicly traded assets. In contrast, data on private companies has traditionally been difficult to gather and share due to confidentiality, while data on public companies has low relevance in the private setting. These conditions have formed a huge obstacle for applying machine learning in the private capital sector.

This is changing. The ubiquity of digitization means that large amounts of high-quality data on private companies is publicly accessible. This trend has enabled some recent machine learning attempts, particularly in Venture Capital, which try to estimate the likelihood of a business succeeding (startup success prediction) leveraging mostly public datasets like Crunchbase and LinkedIn. However, the application of state-of-the-art deep learning models is rare among these prediction tasks, as the models are typically limited by two conflicting facts. For one, deep learning only performs well if exposed to a large number of successful examples that “teach” the model. And yet, successful startups are scarce by nature.

There are many processes that would benefit from the application of deep learning: aside from startup success prediction, other examples include deal sourcing and competitor mapping. In all these cases, the successful adoption of deep learning relies on the availability of a large amount of supervision signals — or, in other words, ground truths to “teach” the model how to act in a particular scenario, also called labels or annotations. However, it is practically impossible to get hold of enough supervision signals.

**Leveraging deep learning for competitor mapping**

Competitor mapping relies on properly measuring the relatedness between any two companies, which typically involves qualitative analysis of textual descriptions to identify similar companies to the target. Automating this process could save time, ensure accuracy, and help identify companies that might otherwise be missed.

A way to automate this work is to train some kind of model to output similarity between a pair of companies based on their textual descriptions. There are existing approaches to achieve this using public data that contains generic texts from sources like wikipedia and news articles. However, without training the model on company descriptions, the model will easily fail to distinguish between "a user-friendly financial platform managed via cloud infrastructure" and "a cloud infrastructure provider that is financially friendly". A general model that is trained using only public data might think these two companies are very similar, when in practice they belong to entirely different business sectors.

Training a state-of-the-art, expert model to understand company descriptions involves annotating the descriptors to indicate relatedness. It’s a time consuming process. Using rough figures, to properly train a deep learning model one might need one million annotations. Assuming it takes 30 seconds to manually annotate if two companies are related, obtaining that one million annotations would take 347 days. Nearly a whole year before it’s even possible to train a model to undertake the competitor mapping. So, the data science team asked themselves: 

> Is there a way to apply deep learning in a way that allows Motherbrain to leverage an entire company dataset, not just annotated descriptors?

**Yes, there is!**

PAUSE — Positive and Annealed Unlabeled Sentence Embedding — generates numerical representations from company descriptions, enabling a measurement of closeness between any two companies. It uses an entire dataset, not just annotated descriptors, meaning the model needs far fewer supervision signals to undertake the competitor mapping task successfully. In practise, the proposed method requires about 5–10% of the annotated descriptors. Using the earlier calculation, enabling training models for competitor mapping can be completed in a matter of weeks, rather than 12 months.

The model is best-in-class at generating the correct representations without relying heavily on pre-existing annotations by investment professionals, as other high performing models do. But it is not just improving competitor mapping: PAUSE can be applied to countless applications in private capital because it solves the biggest issue in applying deep learning to the industry — lack of annotations.

To learn more about PAUSE and how it works, please read our [Medium article](https://medium.com/eqtventures/introducing-pause-a-deep-natural-language-model-for-the-private-markets-55f27033115) or watch the [presentation video](https://underline.io/lecture/37659-pause-positive-and-annealed-unlabeled-sentence-embedding).