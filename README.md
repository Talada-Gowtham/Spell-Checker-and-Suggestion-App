# 🔤 Spell Checker and Suggestion App

A Python-based Information Retrieval project that helps users identify misspelled words, generate spelling suggestions, refine recommendations, and provide feedback through an interactive user interface.

---

## 📖 Introduction

The **Spell Checker and Suggestion App** is a Python application designed to assist users in verifying the spelling of words and discovering possible correct alternatives.

The application utilizes **N-Grams** and **Ranking Algorithms** to generate, rank, and refine spelling suggestions. Users can further provide ratings and feedback, helping evaluate the quality of generated suggestions.

---

## 🚀 Features

* ✅ Spell checking using a predefined dataset
* ✅ Generates up to **30 spelling suggestions**
* ✅ Suggestion refinement based on word patterns
* ✅ Interactive GUI built using Tkinter
* ✅ User rating system (1–5 stars)
* ✅ Feedback and remarks collection
* ✅ Automatic storage of reviews and feedback

---

## 📋 Prerequisites

Before running the application, ensure the following are installed:

* Python 3.x
* Required Python packages:

  * tkinter
  * tabulate

---

## ⚙️ Installation

### Step 1: Clone the Repository

```bash
git clone <repository-url>
cd Spell-Checker-and-Suggestion-App
```

### Step 2: Install Dependencies

```bash
pip install tk tabulate
```

---

## ▶️ Running the Application

Execute the following command:

```bash
python code.py
```

After execution:

1. The **Spell Suggestion App** window will open.
2. Enter a word to search.
3. Enter the number of suggestions required (maximum 30).
4. Click **Get Suggestions**.

---

## 🖥️ How the Application Works

### Scenario 1: Correctly Spelled Word

1. Enter a word.
2. Click **Get Suggestions**.
3. If the word exists in the dataset:

   * The application displays that the word is correctly spelled.
   * You can directly provide a rating.

---

### Scenario 2: Misspelled Word

1. Enter a word that is not present in the dataset.
2. Specify the number of suggestions required.
3. Click **Get Suggestions**.
4. The application generates relevant spelling suggestions.

---

### Suggestion Refinement Process

After suggestions are displayed:

#### If You Are Satisfied

* Click **Yes**
* Provide a rating between **1 and 5**

#### If You Are Not Satisfied

* Click **No**
* The application asks whether you want to refine the suggestions

##### If You Choose to Refine

* Click **Yes**
* Suggestions are refined based on:

  * First letter of the entered word
  * Last letter of the entered word
* A new list of modified suggestions is generated

After refinement:

* If satisfied → Give a rating
* If not satisfied → Give a rating and provide remarks/feedback

##### If You Do Not Want Refinement

* Click **No**
* Directly provide a rating

---

## 📝 Feedback & Review System

The application automatically records user feedback.

### Review Storage

All ratings are saved in:

```text
Review.txt
```

### Remarks Storage

If a rating is **3 stars or below**, additional remarks and feedback are stored in:

```text
remarks.txt
```

---

## 📂 Project Files

| File          | Description                                     |
| ------------- | ----------------------------------------------- |
| `code.py`     | Main application source code                    |
| `dataset.txt` | Dataset used for spell checking and suggestions |
| `Review.txt`  | Stores user ratings                             |
| `remarks.txt` | Stores user feedback and remarks                |

---

## 📊 Technologies Used

* Python
* Tkinter
* Tabulate
* N-Gram Techniques

---

## 📥 Dataset Download

Dataset Link:

https://drive.google.com/file/d/178SguEiFbGunHZ32wrPjLn7hWXCY3gwg/view?usp=drive_link

