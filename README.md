# [Faithful Explanations of Black-box NLP Models Using LLM-generated Counterfactuals](https://openreview.net/forum?id=UMfcdRIotC)

# Authors:

[Yair Ori Gat](https://scholar.google.com/citations?user=ONm-EGQAAAAJ&hl=iw&oi=ao), [Nitay Calderon](https://scholar.google.com/citations?user=_1qnAh4AAAAJ&hl=iw&oi=ao), [Amir Feder](https://scholar.google.com/citations?user=ERwoPLIAAAAJ&hl=iw&oi=ao), [Alexander Chapanin](), [Amit Sharma](https://scholar.google.co.in/citations?user=CXgQufgAAAAJ&hl=en), [Roi Reichart](https://scholar.google.com/citations?user=xXJIsh4AAAAJ&hl=en)

# Abstract

Causal explanations of the predictions of NLP systems are essential to ensure safety and establish trust. Yet, existing methods often fall short of explaining model predictions effectively or efficiently and are often model-specific. 
In this paper, we address model-agnostic explanations, proposing two approaches for counterfactual (CF) approximation.
The first approach is CF generation, where a large language model (LLM) is prompted to change a specific text concept while keeping confounding concepts unchanged. While this approach is demonstrated to be very effective, applying LLM at inference-time is costly. 
We hence present a second approach based on matching, and propose a method that is guided by an LLM at training-time and learns a dedicated embedding space. This space is faithful to a given causal graph and effectively serves to identify matches that approximate CFs.
After showing theoretically that approximating CFs is required in order to construct faithful explanations, we benchmark our approaches and explain several models, including LLMs with billions of parameters. 
Our empirical results demonstrate the excellent performance of CF generation models as model-agnostic explainers. 
Moreover, our matching approach, which requires far less test-time resources, also provides effective explanations, surpassing many baselines. 
We also find that Top-K techniques universally improve every tested method. 
Finally, we showcase the potential of LLMs in constructing new benchmarks for model explanation and subsequently validate our conclusions. Our work illuminates new pathways for efficient and accurate approaches to interpreting NLP systems.

