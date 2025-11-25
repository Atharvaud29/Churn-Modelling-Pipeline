## MLOps on GitHub | Deploy and Automate ML Workflows using GitHub Actions and CML for CI/CD

- **This project demonstrates how to build a machine learning pipeline for predicting customer churn using a Gradient Boosting Classifier. It leverages GitHub Actions for automation and Continuous Machine Learning (CML) for tracking metrics and results directly in GitHub**.

## Pipeline Workflow

<img width="1400" height="540" alt="image" src="https://github.com/user-attachments/assets/70347faa-f6fb-4169-b01a-cb1736078c54" />

## Features
- **Data Processing** : Efficient loading and preprocessing of data.
- **Model Training** : Uses Gradient Boosting for churn prediction.
- **Model Evaluation** : Confusion matrix and ROC curve visualization.
- **CI/CD Integration** : Automates model training and evaluation using GitHub Actions.
- **CML Integration** : Generates reports of model metrics and plots.

### Actions:
<img width="907" height="898" alt="Screenshot 2025-11-25 220228" src="https://github.com/user-attachments/assets/841304cb-8406-4b39-b849-79bf53068b8a" />
<img width="903" height="723" alt="Screenshot 2025-11-25 220300" src="https://github.com/user-attachments/assets/8635646d-7598-47fe-9c62-e0511761c347" />

## Technologies Used :
    Python
    Scikit-learn
    Pandas
    Matplotlib
    GitHub Actions
    Continuous Machine Learning (CML)

## Overview

This project utilizes GitHub Actions to automate the training and evaluation of the churn prediction model. The workflow triggers on pushes and pull requests to the main branch.

### GitHub Actions Configuration:

- The **.github/workflows/main.yml** file defines the workflow. Key steps include:

    1. Checkout Repository: Retrieves the code from the repository.
    2. Install Packages: Installs required Python packages.
    3. Format Code: Automatically formats Python scripts using Black.
    4. Train Model: Runs the train.py script to train the model.
    5. Evaluate Model: Generates a report with metrics and plots, posting results in GitHub comments using CML.

### CML Integration:

- CML (Continuous Machine Learning) is used to create dynamic reports that include model performance metrics and visualizations.

### How to Use:

  - Update the Dataset: Place your dataset (Churn_Modelling.csv) in the root directory of the project.
  - Push Changes: Commit and push changes to the main branch to trigger the GitHub Actions workflow.
  - Review Results: After the workflow completes, check the GitHub Actions tab for logs and results.

### Results:

- Upon successful execution of the workflow, you will find:

    - Model Metrics: Accuracy and F1 Score.
    - Visualizations: Confusion matrix and ROC curve plots.
    - Comments in PRs: CML will post the metrics report in GitHub comments for easy review.

## 🤝Contributing

Contributions are welcome! Please submit a pull request or open an issue for any improvements or bug fixes.

## 📜License

This project is licensed under the MIT License - see the LICENSE file for details.
