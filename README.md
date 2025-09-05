
# Cyberbullying Detection Using SVC

This project is designed to detect cyberbullying in social media comments using a machine learning model (Support Vector Classifier - SVC). The application uses two Graphical User Interfaces (GUIs): the first for uploading a dataset and training the model, and the second for analyzing new comments.

---

##  Prerequisites

Before running the project, make sure the following are installed:

- Python 3.x
- `pandas`
- `scikit-learn`
- `tkinter` (usually included with Python)

To install required packages, run:

```bash
pip install pandas scikit-learn
```

---

##  Dataset Requirements

The dataset should be in **CSV format** with the following columns:

- **Text** – the comment
- **CB_Label** – label (0 for non-cyberbullying, 1 for cyberbullying)

Example:

| Text                      | CB_Label |
|--------------------------|----------|
| You are stupid           | 1        |
| Hope you do well in life | 0        |

---

##  How to Execute

### Step 1: Run the Python File

Run the script using:

```bash
python cyberbullying_gui.py
```

---

### Step 2: First GUI – Upload and Train

- A GUI window opens titled **“Cyberbullying Detection – Upload Dataset”**.
- Click **“Upload”** and select the CSV file.
- Click **“Train”** to train the model (takes ~10 seconds).
- A message box appears: *“Model has been trained successfully. Redirecting to detection window.”*
- First GUI closes and second GUI opens.

---

### Step 3: Second GUI – Analyze Comments

- New GUI opens titled **“Cyberbullying Detection Using SVC”**.
- Enter a comment in the text box.
- Click **“Analyze”**.
- Output:
  - *“Cyberbullying Detected!”* (in red)
  - *“No Cyberbullying Detected.”* (in green)

---

##  Notes

- Training is required once after launching.
- TF-IDF and SVC are used, not keyword matching.
- Second GUI won’t work until training is done.

---

##  Example Use Case

- Upload dataset and train the model.
- Input: *“You’re worthless and ugly.”*
- Output: *Cyberbullying Detected!*

---

##  Tips

- Ensure correct CSV format before uploading.
- Don’t close GUI until success message shows.
- Use clean, labeled data for best accuracy.
