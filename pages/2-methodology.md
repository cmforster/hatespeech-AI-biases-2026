---
title: Methodology
short_title: Methodology
permalink: /methodology/
order: 2
---
## What is BERT?

BERT is a language model originally developed by Google in 2018 (Devlin et al., 2019), with its name standing for “Bidirectional Encoder Representations from Transformers”. It is essentially a model for understanding complex texts through encoding it into mathematical representations (vectors), but it cannot produce text itself. This process of BERT’s text understanding happens through transformers, a neural network component pioneered by Google researchers in 2017 with a famous paper entitled “Attention is all you need” (Vaswani et al., 2017), which has been cited more than a staggering 241 000 times now. Transformers aim to improve language models’ understanding of long-range context in language, meaning how words in a text relate to each other even if they are far apart. Transformers critically introduced self-attention, which is a mechanism by which a model looks at every word in a sentence or text simultaneously and decides itself how strongly which words relate to each other, which allows models to understand contextual meaning better. BERT is an encoder-only model, which reads and learns a representation of text in the form of a vector. Other language also use a decoder, which would transform this encoded representation back into text. BERT only uses an encoder, which is why it cannot output text in its basic version.

BERT’s basic model is trained on unlabelled text, like books, news, and websites already existing. It is trained through two training tasks: masking individual words in a sentence and making BERT predict them as well as predicting the logical order of sentences. BERT was a key advance in natural language processing at the time of its release because it is bidirectional (Devlin et al., 2019) - reading text in both directions, meaning it uses both the words coming before and after each word to assess this context - which makes it better at nuanced understanding. It is used and useful for a variety of tasks because an additional layer can be added to it to adapt it to different tasks, which is the BERT use case this project is occupied with. 

The Mathew et al. (2022) paper was presented at AAAI 2021 and intended to establish a benchmark dataset to allow other researchers to test their model’s ability to detect hate speech on it. The authors are mixed from the Indian Institute of Technology Kharagpur and the University of Hamburg in Germany, with no funding or conflicts of interests declared in the conference paper. They created HateXplain to address previous issues of bias and interpretability in hate speech detection, doing so through annotating a Twitter- and Gab-sourced dataset of 20 148 posts in three categories: classification (is it hate speech, offensive, normal), the community targeted by hate/offensive speech, and the rationale (the parts of the post that provided the basis for the labelling decision of the labellers). This dataset is then used to train a specialised model of BERT, BERT hatexplain (Mathew et al., 2022b), which can be used to classify text as hatespeech, offensive, or normal (Mathew et al., 2022a). 



## Citations

Devlin, J., Chang, M.W., Lee, K. and Toutanova, K., 2019, June. Bert: Pre-training of deep bidirectional transformers for language understanding. In Proceedings of the 2019 conference of the North American chapter of the association for computational linguistics: human language technologies, volume 1 (long and short papers) (pp. 4171-4186). 

Mathew, B., Saha, P., Yimam, S.M., Biemann, C., Goyal, P., Mukherjee, A., 2022a. HateXplain: A Benchmark Dataset for Explainable Hate Speech Detection. https://doi.org/10.48550/arXiv.2012.10289 

Mathew, B., Saha, P., Yimam, S.M., Biemann, C., Goyal, P., Mukherjee, A., 2022b. Hate-speech-CNERG/bert-base-uncased-hatexplain [WWW Document]. Hugging Face. URL (accessed 4.27.26). 

Vaswani, A., Shazeer, N., Parmar, N., Uszkoreit, J., Jones, L., Gomez, A.N., Kaiser, Ł., Polosukhin, I., 2017. Attention is all you need. Advances in neural information processing systems 30. 


{% include chapter-nav.html %}
