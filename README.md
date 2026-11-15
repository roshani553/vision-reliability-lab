# Vision Reliability Lab: Evaluating CLIP Under Image Degradation

## Overview

Vision Reliability Lab is an experimental project investigating how image degradation affects the recognition performance of CLIP (Contrastive Language-Image Pre-training), a vision-language model.

The project focuses on Gaussian blur as a form of image degradation and examines changes in prediction accuracy and confidence scores across different blur levels. It also includes a comparison between model predictions and human responses on a subset of images.

## Research Questions

- How does increasing Gaussian blur affect CLIP's image recognition accuracy?
- How do prediction confidence scores change under different blur conditions?
- How does CLIP's performance compare with human responses on the selected images?

## Methodology

The experiments were conducted using Python in Google Colab.

- Evaluated 30 images across seven Gaussian blur levels.
- Generated 210 image predictions using CLIP.
- Analysed prediction accuracy and confidence scores.
- Compared CLIP predictions with human responses across 24 images and five human participants.

## Key Findings

| Blur Radius | CLIP Accuracy |
|---|---:|
| 0 | 90.00% |
| 5 | 90.00% |
| 10 | 93.33% |
| 15 | 80.00% |
| 20 | 63.33% |
| 25 | 50.00% |
| 30 | 46.67% |

The highest observed accuracy was 93.33% at blur radius 10. At blur radius 30, accuracy decreased to 46.67%.

In the human comparison experiment:

- Human majority accuracy: 83.33%
- CLIP accuracy: 62.50%

These results are specific to the selected images, labels and experimental setup.

## Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- CLIP
- Google Colab
- Pandas
- Matplotlib
- Pillow

## Repository Contents

- `vision_reliability_lab.ipynb` – Main experimental notebook.
- `results/` – Experimental plots and visualisations, if included.
- `requirements.txt` – Python dependencies.

## Reproducibility

The notebook contains the experimental workflow, including image processing, CLIP inference, accuracy calculations and result analysis.

To reproduce the experiments:

1. Open the notebook in Google Colab or Jupyter Notebook.
2. Install the required dependencies.
3. Provide the image dataset used in the experiment.
4. Execute the notebook cells in order.

The original image dataset and human-response data may not be included in this repository. Results should therefore be interpreted in the context of the original experimental setup.

## Limitations

- The evaluation uses a relatively small image collection.
- Results depend on the selected images and candidate labels.
- Human comparison involved only five participants.
- Gaussian blur represents only one type of image degradation.
- The findings should not be generalised to all real-world images or vision tasks.

## Project Type

Independent experimental project exploring the reliability of vision-language models under image degradation.
