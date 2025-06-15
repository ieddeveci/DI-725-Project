# Parameter-Efficient Fine-Tuning of PaliGemma for Image Captioning

This repository contains the final project for the **Transformers and Attention-Based Deep Networks** course. 

The project focuses on enhancing the image captioning capabilities of **PaliGemma**, a vision-language model (VLM), through fine-tuning with the **RISC dataset**.

The primary goal is to improve the baseline performance of PaliGemma in generating image captions by:

- Applying **efficient fine-tuning strategies**, including parameter-efficient fine-tuning (PEFT) techniques.
- Performing **hyperparameter optimization** to identify effective training configurations.
- Integrating **evaluation metrics** that capture both linguistic fluency and visual-semantic alignment.

In the end, this project examined how parameter-efficient fine-tuning, specifically QLoRA applied solely to the language model components, can adapt the PaliGemma VLM for image captioning with minimal computational cost. Freezing the vision and projection modules, the study found that a lightweight configuration surpassed a more heavily parameterized one, indicating that scaling trainable parameters alone is insufficient without alignment to learning dynamics. Evaluation using BLEU, METEOR, and CLIPScore revealed mismatches between surface-level and semantic fidelity, demonstrating the importance of targeted prompting, decoding strategies, and varied evaluation metrics.
