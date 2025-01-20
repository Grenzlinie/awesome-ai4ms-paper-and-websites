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
  - [Multi-modal MatLLM](#multi-modal-matllm)

# Preface

本仓库记录关于LLM (large language models)和AI/ML在材料科学中应用的文献，特别是关于LLM在材料中的应用。看过的文章会至少用一句话概括内容，有些还会有notes。只有标题的就是还没看过的，只是先存档到这里。

# LLM + Materials

## RAG

2025

## Agent

2025

## Knowledge distillation

2025
1. 从零开始实现大模型知识蒸馏 -- Starting from scratch to achieve knowledge distillation of large models (Bilibili video Jan 2025)[[Link]](https://www.bilibili.com/video/BV1kQcoetEFM/?spm_id_from=333.1007.top_right_bar_window_custom_collection.content.click&vd_source=4c43a44b540724d9ab77627ff3efb406) 使用qwen2.5系列模型在特定任务上进行知识蒸馏，教师模型为qwen2.5-3b（qwen2.5-7b），学生模型为qwen2.5-0.5b，尝试只使用KL散度、微调学生模型加KL散度和不微调学生模型加交叉熵加KL散度等不同思路，并且使用了KL散度不同变种（反向KL散度，偏向前向KL散度，偏向反向KL散度）。反向 K2 散度优于前向 K2 散度,但仅仅微调学生模型准确度反而最好为80.3%。

# Materials with AI
## Properties Prediction

2024

## Knowledge Extraction

2024
1. Bridging AI and Science: Implications from a Large-Scale Literature Analysis of AI4Science (Arxiv Nov 2024)[[Paper]](https://arxiv.org/pdf/2412.09628) 大规模(159,295 papers)AI4S文献摘要分析。磁性材料，锂离子电池，钙钛矿太阳能电池是AI融合比较缺乏的领域。作者用文献训练了节点之间的link预测模型，传统的Node2Vec方法比较适合分析AI和Sci领域是否可能产生连接。

# Benchmark and Database
## Multi-modal MatLLM

2024

- ## Materials Benchmark or Database
  | Paper Name | Categories | Link or DOI |
  |---|---|---|
  |  |  |  |

- ## AI-related Benchmark or Database
  | Paper Name | Categories | Link or DOI |
  |---|---|---|
  |  |  |  |