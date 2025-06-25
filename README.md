# 🐦 Bird Species Classification with Deep Learning and Sound Display

Project by **Fadia Boudiaf & Herkat Wifak** — Module IMN (Traitement d'image), Groupe SIQ1.

This project classifies bird species from images using deep learning techniques (CNN / transfer learning) and enhances the user experience by **displaying the corresponding bird call** for the predicted species.

---

## What it does

- Takes an image of a bird as input
- Predicts its species using a fine-tuned ResNet model (trained on the **[Kaggle 200 Bird Species](https://www.kaggle.com/datasets/kedarsai/bird-species-classification-220-categories)** dataset)
- Searches for and plays a **bird call sound** from external sources ([Xeno-Canto](https://xeno-canto.org))

---

## Files included

- `bird_classification.ipynb` – Main notebook with model loading, prediction, and sound playback.
- `README.md` – Project documentation.

---
# Model
The notebook uses **ResNet-18** as a backbone, fine-tuned in two phases:

- Feature extraction (freezing the backbone)

- Full fine-tuning (gradually unfreezing layers)

The model is trained on [the 200 Bird Species dataset from Kaggle](https://www.kaggle.com/datasets/kedarsai/bird-species-classification-220-categories)

---

# Audio Integration
The model links predictions to **the Xeno-Canto API** and plays back the sound of the predicted bird using:

- requests for querying the API

- pydub and simpleaudio for audio playback

- IPython.display to embed audio in notebooks (Google Colab-compatible)

---
### 🔗 Download the trained model

You can download the trained model file here:  
📥 [best_model_final.pth (Google Drive File)](https://drive.google.com/file/d/1CYnerIBOQLwc3N7G6EdGKK3l0yGQVRY3/view?usp=drive_link)
you find here info about the model :
📥 [Bird_Model (Google Drive Folder)](https://drive.google.com/drive/folders/1yvfD1v39LlubdYMmf-BExVP2ugMYQ-VB?usp=drive_link)
---

# Authors
- **Fadia Boudiaf**  
  [lf_boudiaf@esi.dz](mailto:lf_boudiaf@esi.dz)

- **Herkat Wifak**  
  [lw_herkat@esi.dz](mailto:lw_herkat@esi.dz)

***Module IMN – Traitement d'image numérique***
***Groupe SIQ1***
***ESI (École nationale supérieure d'informatique)***

  
