**FashionMNIST Similarity Search 🔍**
=====================================

**📌 Overview**
---------------

This project implements multiple **image similarity search methods** on the **FashionMNIST dataset**, leveraging deep learning and traditional similarity search techniques. The goal is to efficiently find visually similar images from a gallery dataset using various feature extraction techniques.

**📊 Methods Implemented**
--------------------------

1.  **Feature Extraction using Pre-trained CNNs**

    -   Uses deep CNNs like **ResNet, VGG, or EfficientNet** to extract meaningful features.
    -   Nearest neighbor search is performed using **k-NN or Cosine Similarity**.
2.  **Deep Metric Learning (Siamese Network)**

    -   Employs a **Siamese Network** trained with **Contrastive Loss** or **Triplet Loss**.
    -   Learns embeddings to measure pairwise image similarity.
3.  **Vision Transformers (ViTs) & CLIP-based Embeddings**

    -   Utilizes **ViTs or CLIP** to generate visual embeddings.
    -   Computes similarity using nearest neighbor techniques.
4.  **Hashing-based Search (LSH - Locality Sensitive Hashing)**

    -   Encodes images into hash codes for **efficient similarity search**.
    -   Uses **LSH & k-d Tree for fast retrieval**.
5.  **Autoencoder-based Image Embeddings**

    -   Uses **Autoencoders** to learn compact feature representations.
    -   Performs similarity search using **Euclidean or Cosine distance**.

**🛠️ Setup & Installation**
----------------------------

### **1️⃣ Clone the Repository**

bash

CopyEdit

`git clone https://github.com/AnirudhGupta007/FashionMNIST-Similarity-Search.git
cd FashionMNIST-Similarity-Search`

### **2️⃣ Create a Virtual Environment (Optional but Recommended)**

bash

CopyEdit

`python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate`

### **3️⃣ Install Dependencies**

bash

CopyEdit

`pip install -r requirements.txt`

**🚀 Usage**
------------

### **Training & Feature Extraction**

-   Run different methods using the corresponding Jupyter notebooks:
    -   `method_1.ipynb` → CNN-based Feature Extraction
    -   `method_2.ipynb` → Siamese Network
    -   `method_3.ipynb` → Vision Transformers & CLIP
    -   `method_4.ipynb` → Autoencoder & Hashing-based Search

bash

CopyEdit

`jupyter notebook`

-   Open and run the desired notebook.

### **Query Image Search**

-   Upload an image to search for similar images in the gallery.
-   The retrieved images will be displayed along with similarity scores.

**📂 Project Structure**
------------------------

bash

CopyEdit

`📁 FashionMNIST-Similarity-Search
│── 📄 README.md
│── 📄 requirements.txt
│── 📁 gallery_set/      # Image gallery for similarity search
│── 📁 query_set/        # Query images to test similarity search
│── 📝 method_1.ipynb    # CNN-based feature extraction
│── 📝 method_2.ipynb    # Siamese Network
│── 📝 method_3.ipynb    # Vision Transformers & CLIP
│── 📝 method_4.ipynb    # Autoencoder & Hashing`

**📌 Future Improvements**
--------------------------

-   **Improve retrieval accuracy** by fine-tuning models.
-   **Optimize inference time** for real-world applications.
-   **Expand dataset** to include more diverse fashion images.

**📜 License**
--------------

This project is **open-source** under the **MIT License**
