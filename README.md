# 4th Year Undergraduate Computational Project (2024)
 
## Script to preprocess and evaliate multiple machine learning alogorithims on a materials dataset to compare statistics and performance.

### Written by Navraj Eari | as part of our submission for the "MATE70026 - Machine Learning for Materials" module.

- The matbench_perovskites dataset is used, which is provided by Matbench (Figshare URL: https://ml.materialsproject.org/projects/matbench_perovskites.json.gz)
- The following dataset was then cleaned, MinMaxScaled, and featureised using the "ElementFrtactions" Feturisier.
- The following regressors were evaluated and tested against eachother on a test-trained split dataset using 10 K-straitifed splits:
- Random Forest
- XGB
- K Nearest Neibours
- Support Vector Regression
- Decision Tree

<img width="471" alt="Screenshot 2022-07-08 153319" src="https://user-images.githubusercontent.com/102254245/178013220-5d4370ab-3c36-4d18-840b-2cad54066e90.png">

- Displays the predicted classifaction (the ones the alogorithmn calculated) against the actual classifaction (the true one, provided in the dataset). Therefore diagonal elements are desired.
- Abilty to remove a parameter via the box on the right, and observe how the accuracy of the classifer changes.

- To use, run the Juypter notebook. Ensure all files are in the same directory.

[1] - Santosh Behara, Taher Poonawala, Tiju Thomas, Crystal structure classification in ABO3 perovskites via machine learning, Computational Materials Science,
Volume 188, 2021, 110191,
ISSN 0927-0256,
(https://www.sciencedirect.com/science/article/pii/S0927025620306820)
