# awesome-ai4ms-paper-and-websites

This repository is a collection of my thoughts, summaries, and reflections on literature, websites, and tutorials that explore the intersection of materials science and artificial intelligence.

## Directory
- [Preface](#preface)
- [LLM + Materials](#llm--materials)
  - [RAG](#rag)
  - [Agent](#agent)
  - [Knowledge distillation](#knowledge-distillation)
- [Materials with AI](#materials-with-ai)
  - [Properties Prediction](#properties-prediction)
  - [Knowledge Extraction](#knowledge-extraction)
- [Benchmark and Database](#benchmark-and-database)
  - [Materials Benchmark or Database](#materials-benchmark-or-database)
  - [AI-related Benchmark or Database](#ai-related-benchmark-or-database)

# Preface

本仓库记录关于LLM (large language models)和AI/ML在材料科学中应用的文献，特别是关于LLM在材料中的应用。看过的文章会至少用一句话概括内容，有些还会有notes。只有标题的就是还没看过的，只是先存档到这里。

# LLM + Materials

## RAG
None

## Agent
None

## Knowledge distillation
1. 从零开始实现大模型知识蒸馏 -- Starting from scratch to achieve knowledge distillation of large models (Bilibili video Jan 2025) [[Link]](https://www.bilibili.com/video/BV1kQcoetEFM/?spm_id_from=333.1007.top_right_bar_window_custom_collection.content.click&vd_source=4c43a44b540724d9ab77627ff3efb406) 使用qwen2.5系列模型在特定任务上进行知识蒸馏，教师模型为qwen2.5-3b（qwen2.5-7b），学生模型为qwen2.5-0.5b，尝试只使用KL散度、微调学生模型加KL散度和不微调学生模型加交叉熵加KL散度等不同思路，并且使用了KL散度不同变种（反向KL散度，偏向前向KL散度，偏向反向KL散度）。反向 K2 散度优于前向 K2 散度,但仅仅微调学生模型准确度反而最好为80.3%。

# Materials with AI
## Properties Prediction
None

## Knowledge Extraction
1. Bridging AI and Science: Implications from a Large-Scale Literature Analysis of AI4Science (Arxiv Nov 2024) [[Paper]](https://arxiv.org/pdf/2412.09628) 大规模(159,295 papers)AI4S文献摘要分析。磁性材料，锂离子电池，钙钛矿太阳能电池是AI融合比较缺乏的领域。作者用文献训练了节点之间的link预测模型，传统的Node2Vec方法比较适合分析AI和Sci领域是否可能产生连接。

## Crystal structure
1. Progress in Deep Learning Crystal Structure Generation (Github repo) [[Link]](https://github.com/kdmsit/Awesome-Crystal-GNNs/tree/main)

# Benchmark and Database
- ## Materials Benchmark or Database
  | Name | Description | Link | Category |
  |---|---|---|---|
  | perovskitedatabase  | perovskitedatabase | https://github.com/Grenzlinie/perovskitedatabase | perovskite |
  | dlmatreview | software packages and databases used in deep-learning applications for materials science and engineering | https://github.com/deepmaterials/dlmatreview | 材料科学数据库和软件github仓库 |


- ## AI-related Benchmark or Database
  | Name | Description | Link | Category |
  |---|---|---|---|
  | SciAssess | Benchmarking LLM Proficiency in Scientific Literature Analysis | https://arxiv.org/abs/2403.01976 | 材料文本问答数据库 |
  | SciQAG | A Framework for Auto-Generated Science Question Answering Dataset with Fine-grained Evaluation | https://arxiv.org/abs/2405.09939 | 材料文本问答数据库 |
  | HoneyComb | A Flexible LLM-Based Agent System for Materials Science | https://aclanthology.org/2024.findings-emnlp.192/ | 材料Agent数据库 |
  | Bohrium | DeepMD and AI4S notebook square | https://bohrium.dp.tech/notebooks?notebookTab=recommendations | AI4S知识分享平台 |
  | LLM4Mat-Bench | Benchmarking Large Language Models for Materials Property Prediction | https://arxiv.org/abs/2411.00177 | LLM在材料科学知识的回答表现 |
  | MaScQA | investigating materials science knowledge of large language models | https://pubs.rsc.org/en/content/articlelanding/2024/dd/d3dd00188a | LLM在材料科学知识的回答表现 |