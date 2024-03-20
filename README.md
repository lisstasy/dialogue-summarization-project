# FLAN-T5 Dialogue Summarization Project

## Overview
This project utilizes FLAN-T5 from Hugging Face for dialogue summarization. The dialogues are sourced from the [DialogSum](https://huggingface.co/datasets/knkarthick/dialogsum) dataset, which consists of 10,000+ dialogues with manually labeled summaries and topics.

### 1. `1_summarize_dialogue.ipynb`
#### Generative AI: Summarize Dialogue

**Description:**
Explore dialogue summarization using generative AI. Compare zero shot, one shot, and few shot inferences to enhance generative output. Perform prompt engineering to direct the model.

**Table of contents:**
- Set up Kernel and Required Dependencies
- Summarize Dialogue without Prompt Engineering
- Summarize Dialogue with an Instruction Prompt
  - Zero Shot Inference with an Instruction Prompt
  - Zero Shot Inference with the Prompt Template from FLAN-T5
- Summarize Dialogue with One Shot and Few Shot Inference
- Generative Configuration Parameters for Inference

### 2. `2_fine_tune_generative_ai_model.ipynb`
#### Fine-Tune a Generative AI Model for Dialogue Summarization

**Description:**
Fine-tune FLAN-T5 for enhanced dialogue summarization. Evaluate results with ROUGE metrics. Explore Parameter Efficient Fine-Tuning (PEFT) for improved performance.

**Table of contents:**
- Set up Kernel, Load Required Dependencies, Dataset, and LLM
- Perform Full Fine-Tuning
- Perform Parameter Efficient Fine-Tuning (PEFT)

### 3. `3_fine_tune_model_to_detoxify_summaries.ipynb`
#### Fine-Tune FLAN-T5 with Reinforcement Learning (PPO) and PEFT to Generate Less-Toxic Summaries

**Description:**
Fine-tune FLAN-T5 to generate less toxic content using Meta AI's hate speech reward model. Utilize Proximal Policy Optimization (PPO) to reduce model toxicity.

**Table of contents:**
- Set up Kernel and Required Dependencies
- Load FLAN-T5 Model, Prepare Reward Model, and Toxicity Evaluator
- Perform Fine-Tuning to Detoxify the Summaries
