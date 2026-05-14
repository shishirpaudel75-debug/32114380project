# The Use of Machine Learning in Waste Processing from Hospitals

## Project Overview

This final-year project investigates how machine learning can support hospital waste classification and improve waste segregation in healthcare environments. The project focuses on the use of machine learning and computer vision concepts to classify hospital waste according to NHS Health Technical Memorandum 07-01 (HTM 07-01) waste categories.

The project is simulation-based and uses a synthetic dataset instead of real hospital waste images. This approach was selected because collecting real hospital waste images may involve ethical, privacy, safety, and access limitations. The simulation allows the machine learning workflow to be tested without using patient data, staff data, or real hospital waste imagery.

## Project Aim

The aim of this project is to analyse machine learning methods used in hospital waste processing and evaluate their effectiveness, limitations, and practical applicability in healthcare settings.

## Objectives

The main objectives of this project are:

- To review machine learning techniques used in hospital waste classification.
- To evaluate the strengths and weaknesses of existing machine learning approaches.
- To identify technical, operational, ethical, and regulatory challenges.
- To develop a simulation-based machine learning workflow.
- To propose a conceptual framework for implementing ML-based hospital waste classification in NHS settings.

## Repository Contents

This repository contains the Colab/Jupyter notebook used for the simulation part of the project.

| File | Description |
|---|---|
| `project_notebook.ipynb` | Main notebook containing the simulated ML workflow, dataset generation, model training, evaluation, and visualisation outputs. |

## Methodology

The project uses a desk-based and simulation-driven research method. The simulation is implemented using Python and machine learning libraries. A synthetic dataset of 3,200 samples is created to represent hospital waste categories based on HTM 07-01 classification.

The dataset uses 64-dimensional synthetic feature vectors to represent CNN-style image features. These features are generated using class-specific distributions to simulate differences between waste categories. Some overlap is deliberately included between visually similar categories, such as infectious, sharps, and anatomical waste.

## Waste Categories Used

The simulation includes eight HTM 07-01-related waste categories:

- Infectious waste
- Cytotoxic waste
- Pharmaceutical waste
- Sharps waste
- Chemical waste
- Offensive waste
- Anatomical waste
- General non-hazardous waste

## Machine Learning Models

Three machine learning models are tested in the notebook:

1. **Random Forest classifier**  
   Used to simulate an EfficientNet-B0 / CNN-style feature classification approach.

2. **Support Vector Machine (SVM)**  
   Used as a classical machine learning classifier on CNN-style features.

3. **Logistic Regression**  
   Used as a simple baseline classifier.

## Evaluation Metrics

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Weighted F1-score
- Confusion matrix
- ROC curve
- ROC-AUC score
- Cross-validation accuracy
- PCA feature-space visualisation
- Simulated learning curves
- Simulated Grad-CAM style explainability visualisation

## Key Results

The simulation achieved strong classification results on the synthetic feature-vector dataset. The simulated EfficientNet-B0 approach achieved approximately:

- Test accuracy: **99.53%**
- Weighted F1-score: **0.9952**
- Mean ROC-AUC: **1.0000**

The SVM and Logistic Regression models achieved **100% accuracy** on the synthetic feature set. These high results should be interpreted as simulation-based performance rather than proof of direct NHS deployment readiness. Further work would be required using real hospital waste image datasets before practical NHS deployment.

## Limitations

This project has some important limitations:

- The dataset is synthetic and does not use real hospital waste images.
- The simulation represents CNN-style feature vectors rather than training a full deep learning image model.
- The high classification scores are partly due to the controlled structure of the synthetic feature space.
- Real-world factors such as lighting, camera angle, background noise, object occlusion, and hospital workflow differences are not fully captured.
- The system has not been tested in a live hospital environment.
- The implementation is a simulation/proof-of-concept rather than a deployed software system.

## Ethical Considerations

No real patient data, hospital staff data, or real hospital waste images are used in this project. The project uses synthetic data only, making it suitable for a low-risk simulation-based study.

## Tools and Libraries Used

The project uses:

- Python
- Google Colab / Jupyter Notebook
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

## How to Run the Notebook

1. Open the repository on GitHub.
2. Open `project_notebook.ipynb`.
3. Click **Open in Colab** or download the notebook and open it in Jupyter Notebook.
4. Run the cells from top to bottom.
5. Review the generated outputs, including tables, model results, confusion matrix, ROC curves, PCA plot, and other visualisations.

## Project Output

The notebook produces:

- Synthetic hospital waste dataset
- Trained ML classifiers
- Model performance comparison
- Confusion matrix
- Per-class performance table
- ROC curve analysis
- PCA feature-space visualisation
- Simulated explainability outputs
- Results and figures used in the final project report

## Final Report

The final report explains the full project, including the background, literature review, methodology, implementation, results, critical evaluation, NHS implementation framework, conclusions, and recommendations.

## Author

**Shishir Paudel**  
BSc Computer Science  
University of West London  
Student ID: 32114380

## Project Status

Completed for final-year project submission.
