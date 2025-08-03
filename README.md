# LLMUsefulnessLabels
A repository for codes curated to create LLM generated usefulness labels with pre-trained (prompt) and finetuned LLM models.

**Abstract:** In the information retrieval (IR) domain, evaluation plays a crucial role in optimizing search experiences and supporting diverse user intents. In the recent LLM era, research has been conducted to automate document relevance labels. These labels have traditionally been assigned by crowd-sourced workers, a process that is both time consuming and costly. This study focuses on LLM-generated usefulness labels, a crucial evaluation metric that considers the user’s search intents and task objectives, an aspect where relevance falls short. Our experiment utilizes task-level, query-level and document-level features along with user search behavior signals, which are essential in defining the usefulness of a document. Our research finds that (i) pre-trained LLMs can generate moderate usefulness labels by understanding the comprehensive search task session, and (ii) pre-trained LLMs perform better judgment in short search sessions when provided with search session contexts. Furthermore, we investigate whether LLMs can capture the unique divergence between relevance and usefulness, along with conducting an ablation study to identify the most critical metrics for accurate usefulness label generation. In conclusion, this work explores LLM-generated usefulness labels by evaluating critical metrics and optimizing for practicality in real-world settings.

Short Paper: https://arxiv.org/pdf/2503.08965 (accepted at SIGIR 2025 Padova, Italy)

Full Paper: https://arxiv.org/pdf/2504.14401 (preprint under review)

# Finetuning for Usefulness Labels

This finetuned model code repo has been created as part of an experiment for finetuning LLMs on user search behavior signals to predict usefulness labels. The finetuning has been conducted on the dataset THUIR KDD'19 and details of the project can be found in our paper **'LLM-Driven Usefulness Labeling for IR Evaluation'**:
https://arxiv.org/abs/2503.08965.

- **Developed by:** Mouly Dewan (University of Washington)
- **Shared by:** Mouly Dewan
- **Model type:** Llama
- **Finetuned from model:** Meta-Llama-3.1-8B-Instruct
- **Finetuned Dataset:** [Finetuned_THUIR_Dataset](https://huggingface.co/datasets/moulydewan/THUIR_finetune_dataset)
- **Finetuned Model:** [Finetuned_THUIR_Model](https://huggingface.co/moulydewan/Llama-3.1-8B-Instruct-Finetuned-THUIR)

