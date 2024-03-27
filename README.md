# Document-level Event Causality Identification with Knowledge-guided Multi-turn Question Answering

## Introduction
### Research Background
Event causality identification (ECI) is a crucial information extraction (IE) task aimed at identifying causal relations between event mentions in text. This task is challenging because causal relations are often implicit in text, requiring models to understand the associations between events. Existing methods rely on pre-trained language models (PLMs) but struggle to comprehensively capture these associations. Some methods use external knowledge or data augmentation, but these approaches have limitations.

### Research Challenges
Current research on ECI faces challenges, including the limitations of PLM-based methods, which fail to fully model associations among events, and LLM-based methods, which struggle with understanding texts and specific tasks. These challenges highlight the need for a new approach to ECI.

### Objectives
To address these challenges, we propose a knowledge-guided multi-turn question-answering approach for document-level ECI. Our objectives are to leverage large language models (LLMs) for implicit semantic understanding and to formulate ECI as a multi-turn question answering task to improve performance.

## Main Findings
1. Generative models (GPT-4 and Flan-T5-XL) perform comparably or better than the standard BERT model under the zero-shot setting. Utilizing multi-turn question answering and temporal reasoning further improves results, approaching the state-of-the-art model, RichGCN.
2. Fine-tuning the generative model, Flan-T5-Base, outperforms state-of-the-art PLM-based models on both ECI and CRE tasks, demonstrating the effectiveness of generative models for binary classification and causal reasoning.
3. Cross-task knowledge, such as event arguments and their relations, aids in identifying causal relations between events but does not help in CRE due to a lack of explicit connection with events.

## Conclusion
Our approach demonstrates the effectiveness of knowledge-guided multi-turn question answering for document-level ECI. Future research could explore further improvements in leveraging external knowledge and enhancing cross-task knowledge for better performance.
