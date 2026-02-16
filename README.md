Resume Screening and Placement Prediction Model
===

This project builds an end-to-end machine learning system to assist recruitment and campus placement analysis. It performs two core tasks:
1. **Resume Domain Classification (NLP)**: Automatically categorizes resumes into job domains using TF-IDF text vectorization and supervised learning.
2. **Placement Prediction**: Predicts whether a candidate is likely to be placed based on academic and experience features such as CGPA and internships.

The system demonstrates the integration of natural language processing with traditional machine learning for recruitment analytics.

> **Problem Statement**

Recruiters manually screen large volumes of resumes and evaluate candidate potential for placement. This project automates:
- resume domain identification
- placement likelihood prediction

> **Datasets**
1. **Resume Dataset**:
    - Resume text
    - Job category labels
    - Used for NLP classification
2. **Placement Dataset**:
    - Age
    - Gender
    - Academic stream
    - CGPA
    - Internships
    - Backlogs
    - Hostel status
    - Placement status (target)

> **System Architecture**

Resume Text → Cleaning → TF-IDF Vectorization → KNN Classifier → Domain Prediction → Structured Data → Feature Selection → Multiple ML Models → Placement Prediction

> **Machine Learning Techniques Used**
1. **NLP Pipeline**:
    - Text preprocessing
    - TF-IDF feature extraction
    - Label encoding
    - K-Nearest Neighbors classifier
    - Hyperparameter tuning (GridSearchCV)
    - Cosine similarity for resume matching
2. **Placement Prediction Models**:
- Multiple classifiers compared:
    - Logistic Regression
    - Support Vector Machine
    - K-Nearest Neighbors
    - Random Forest

- Model evaluation:
    - accuracy
    - confusion matrix
    - cross-validation

> **Features**
- Resume category classification
- Candidate placement prediction
- Model comparison framework
- Cross-validation evaluation
- Model persistence
- Interactive prediction interface

> **Technologies Used**

Python, Scikit-learn, NLP (TF-IDF, spaCy), Pandas, NumPy, Matplotlib, Seaborn

> **Future Improvements**
- Deep learning NLP (BERT)
- Resume parsing automation
- Real recruiter dashboard
- More predictive features
- Deployment as web app
