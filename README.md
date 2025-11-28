# image_and_text_categorizer

# 🛒 Product Categorization Using Deep Learning  
**Image-Based & Title-Based Category Prediction for Iranian E-commerce Items ([torob](https://torob.com/))**

---

## 📚 Overview

This repository contains two **Deep Learning pipelines** designed to automatically predict the **category ID** of products listed on **Torob**, a popular Iranian marketplace and price comparison platform.

These notebooks are parts of projects that I have done during my [Deep Learning Course](https://quera.org/certificate/lkxybXhn/).

The project investigates the categorization task from **two different perspectives**:

| Perspective | Input | Model Type | Output |
|------------|-------|-----------|--------|
| **Image Categorizer** | Product images | CNN-based Image Classifier | `category_id` |
| **Title Categorizer** | Product titles (Persian text) | NLP-based Text Classifier | `category_id` |

These two Jupyter notebooks show how computer vision and natural language processing techniques can independently learn product semantics to classify e-commerce items accurately.

---

## 🔍 Notebook 1 — `image_categorizer.ipynb`

### 🧠 Goal
Predict product categories using **only item images** from Torob.

### 🏗️ AI & Data Science Concepts
- **Deep Learning**
- **Convolutional Neural Networks (CNNs)**
- **Image feature extraction & classification**
- **Supervised learning**

### 🛠️ Key Libraries & Packages
| Package | Purpose |
|--------|---------|
| `numpy`, `pandas` | Data loading and manipulation |
| `keras` | CNN architecture design and training |
| `scikit-learn` | performance metric |

### 🚀 Steps Implemented
1. Load and preprocess product images  
2. Build CNN layers for feature extraction  
3. Train the model on category labels  
4. Evaluate performance on validation/test sets  
5. Predict `category_id` for unseen images  

### 🏁 Output
A trained **CNN classifier** that maps product images to correct categories.

---

## 📝 Notebook 2 — `title_categorizer.ipynb`

### 🧠 Goal
Predict product categories using **only Persian product titles**.

### 🏗️ AI & Data Science Concepts
- **Natural Language Processing (NLP)**
- **Text tokenization and embeddings**
- **Neural sequence models**
- **Deep learning for classification**

### 🛠️ Key Libraries & Packages
| Package | Purpose |
|--------|---------|
| `numpy`, `pandas` | Text data handling |
| `parsivar` | Persian text normalization and tokenization |
| `keras` | Text classification model training |
| `scikit-learn` | Metrics and evaluation |

### 🚀 Steps Implemented
1. Load product titles with category labels  
2. Clean and tokenize Persian text  
3. Convert tokens into vectors (embeddings)  
4. Train a neural text classifier  
5. Predict category IDs from new product titles  

### 🏁 Output
An NLP-based classifier capable of inferring **product categories from text alone**.

