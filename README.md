# Week‑11 Internship Projects — 😷 Face Mask Detection & 📊 Customer Segmentation

Take it smart (OPC) Private Limited — Data Science Internship (Week‑11, 18‑4‑26)

Summary 📌
-------
This repository contains two complementary machine learning projects demonstrating practical applications of supervised deep learning and unsupervised clustering:

- **Face Mask Detection** — CNN-based image classifier to detect whether a person is wearing a mask. 😷
- **Customer Segmentation** — K‑Means clustering on customer purchasing behavior to discover actionable segments. 📊

Each project is provided as a Jupyter notebook with end‑to‑end steps: data loading, preprocessing, model training, evaluation, and visualizations.

Project highlights ✨
------------------

- Face Mask Detection (Computer Vision) 🤖:
  - CNN architecture using `Conv2D`, `MaxPooling2D`, `Flatten`, `Dense`, and `Dropout` layers.
  - Data augmentation (rotation, shifts, flips) and standard preprocessing for robustness.
  - Evaluation with confusion matrix and classification report. Reported overall test accuracy: **91.89%**.
  - Brief metrics (see notebook for full details):
    - With Mask — Precision: 0.87, Recall: 0.98, F1: 0.92
    - Without Mask — Precision: 0.98, Recall: 0.86, F1: 0.91

- Customer Segmentation (Unsupervised Learning) 🛍️:
  - Exploratory Data Analysis on `annual_income`, `purchase_amount`, `purchase_frequency`, and `loyalty_score`.
  - Feature scaling using `StandardScaler` and Elbow method to select `K` (K = 4).
  - K‑Means clustering to produce actionable segments for targeted marketing.

Repository structure 🗂️
--------------------

Top-level layout:

- `Face Mask Detection using CNN/`
  - `Face_Mask_Detection_using_CNN.ipynb`
  - `Input images/` 
  - `Output snapshots/` 
  - `Screen recording/` 
- `Customer Segmentation using K-Means Clustering/`
  - `Customer_Segmentation_using_K_Means_Clustering.ipynb`
  - `Dataset/` 
  - `Output snapshots/` 
  - `Screen recording/` 
- `README.md` 
- `Task5.pdf` (project/task reference)

Quick start 🚀
-----------

1. Create and activate a virtual environment (example):

```bash
python 3.8 -m venv .venv
# Windows PowerShell
.venv\\Scripts\\Activate.ps1
# macOS / Linux
source .venv/bin/activate
```

2. Install recommended libraries (create `requirements.txt` as needed):

```bash
pip install numpy pandas scikit-learn matplotlib seaborn jupyter tensorflow opencv-python
```

3. Open the notebook you want to run (VS Code or Jupyter):

```bash
jupyter notebook
```

Notes for reproducibility 📝
-------------------------

- Place the face images under `Face Mask Detection using CNN/Input images/` and the customer CSV under `Customer Segmentation using K-Means Clustering/Dataset/` before running notebooks.
- For consistent K‑Means results, use `random_state=42` when creating the `KMeans` instance.
- If training on CPU, consider reducing batch size or image size to lower memory use.

Output snapshots 🖼️
----------------
- Face Mask Detection:
  - Confusion Matrix and Classification Report:
<img width="632" height="732" alt="Screenshot 2026-05-09 162721" src="https://github.com/user-attachments/assets/f65df685-66e0-427e-8eca-243dddebe49e" />
  - Output : Mask
<img width="623" height="444" alt="Screenshot 2026-05-09 162747" src="https://github.com/user-attachments/assets/22d8f0e4-fd32-425e-8f63-6230ca13f118" />
  - Output : No Mask
<img width="602" height="442" alt="Screenshot 2026-05-09 162756" src="https://github.com/user-attachments/assets/91bd01aa-2c01-4fe4-a483-631279ff6bf5" />

- Customer Segmentation:
  - Univariate and Bivariate analysis
<img width="920" height="546" alt="Screenshot 2026-05-09 162813" src="https://github.com/user-attachments/assets/ed54b44d-f1b7-4fe6-a1b0-3e7c5b58467c" />
  - Plot using Elbow method for optimal K
<img width="661" height="751" alt="Screenshot 2026-05-09 162911" src="https://github.com/user-attachments/assets/7ed4090a-46e8-4310-be3b-5c14eb68bd37" />

Project Explanation Video 🎥
-------------------------
- Face Mask Detection:
https://github.com/user-attachments/assets/85767011-5e61-4ef0-bee5-35f11ecd7b35
  
- Customer Segmentation:
https://github.com/user-attachments/assets/17e2319e-c8ae-44c1-962e-f7609060b434

Project results (short) ✅
----------------------

- Face Mask Detection — Overall test accuracy: **91.89%**; strong masked‑class recall (0.98).
- Customer Segmentation — K = 4 discovered distinct groups useful for targeted campaigns (see notebook cluster summaries).

Contact & repository 🔗
--------------------

GitHub: https://github.com/Umesh-L/Week-11_Assignment_18-5-26-Face_Mask_Det.--Customer_Segmentation-DataScience_Internship-TakeItSmart

For questions, open an issue in the repository or contact the author via the GitHub profile.

Acknowledgements 🙏
----------------

Thanks to Take it smart (OPC) Private Limited for the internship opportunity and access to datasets and guidance during these projects.

