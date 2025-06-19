# RuDialect-HTR: Handwritten Russian Dialectic Text Recognition using CRAFT/YOLO and TrOCR
**RuDialect-HTR** is a project focused on the detection and recognition of handwritten Russian dialectic texts using modern deep learning models.

## Repository Structure

This repository contains four Jupyter notebooks:

- `fine-tuning-craft` — fine-tuning the **CRAFT** model for text detection
- `fine-tuning-yolo` — fine-tuning **YOLO** for text detection
- `fine-tuning-trocr` — fine-tuning **TrOCR** for handwritten text recognition (HTR)
- `htr-pipeline` — full end-to-end HTR pipeline: text detection + recognition + output formatting

---

## Training Results

All training was performed in **Kaggle Notebooks** using free cloud GPUs.

| Model | Task                         | Notebook                                                                                                                                |
| ----- | ---------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| CRAFT | Text Detection               | [CRAFT: Russian Dialectic Text Detection](https://www.kaggle.com/code/daniilmatvienko/craft-russian-dialectic-text-detection/output)    |
| YOLO  | Text Detection               | [YOLO: Russian Dialectic Text Detection](https://www.kaggle.com/code/daniilmatvienko/yolo-russian-dialectic-text-detection)             |
| TrOCR | Handwritten Text Recognition | [TrOCR: Russian Dialectic HTR with PEFT (DoRA)](https://www.kaggle.com/code/daniilmatvienko/trocr-russian-dialectic-htr-with-peft-dora) |

> **Note:** These notebooks are demonstration versions (final experiment configurations). The original development notebooks are private and will not be published.

---

## Model Checkpoints

Fine-tuned model checkpoints are available on Hugging Face:

| Model                   | Hugging Face Link                                                                                                    |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------- |
| YOLO11x-dialectic       | [huggingface.co/Daniil-Domino/yolo11x-dialectic](https://huggingface.co/Daniil-Domino/yolo11x-dialectic)             |
| TrOCR-base-ru-dialectic | [huggingface.co/Daniil-Domino/trocr-base-ru-dialectic](https://huggingface.co/Daniil-Domino/trocr-base-ru-dialectic) |
| CRAFT                   | *Not published due to low performance* — weights available in Kaggle notebook output (see above).                    |

---

## Installation & Usage

If you're running **Kaggle notebooks listed above**, all required dependencies are already included in the environment.

For local or custom environments, install the dependencies manually using:

```bash
pip install -r requirements.txt --quiet
```
Tested with python version 3.10.18

---

## Contributors
[Matvienko Daniil](https://github.com/SaylesMand) - Machine Learning

[Starikov Alexander](https://github.com/ACherryJam) - Dataset Building, Backend