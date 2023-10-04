---
base_model: NousResearch/Llama-2-7b-hf
tags:
- generated_from_trainer
model-index:
- name: qlora-out
  results: []
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

[<img src="https://raw.githubusercontent.com/OpenAccess-AI-Collective/axolotl/main/image/axolotl-badge-web.png" alt="Built with Axolotl" width="200" height="32"/>](https://github.com/OpenAccess-AI-Collective/axolotl)
# qlora-out

This model is a fine-tuned version of [NousResearch/Llama-2-7b-hf](https://huggingface.co/NousResearch/Llama-2-7b-hf) on the None dataset.
It achieves the following results on the evaluation set:
- Loss: 0.0014

## Model description

More information needed

## Intended uses & limitations

More information needed

## Training and evaluation data

More information needed

## Training procedure

### Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 0.0002
- train_batch_size: 2
- eval_batch_size: 2
- seed: 42
- distributed_type: multi-GPU
- num_devices: 2
- gradient_accumulation_steps: 4
- total_train_batch_size: 16
- total_eval_batch_size: 4
- optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- lr_scheduler_type: cosine
- lr_scheduler_warmup_steps: 10
- num_epochs: 1

### Training results

| Training Loss | Epoch | Step | Validation Loss |
|:-------------:|:-----:|:----:|:---------------:|
| 0.4383        | 0.05  | 20   | 0.0220          |
| 0.1339        | 0.1   | 40   | 0.0150          |
| 0.1871        | 0.14  | 60   | 0.0143          |
| 0.1794        | 0.19  | 80   | 0.0005          |
| 0.1591        | 0.24  | 100  | 0.0082          |
| 0.1309        | 0.29  | 120  | 0.0079          |
| 0.1372        | 0.33  | 140  | 0.0075          |
| 0.1633        | 0.38  | 160  | 0.0008          |
| 0.2095        | 0.43  | 180  | 0.0072          |
| 0.2859        | 0.48  | 200  | 0.0003          |
| 0.131         | 0.52  | 220  | 0.0049          |
| 0.1869        | 0.57  | 240  | 0.0046          |
| 0.1786        | 0.62  | 260  | 0.0016          |
| 0.1802        | 0.67  | 280  | 0.0014          |
| 0.1754        | 0.72  | 300  | 0.0005          |
| 0.1316        | 0.76  | 320  | 0.0017          |
| 0.1233        | 0.81  | 340  | 0.0021          |
| 0.1719        | 0.86  | 360  | 0.0023          |
| 0.1278        | 0.91  | 380  | 0.0016          |
| 0.1631        | 0.95  | 400  | 0.0014          |


### Framework versions

- Transformers 4.35.0.dev0
- Pytorch 2.0.1+cu118
- Datasets 2.14.5
- Tokenizers 0.14.0
