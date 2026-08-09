## Plasmo3Net: A Convolutional Neural Network-Based Algorithm for Detecting Malaria Parasites in Thin Blood Smear Images
![App Screenshot](logo/header.png)

### Live Demo
[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://plasmo3net.streamlit.app/)

### *[Article](https://www.biorxiv.org/content/10.1101/2024.12.12.628235v1.full)*
### Authors
[Afolabi Owoloye<sup>1,2,3</sup>](https://www.linkedin.com/in/afolabi-owoloye-a1b8a5b5/)
[Funmilayo Ligali<sup>1,3</sup>](https://www.linkedin.com/in/samuel-olawale-olubode-6191a81aa/)
[Ojochenemi Enejoh<sup>4</sup>](https://www.linkedin.com/in/adewale-ogunleye-09029684/)
[Oluwafemi Agosile<sup>1</sup>](https://www.linkedin.com/in/samuel-olawale-olubode-6191a81aa/)
[Adesola Musa<sup>3</sup>](https://www.linkedin.com/in/adewale-ogunleye-09029684/)
[Oluwagbemiga Aina<sup>3</sup>](https://www.linkedin.com/in/adewale-ogunleye-09029684/)
[Adetunji Adewole<sup>5</sup>](https://scholar.google.com/citations?user=VF3nzuYAAAAJ&hl=en&oi=ao)
[Taiwo Idowu<sup>2</sup>](https://scholar.google.com/citations?hl=en&user=ViS6ndQAAAAJ)
[Kolapo Oyebola<sup>1,3</sup>](https://www.linkedin.com/in/kolapo-oyebola-phd-67493836/)

[<sup>1</sup>Centre for Genomic Research in Biomedicine (CeGRIB), College of Basic and Applied Sciences, Mountain Top University, Ibafo, Nigeria.</sup>](https://www.linkedin.com/company/81576850/admin/dashboard/)<br>
<sup>2</sup> Parasitology and Bioinformatics Unit, Department of Zoology, Faculty of Science, University of Lagos, Lagos, Nigeria.<br>
<sup>3</sup> Nigerian Institute of Medical Research, Lagos, Nigeria.<br>
<sup>4</sup> Genetics, Genomics and Bioinformatics Department, National Biotechnology Research and Development Agency, Abuja, Nigeria. <br>
<sup>5</sup> Computer Science Department, Faculty of Science, University of Lagos, Lagos, Nigeria
<br>
<br>
<br>

<img width="880" height="680" alt="image" src="https://github.com/user-attachments/assets/e1fb7d4e-f747-4643-8ac3-fcabeace6feb" />

### Figure 1.0: Experimental workflow for developing the convolutional neural network

# 🦟 Plasmo3Net: Malaria Detection Web App

A deep learning-powered web application for automated detection of *Plasmodium falciparum* in red blood cells (RBCs) using convolutional neural networks (CNNs). Achieves **99.3% accuracy** in classifying infected vs. uninfected cells.

## 🔍 Features

- **Cell Segmentation**: Extracts individual RBCs from microscope slide images using OpenCV.
- **CNN Classification**: 
  - Custom **Plasmo3Net** model (13-layer CNN) with 99.3% accuracy.
  - Benchmarked against ResNet50, InceptionV3, VGG16, and AlexNet.
- **User-Friendly Interface**:
  - Upload microscope slides or pre-segmented RBCs.
  - Real-time predictions with visual results.
  - Download segmented cells as a ZIP file.

## 📊 Performance Metrics
| Metric       | Plasmo3Net | ResNet50 (Baseline) |
|--------------|------------|---------------------|
| Accuracy     | 99.3%      | 97.9%               |
| Precision    | 99.1%      | 97.6%               |
| Recall       | 99.6%      | 98.3%               |
| F1 Score     | 99.3%      | 97.9%               |

## 🚀 Quick Start

### Prerequisites
- Python 3.8+
- TensorFlow 2.x
- Streamlit
- OpenCV

```markdown
### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/CeGRIB/plasmo3net.git 
   cd plasmo3net
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the app:
   ```bash
   streamlit run app.py
   ```

4. Access the app at `http://localhost:8501`.

## 🧩 Workflow.
1. **Upload**: Microscope slide image or segmented RBCs.
2. **Segment**: Automated RBC extraction (if using slides).
3. **Classify**: Predicts "Parasitized" or "Uninfected" for each cell.
4. **Results**: Displays predictions with confidence metrics.

## 📂 File Structure
```
.
├── app.py                # Streamlit application
├── model.h5              # Trained Plasmo3Net model
├── requirements.txt      # Dependencies
├── script/               # python scripts
├── RBC/                  # Processed RBC images
└── logo/                 # App assets
```

## 📄 Citation
If you use this work, please cite:
```bibtex
@article{
  authors={Owoloye et al.},
  title={Plasmo3Net: A Convolutional Neural Network-Based Algorithm for Detecting Malaria Parasites in Thin Blood Smear Images},
  journal={bioRxiv},
  year={2024},
  doi={10.1101/2024.12.12.628235v1}
}
```

## 🤝 Contribute
- Report bugs via [Issues](https://github.com/cegrib/plasmo3net/issues).
- Fork and submit Pull Requests.

## 📧 Contact
CeGRIB - [@cegrib](https://www.linkedin.com/company/cegrib/?viewAsMember=true)
[LinkedIn](https://www.linkedin.com/company/cegrib/?viewAsMember=true) | [Twitter](https://x.com/CeGRIB_)
```
