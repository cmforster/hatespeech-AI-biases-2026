---
title: Introduction
short_title: Introduction
permalink: /introduction/
order: 1
---

With the rise of social media platforms, identifying and moderating hate speech online has become an ever-more pressing challenge. As of 2025, 74% of the global population has gained access to the internet, and with that comes the possibility to express oneself freely and anonymously online (ITU, 2025). This advancement has democratised free speech and removed the power previously held by editors, publishing houses, and broadcasters to gatekeep certain content. Meaningful changes to democratic processes can be identified, as strong social media presence and campaigns have enabled previously lesser-known political candidates to reach wider audiences and get elected, as exemplified by Zohran Mamdani in the New York Mayoral Election in 2025 (Searchlight Institute 2025). Yet that same shift in access to new media has dismantled the safeguards those editors, publishers and broadcasters provided. Content that would not have survived review can now reach millions within minutes, and given the vast volume of content posted across platforms, fully human moderation is impossible. 

According to the Stanford Human-Centred Artificial Intelligence Centre (Gordon et al., 2021), AI models are the first line of defence against online hate speech. Facebook claims its models have identified and taken down 27 million hate-speech posts in the final three months of 2020 alone (ibid). Their algorithm was even faster than humans, flagging content before users did in 97% of cases. However, the path between helpful content moderation and the repression of freedom of speech is narrow. Errors in either direction carry serious consequences, with over-classification risking silencing political dissent and satirical speech. At the same time, under-classification allows targeted harassment, incitement to violence, and dehumanising content to be spread. When content moderation decisions are delegated to algorithms, the stakes of those errors are vastly multiplied. This raises the question of what basis these systems use to make their decisions, and how reliable the data on which they were trained is. Hate speech detection algorithms are only as good as the annotations that trained them, and are heavily shaped by the cultural context, linguistic background, and in-group vs out-group biases of the human annotators. Investigating the training data set, the people who manually annotated the posts, and the context and conditions under which they were labelled are essential for understanding how and when posts are flagged as hate speech, with far-reaching consequences for private and political life. 

This paper examines these questions using the HateXplain dataset and the BERT-HateXplain classifier. It aims to investigate the classification of the original annotators outsourced to Amazon Mechanical Turks (MTurks) and compare it with the research group’s own labels, as well as two LLMs, namely Grok and Claude. The analysis proceeds in four parts: a working definition of hate speech, a quantitative analysis of inter-annotator (dis-)agreement across all groups, a qualitative analysis of the different interpretations that likely produced the disagreement, and a discussion about the findings in terms of making recommendations while acknowledging the limitations of the research.

### Citations

International Telecommunication Union (2024). Individuals using the internet (% of population). World Telecommunication/ICT Indicators Database. Washington, D.C.: World Bank. Available at: https://data.worldbank.org/indicator/IT.NET.USER.ZS (Accessed: 29 April 2026).

Searchlight Institute (2025) 'How Zohran Mamdani won', Searchlight Institute, 5 November. Available at: https://www.searchlightinstitute.org/research/how-zohran-mamdani-won (Accessed: 29 April 2026).


{% include chapter-nav.html %}
