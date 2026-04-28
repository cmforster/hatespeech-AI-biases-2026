---
title: Methodology
short_title: Methodology
permalink: /methodology/
order: 2
---
> **Research question: How does dataset annotation influence hate speech classification and what does this imply for automated content moderation?**

The analysis of the dataset was chosen specifically due to the importance of annotated datasets like this in the training of classifiers like BERT hatexplain is one. BERT is adapted to hate speech classification through supervised learning - comparing the model’s predictions to what is the ‘correct’ label provided in the dataset and successively correcting itself, so what is conceived as this ‘correct’ answer in the dataset is crucial to the classifications the model ultimately makes - “supervised machine learning [...] is only as good as the quality of the data” (Geiger et al., 2021).

A 500-post subset was randomly selected from the original dataset for analysis. The analysis focuses specifically on the classification and the target community properties and not the rationales - while they were important in terms of the innovation of this dataset, this project takes an approach more focused on what hate speech is and what the effects of this definition may be in the context of AI detection of hate speech. Furthermore, capacity constrained us from analysing the rationales, which would have been a lot more text-and time-intensive and therefore prohibitive to choosing a sufficiently large subset of the dataset for the analysis to be meaningful.

## Dataset

The original full dataset contains 20 148 of posts collected from Twitter and Gab, with the rationale that these platforms are frequently subject to hate speech analysis. This is a practicable choice by the authors but it may have been interesting to study other platforms in order to understand how hate speech manifests in different contexts.

It was then annotated through gig workers with Amazon Mechanical Turk, which the paper claims were instructed as following:

“We prepare instructions for workers that clearly explain the goal of the annotation task, how to annotate spans and also include a definition for each category. We provided multiple examples with classification, target community and span annotations to help the annotators understand the task.”

However, quite crucially, the paper does not provide the specific instructions or examples given to the annotators, which would have been instrumental in assessing how they defined hate speech and how they shaped the opinion of annotators on the same.
Data collection for our project
As ca. 20 000 entries are too many to manually analyse, a subset of 500 posts was chosen through pseudo-random number generation. As there were roughly similar proportions of Twitter posts (9027 posts / 44.9%) and Gab posts (11093 posts / 55.1%) in the original dataset, this was not accounted for, which left us with PROPORTIONS IN OUR TARGET DATASET. For our purposes, the data was exported from GitHub and converted to a .csv file, with columns for:

"annotator1_classification", "annotator1_targetgroup", "annotator2_classification", "annotator2_targetgroup", "annotator3_classification", "annotator3_targetgroup"

An additional variable was added to differentiate between the two origin platforms Twitter and Gab and facilitate respective analysis.

### Annotation process

The project aims to explore how the dataset constructs hate speech and where it draws the boundaries between hate and offensiveness, as this will respectively inform BERT’s hate speech classification and would find similar applications in content moderation contexts. To facilitate this, there were several steps of additional coding and analysis:

The AMT annotations for all posts were hidden and each group member was randomly allocated a subset of 100 posts to classify as hate, offensive, or normal and identify the target group. Our understanding of hate speech was facilitated by a previous analysis of differing legal and platform definitions of hate speech, as is discussed in the following section.
In a second round, each group member was allocated a further 100 random posts among the 400 they had not seen previously through an ordered repetition that meant there were not two annotators grouped for the analysis of the same 100 posts.
Grok AI and Claude AI, without seeing the annotations of the group members or AMT, respectively classified all 500 posts as hate, offensive, normal, and identified their target group in a process described in more detail in the following section.

Through this approach, we hope to highlight the discrepancies in what hate speech can mean under different definitions and perceptions of offensiveness and how this can influence content moderation practices.

### Supplementary annotation through LLMs

In addition to the human annotations from AMT and the project group, it was decided to include two LLM-generated annotations. According to the Stanford Human-Centred Artificial Intelligence Centre (Gordon et al., 2021), AI models are the first line of defence against hate speech online. Facebook claims its models have identified and taken down 27 million hate-speech posts in the final three months of 2020 alone (ibid). The system was even faster than humans, flagging content in 97% of cases. However, the path between helpful content moderation and the limitation of freedom of speech is narrow. While automated speech police might perform exceptionally well on technical tests, they can cause considerable discontent among humans with their choices. The primary issue is that, particularly in today’s divisive context, evaluating more conventional AI tasks, such as spoken language recognition, is very different from the considerably more challenging task of identifying hate speech, harassment, or misinformation.

While classifier models used to recognise hate speech are different types of AI to LLMs, using LLMs for annotation here is very interesting as they reveal the bias of their source data and training, which often includes a broad range of resources representing elements of general public opinion. Asking them to qualify what is hate speech may therefore give insight into the public perception of hate speech, which is in turn important for moderation practices and may inform platform understandings of appropriate moderation.


### Citations

Geiger, R.S., Cope, D., Ip, J., Lotosh, M., Shah, A., Weng, J., Tang, R., 2021. “Garbage In, Garbage Out” Revisited: What Do Machine Learning Application Papers Report About Human-Labeled Training Data? Quantitative Science Studies 2, 795–827. https://doi.org/10.1162/qss_a_00144 

Gordon, M., Zhou, K., Patel, K., Hashimoto, T. and Bernstein, M. (2021) 'The disagreement deconvolution: Bringing machine learning performance metrics in line with reality', Proceedings of the 2021 CHI Conference on Human Factors in Computing Systems, Article 470. https://doi.org/10.1145/3411764.3445423


{% include chapter-nav.html %}
