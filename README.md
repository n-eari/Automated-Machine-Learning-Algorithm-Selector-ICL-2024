# 4th Year Undergraduate Computational Project (2024)
 
## Script to preprocess and evaluate multiple machine learning alogorithims on a materials dataset to compare statistics and performance.

### Written by Navraj Eari | as part of our submission for the "MATE70026 - Machine Learning for Materials" module.

- The matbench_perovskites dataset is used, which is provided by Matbench (Figshare URL: https://ml.materialsproject.org/projects/matbench_perovskites.json.gz)
- The following dataset was then
	- Cleaned
	- MinMax Scaled
	- Featureised using the "ElementFractions" and "ElementProperties" featureiser.
- The following regressors were evaluated and tested against eachother on a test-trained split dataset using 10 K-straitifed splits, with the hyperparamters adjusted using a parameter grid:
	- Random Forest
	- XGB
	- K Nearest Neibours
	- Support Vector Regression
	- Decision Tree
	- Auto Machine Learning (FLAML)
	- Dense nerual network created with AutoKeras
- The scoring criteria was based of the:
	- Root Mean Squared Error (RMSE)
	- Mean Absolute Error (MAE)
	- R squared (r2)

### Results
<img width="450" alt="image" src="https://github.com/user-attachments/assets/fb8e2fcd-7466-428c-bd7e-8ac4973c4ccc" />

<img width="450" alt="image" src="https://github.com/user-attachments/assets/2b1662a1-7dbf-4708-bc89-802e44b0140d" />

<img width="450" alt="image" src="https://github.com/user-attachments/assets/74173511-5089-4ee8-bce9-81a9dd2c7f15" />

<img width="450" alt="image" src="https://github.com/user-attachments/assets/3258bc19-f176-42b6-b724-f6520ca3c78b" />

- Results show that the XGB regressor performed the best, and the SHAP plot provides insights into the more critical features which impacted the model the most.

- To use, run the Juypter notebook. Ensure all files are in the same directory.
