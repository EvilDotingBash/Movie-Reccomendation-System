🎬 Movie Recommender System Using Machine Learning

📌 Introduction

Recommendation systems are becoming increasingly important in today’s fast-paced world. With limited time and numerous options available, people rely on these systems to make the right choices efficiently.

The purpose of a recommendation system is to search for and suggest content that would be interesting to an individual. These systems analyze various factors to create personalized lists of useful and relevant content.

AI-driven recommendation algorithms skim through massive datasets and generate customized recommendations based on user profiles, browsing history, similarities with other users, and predictive modeling techniques.

🔍 Types of Recommendation Systems

1️⃣ Content-Based Filtering

Uses item characteristics and user preferences.

Examples: Twitter, YouTube.

Forms embeddings for features like music preferences, singer choices, etc.

Generates recommendations based on user-specific actions or item similarity.

Challenges: Over-specialization can lead to obvious or redundant recommendations.

2️⃣ Collaborative Filtering

Uses user-item interactions and ratings.

Identifies clusters of users with similar interests.

Example: Book recommendation systems.

Assumption: If User A and User B like Item X, and User B likes Item Y, then User A might also like Item Y.

Challenges:

Computationally expensive (User-Item matrix is large).

Biased towards popular items, neglecting new ones.

3️⃣ Hybrid Recommendation System

Combines both content-based and collaborative filtering methods.

Avoids the limitations of each method when used alone.

Uses techniques like word2vec and embedding models.

Commonly implemented in modern recommendation systems.

📌 About This Project

This is a Streamlit web application that recommends movies based on user interests using a precomputed similarity model.

🔹 Concept Used: Cosine Similarity

Cosine Similarity measures the similarity between two documents (or items) using vector representations.

It converts text data into vectors using numpy arrays.

The similarity score ranges from 0 to 1:

0 → Completely different items.

1 → Identical items.

For more details, check: Cosine Similarity Guide.

📂 Dataset Used

Dataset link: [Dataset URL] (Add dataset link here)

🛠️ Tech Stack

Programming Language: Python

Framework: Streamlit

Machine Learning: Cosine Similarity

Libraries: NumPy, Pandas, Scikit-Learn

📋 Project Structure
Movie-Recommender-System/
│
├── app.py                      # Streamlit app script
├── requirements.txt             # Project dependencies
├── models/                      # Pretrained models
│   └── model.pkl                # Movie recommendation model
├── notebooks/                   # Jupyter Notebooks for analysis
│   └── Movie_Recommender.ipynb   # Data analysis and model training
├── assets/                      # Images and resources
├── data/                        # Dataset files
├── utils/                       # Helper functions
└── README.md                    # Project documentation

🚀 Setup and Usage

1️⃣ Clone the Repository

git clone https://github.com/entbappy/Movie-Recommender-System-Using-Machine-Learning.git
cd Movie-Recommender-System-Using-Machine-Learning

2️⃣ Create a Virtual Environment

conda create -n movie python=3.7.10 -y
conda activate movie

3️⃣ Install Dependencies

pip install -r requirements.txt

4️⃣ Train the Model (if required)

Run the Jupyter Notebook to generate the models:

jupyter notebook Movie_Recommender.ipynb

5️⃣ Run the Application
