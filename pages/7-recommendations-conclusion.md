---
title: Recommendations and Conclusion
short_title: Recommendations and Conclusion
permalink: /Recommendations/
order: 7
---
# Recommendations

Datasets like the one used in this study will continue to be essential in training AI models in the goal of identifying hate speech and other harmful content on social media platforms, something that will only continue growing in importance in the coming years. However, with the detailed analysis of how humans and AI models classify different types of speech present in this study, and the implications of the differences that were observed, this study proceeds to provide recommendations to improve these datasets, and the way they are created, for their purpose, and hopefully positively influence the outcomes from them.

The quantitative data from our study, particularly the high rate at which the human annotators moved over 80% of AI-labeled “Hate speech” into the “Offensive” category, shows a critical weakness in the current moderation architecture as a whole; namely, that the “Offensive” category transforms into a catch-all for any linguistically diverse posts that are not either strictly inoffensive or clearly inciting political violence. Davidson et al. (2017), for example, find that “racist and homophobic tweets are more likely to be classified as hate speech but that sexist tweets are generally classified as offensive” (p. 512). By grouping reclaimed slurs, self-deprecating humor, irony, in-group references, and aggressive speech under one single label, nuance is lost not only in the AI model’s categorization, but in the nature of the categorization itself. Generalizing diverse speech into one broad “Offensive” category is inherently destructive to the quality of the training data too. As noted in the IYKYK (2026) study, this compressing of language is unable to capture “community-level heterogeneity” and thereby makes the categorization of any language that is not at the ‘extreme’ end effectively moot. More focused studies, such as that advocated by the AIWizards (2024) team, suggest that training models with hierarchical context is one way to develop more sophisticated ‘reasoning’, where this over-generalization into the “Offensive” category is combatted by the system evaluating the speaker’s relationship to the term based on context. In general, if this study were repeated, the research team would suggest a more extensive set of classifications be used beyond “Normal”, “Offensive”, and “Hate speech” to tackle this large grey zone that the majority of posts ended up being grouped into.  

Given these points, the construction of the datasets can be adapted to achieve better results. The first recommendation we leverage from our findings is the importance of precisely defining the purpose and objectives of the datasets. Different aims for the AI models (removing hate speech, identifying and flagging offensive posts, or providing a better user experience) will lead to different necessities. Indeed, if the AI model will be used for removing hate speech, it needs to be equipped with a strong and unwavering sense of what is classified as hate speech, which means a clear definition of hate speech but a dataset with limited scope and context. However, if the AI model will be used to provide a better user experience, flagging discriminatory, offensive text and more, annotators will need both more context and a wider variety of annotation options, as well as potentially inputting context coding. To achieve this, dataset creators will have to achieve a further understanding of market needs.

A second recommendation, stemming from the understanding that different use cases for the AI models trained on these databases, is the need for additional context on the posts being classified by human annotators. Additional context for the annotators on the content they are analysing, including the posts that the content is replying to, can boost the accuracy of the annotations, yielding more efficient and accurate AI models. Software can be created to render the visual presentations and the additional information easier to analyse for the annotators.

Diversifying the platforms where the data is collected for the databases is crucial. The database analysed by this study took into account only Twitter and Gab which are arguably some of the most prone to the presence of hate speech among the content present given their lax content moderation. Furthermore, the content on these two platforms may reflect far-right ideological content bubbles more than other platforms. Using content from only these two platforms may create blindspots for the AI’s trained on this data. Including content from other platforms will include the different ideologies, cultures and perspectives of the posts on these, improving the accuracy of the AI models trained on the databases.

Finally, the selection of annotators, which in the case of the dataset this study analysed was selected through Amazon Mechanical Turk, should be done to enable the clearest understanding of the cultural context of the content presented. Indeed, if the content is mostly US-centred, it should be US annotators interacting with the database’s content and annotating. Furthermore, some demographic data about the annotators (such as country of residence and age) should be included in the information attached to the database in order to increase transparency and understanding regarding the context in which the database was created.

## Citations

Davidson, T., Warmsley, D., Macy, M., & Weber, I. (2017). Automated Hate Speech Detection and the Problem of Offensive Language. Proceedings of the International AAAI Conference on Web and Social Media, 11(1), 512-515. https://doi.org/10.1609/icwsm.v11i1.14955 

IYKYK (But AI Doesn't): Automated Content Moderation Does Not Capture Communities' Heterogeneous Attitudes Towards Reclaimed Language. (2026). arXiv. https://arxiv.org/html/2604.16654v2

‌Tedeschini, Luca, and Matteo Fasulo. “AIWizards at MULTIPRIDE: A Hierarchical Approach to Slur Reclamation Detection.” ArXiv.org, 2026, arxiv.org/abs/2602.12818. 



{% include chapter-nav.html %}

