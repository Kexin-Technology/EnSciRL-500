# EnSciRL-500

The dataset of 500 English Scientific Research Literatures (EnSciRL-500) is from ***the NLPCC2024 Shared Task 6: Scientific Literature Survey Generation*** of [The 13th CCF International Conference on Natural Language Processing and Chinese Computing (NLPCC 2024)](http://tcci.ccf.org.cn/conference/2024/taskdata.php).

## Dataset

Name: 500 English Scientific Research Literatures (EnSciRL-500)

File: train data_2024_forNLPCC.7z

HuggingFace download: [Kexin Technology/EnSciRL-500](https://huggingface.co/datasets/Kexin-Technology/EnSciRL-500)

## Guideline of the NLPCC2024 Shared Task 6

A.Competition background

Doing literature survey is a necessary part of scientific research. However, it takes more and more time for researchers to do this, since the amount of scientific publications is vast and the publishing speed is still increasing rapidly. AI-generated literature survey can help researchers to save time. It becomes more realistic for researchers to adopt AI-generated literature survey with the power of large language model (LLM).

In this competition, we will further investigate the possibility and evaluate the usability of AI-generated literature survey. Given a list of topic-related references, the task aims to develop models for long form literature survey generation. We provide a training set which contains randomly crawled arXiv survey papers together with their references. For each survey paper, participants are expected to provide a corresponding AI-generated survey by developing retrieval augmented generation models based on the content and references in the original survey paper. Both automatic and human evaluation will be conducted to measure the generated survey outline and content quality. There is no limit for the use of large language models (e.g. LLaMA2, GPT4, etc.), however, reverse engineering is not allowed.

B.Competition task

To develop retrieval augmented text generation models for scientific literature survey generation, based on the given metadata (title, subject, abstract, references) of scientific research literature survey papers and corresponding survey text in different scientific fields.

C.Deliverables

Model development code, report, and generated surveys.

D.Training data

We provide around 500 English scientific research survey papers, of which 400 can be used as training set and 100 can be used as verification set. Each sample data contains the title, article_id, subject, abstract, reference, reference_content of the article and survey content. (Note: data other than the training set cannot be used in the process of model development).
The sample of training data is provided as JSON files which are displayed as Fig 1. “reference_content” contains title and abstract for part of references.

![image](https://github.com/user-attachments/assets/02af92ca-6f5f-48bb-ad59-150d8a440e4c)

E.Testing data

200 survey papers are provided as testing set. The testing datasets will be provided as a JSON file in format of {“subject”: “”,  “reference”: [...]}

F.Evaluation criteria

Automatic evaluation is mainly based on ROUGE, Soft Heading Recall1, LLM and human evaluation will also be conducted to measure the survey outline and content quality. Each method will be accounted for 25% weight.

(1)We utilize ROUGE-1/2/L provided by Google2 to evaluate the content of generated survey.

(2)We utilize Soft Heading Recall for evaluating the structure of generated survey.

(3)We utilize LLM and human experts to evaluate the following aspects:

- Fluent language with clear expression;
- Logical article structure;
- Ample, reliable, and accurate citations;
- Consistency of content with the theme, staying on-topic;
- Broad analytical scope.

## Organizers

Organizations: [Kexin Technology](https://note.kxsz.net/), Deakin University

Organizers: Yangjie Tian, Xungang Gu, Aijia Li, [He Zhang](https://scholar.google.com/citations?user=CM_tgIEAAAAJ&hl=en&oi=ao)\*, Ruohua Xu, Yunfeng Li, [Ming Liu](https://scholar.google.com/citations?user=uyBJ6KIAAAAJ&hl=en)

## Overview report of the Shared Task 6

Title: [Overview of the NLPCC2024 Shared Task 6: Scientific Literature Survey Generation](https://link.springer.com/chapter/10.1007/978-981-97-9443-0_35)

## Publications from participants of the Shared Task 6

[Instruct Large Language Models to Generate Scientific Literature Survey Step by Step](https://link.springer.com/chapter/10.1007/978-981-97-9443-0_43)

[Cluster-Based Effective Generation of AI-Driven Literature Surveys](https://link.springer.com/chapter/10.1007/978-981-97-9443-0_37)

[Literature Hunter: Literature Reading Aided by Large Language Models](https://link.springer.com/chapter/10.1007/978-981-97-9443-0_29)

[Generation of Scientific Literature Surveys Based on Large Language Models (LLM) and Multi-Agent Systems (MAS)](https://link.springer.com/chapter/10.1007/978-981-97-9443-0_14)

