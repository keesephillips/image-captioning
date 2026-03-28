# Applied Computer Vision: Image Captioning

Author: Keese Phillips

---

## Overview

This project implements an image captioning pipeline that generates natural language descriptions of images using deep learning. The system pairs a convolutional neural network encoder for visual feature extraction with a recurrent decoder that produces sequential text output, trained end-to-end on paired image-caption data. Caption quality is evaluated using standard NLP metrics including BLEU scoring via NLTK.

For a detailed discussion of the model architecture, training procedure, experimental results, and qualitative evaluation, refer to the [Project Report (PDF)](./project_4.pdf).

## Repository Structure

```
.
|-- README.md              Project documentation
|-- LICENSE                 MIT License
|-- requirements.txt       Python dependencies
|-- model.ipynb            Notebook used for training and testing the model
|-- project_4.pdf          Full project report with methodology and evaluation
|-- .gitattributes         Git line-ending configuration
```

## Environment

This project was developed on Windows with Python 3.x and the following core libraries.

**Deep Learning and Vision:**
- PyTorch 2.2.0 with TorchVision 0.20.1 and TorchAudio 2.5.1
- TorchText 0.15.2 for text preprocessing and vocabulary management
- TorchMetrics 1.6.0 for standardized evaluation metrics
- OpenCV 4.10.0 and scikit-image 0.24.0 for image processing

**NLP and Evaluation:**
- NLTK 3.9.1 for tokenization, BLEU scoring, and text utilities
- Regex 2024.11.6 for text normalization

**Data and Utilities:**
- KaggleHub 0.3.4 for dataset access
- Pandas 2.2.3 and NumPy 1.26.4 for data handling
- Matplotlib 3.9.3 and Seaborn 0.13.2 for visualization
- Streamlit 1.40.2 for interactive demonstration
- LIME 0.2.0.1 for model interpretability

The full dependency list is available in `requirements.txt`.

## Setup

Clone the repository and install the required packages inside a virtual environment.

```bash
git clone https://github.com/<your-username>/applied-cv-project-4.git
cd applied-cv-project-4

python -m venv venv
venv\Scripts\activate        # Windows
# source venv/bin/activate   # macOS / Linux

pip install -r requirements.txt
```

Note that `requirements.txt` reflects the complete development environment and includes packages beyond the strict project dependencies. A minimal installation covering PyTorch, TorchVision, TorchText, NLTK, OpenCV, and Matplotlib is sufficient to run the core pipeline.

## Attribution

This project references and builds upon material from [Modern Computer Vision with PyTorch](https://github.com/PacktPublishing/Modern-Computer-Vision-with-PyTorch) by Packt Publishing.

## License

This project is released under the [MIT License](./LICENSE). Copyright (c) 2024 Keese Phillips.
