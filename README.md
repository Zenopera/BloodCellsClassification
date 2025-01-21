# BloodCellsClassification


This project addresses a multi-class classification problem using 96x96 RGB images of blood cells. The dataset includes eight distinct classes, each representing a specific type of blood cell, such as basophils, neutrophils, and lymphocytes.

Our approach began with a simple from-scratch model to establish a baseline. We then applied transfer learning with fine-tuning, leveraging pre-trained networks to improve classification accuracy and efficiency.

Repository Contents

Report - LOS PINGUINOS

The report provides a detailed overview of the following project stages:

Data inspection and cleaning: Initial data exploration, identification, and removal of outliers (e.g., irrelevant images like Shrek and Rick Astley).

Dataset splitting: Strategy for splitting the data into training, validation, and test sets.

Developed models:

Basic Model: Built from scratch with three convolutional layers, incorporating regularization and data augmentation techniques.

Transfer Learning and Fine-Tuning: Implementation of ConvNeXtSmall with advanced augmentation, fine-tuning layers, and pre-trained networks.

Conclusions: Analysis of achieved performance and considerations for future improvements.

Code Files

Basic_model.ipynbContains the implementation of the initial baseline model built from scratch. This notebook includes:

Creation of a simple CNN with three convolutional layers.

Application of basic techniques to mitigate overfitting (dropout and L2 regularization).

Evaluation of performance on the local validation dataset.

Basic_with_ImageDataGenerator.ipynbIntroduces an improved model by leveraging data augmentation techniques to enhance data variability and generalization. This notebook includes:

Rotations, flips, translations, and adjustments to brightness and contrast.

Computation of class weights to address dataset imbalance.

Improved results compared to the baseline model.

Final_Model.ipynbDetails the final approach to the problem using transfer learning and fine-tuning. It includes:

Use of the pre-trained ConvNeXtSmall model.

Advanced data augmentation with custom pipelines.

Fine-tuning strategy involving selective unfreezing of convolutional layers and mixed precision training.

Achieved performance: 97.66% accuracy on the local test set.

Getting Started

Clone this repository:

git clone https://github.com/your_username/BloodCellsClassification.git

Ensure you have Python and the required dependencies installed. Install them using:

pip install -r requirements.txt

Explore the .ipynb files to replicate our experiments and analyses.

Contributors

Daniele Vozza

Francesco Tomasi

Zeno Peracchione

Lorenzo Galatea
