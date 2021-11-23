# Antimicrobial Peptide Identification with NLP [(colab)](https://colab.research.google.com/drive/19hZ5OoqtFFKC4G7Yr5rYq0GYcKSBW7Ql#scrollTo=Ul-D9UCa_kHg)
I worked led my team to create several Natural Language Processing models to identify whether or not a given peptide may have antimicrobial properties. This project was interesting, and allowed us to explore the intersection between Machine Learning and proteomics. We evaluated 8 different model architectures and found that Random Forest had the highest F1 score (0.95+)

## Problem Statement:
Peptides are proteins comprised of a relatively short chain of amino acids. The drug discovery and wellness industry look at peptides as a potential solution for health optimization and disease management while being radically cost effective and with little to no known side-effects. This makes the process of discovering such amino acid chains a valuable endeavor. There are many studies that indicate that certain peptides have anti-cancer properties - these are known as APCs. The function of these peptides is determined by their amino acid sequence.

Our Project focused on using the Word2Vec algorithm to encode amino acid sequences of variable length into embeddings. This is an important step as these amino acid sequences have important positional and structural relationships which will be preserved and exploited in order to create embeddings.

This is a supervised classification problem, where categorized certain peptides as therapeutic or not. As a final step, we presented the task of successful discovery as a classification problem.

## Data description
[Example data](http://split4.pmfst.hr/dadp/?a=list)
We will extract roughly 2150 peptides from the DADP, or the database of anuran defense peptides, which has thousands of peptides found in the skin of frogs that have been shown to have antimicrobial properties

"While it is easy to download the positive data set from the APD, it is difficult to get a true negative data set because the activities of the sequences in the negative data set have not been validated by experiments. Yet, the program is set up with good predictive ability." -Improved Methods for Classification, Prediction and Design of Antimicrobial Peptides. This is based on the methodology from [a study to find anticancer peptides](https://www.researchgate.net/publication/258055594_In_Silico_Models_for_Designing_and_Discovering_Novel_Anticancer_Peptides).

Datasets: (https://webs.iiitd.edu.in/raghava/satpdb/catalog.php), (APD, http://aps.unmc.edu/AP/main.php), (CAMP, http://www.bicnirrh.res.in/antimicrobial),(DADP, http://split4.pmfst.hr/dadp/)

## Model Architectures
We utilized supervised machine learning to build a classification model. We tried using the following model architectures, and evaluated performance based on Accuracy score, Sensitivity, and Specificity. 
- Decision Tree
- SVM (Support Vector Machine)
- Linear Discriminant Analysis
- Quadratic Discriminant Analysis
- Random Forest
- K-nearest neighbors
- Bayes
- Neural Network
