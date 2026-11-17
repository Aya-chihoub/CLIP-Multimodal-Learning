# CLIP Multimodal Learning

TP de M2 VMI — Multimodalité et IA générative, Université Paris Cité.

Experiments with CLIP on natural and medical images, based on the [course tutorial](https://github.com/ckurtz/teaching_UPC_UFRMI/blob/main/CLIP_tutorial_(with_medical_images_ROCO).ipynb).

## Experiments

- Image–text similarity on natural images and ROCO medical images
- Comparison of RN50, ViT-B/32 and ViT-B/16 on 100 ROCO pairs
- Examples of correct and incorrect medical-caption retrieval
- Zero-shot classification on 1,000 CIFAR-10 images (10 classes)
- Illustration of medical CLIP before and after fine-tuning

## Results

**ROCO — image-to-text retrieval (100 pairs)**

| Model | Top-1 (%) | Top-5 (%) |
| --- | ---: | ---: |
| RN50 | 19.0 | 48.0 |
| ViT-B/32 | 17.0 | 47.0 |
| ViT-B/16 | 23.0 | 53.0 |

**CIFAR-10 — zero-shot classification (1,000 images)**

| Model | Accuracy (%) |
| --- | ---: |
| RN50 | 69.3 |
| ViT-B/32 | 88.9 |
| ViT-B/16 | 88.1 |

## Run

Open [CLIP_TP_solutions.ipynb](CLIP_TP_solutions.ipynb) in Google Colab with a GPU runtime. Install the CLIP package and mount Google Drive. The ROCO dataset and the medical fine-tuning checkpoint are provided separately for the course and are not included in this repository.

The training cell is optional; the supplied checkpoint can be used for the fine-tuned demonstration.
