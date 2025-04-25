# Clinical-R1: Reinforcement Learning for Clinical Decision-Making with Large Language Models

This project explores how to use **Group Relative Policy Optimization (GRPO)** to train a large language model (LLM) to make clinical decisions using patient history and simulated SQL-based information retrieval. The model can either diagnose based on initial notes or retrieve more information before answering.

## What This Project Does

- Uses reinforcement learning (GRPO) to fine-tune an LLM for **clinical reasoning**
- Fine-tunes small-scale open-source LLMs using **consumer GPUs** with [Unsloth](https://github.com/unslothai/unsloth)
- Evaluates models on a labeled subset of [MIMIC-IV-Ext-CDM](https://physionet.org/content/mimic-iv-ext-cdm/1.1/)


## Technologies Used

- [Unsloth](https://github.com/unslothai/unsloth) for QLoRA fine-tuning
- [Hugging Face GRPO trainer](https://github.com/huggingface/trl)
- DuckDB for executing SQL queries in reward functions

## Future Work

- Support turn-based function calling within Unsloth
- Add cost-sensitive reward shaping (e.g., penalize unnecessary lookups)
- Improve reward function robustness to prevent gaming

## Citation

If you found this helpful or build upon it, please cite the relevant original datasets and GRPO papers.

## Related Work

- [Search-R1 (Jin et al. 2025)](https://arxiv.org/abs/2503.09516)
- [Med-R1 (Lai et al. 2025)](https://arxiv.org/abs/2503.13939)
- [MedVLM-R1 (Pan et al. 2025)](https://arxiv.org/abs/2502.19634)


