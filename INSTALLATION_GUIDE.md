INSTALLATION_GUIDE

Instagram User Analytics Using Machine Learning

Overview

This guide explains how to install, configure, and run the Instagram User Analytics project on your local machine.

The project uses Python and several data science libraries to analyze Instagram engagement data and predict post likes using machine learning.

──────────────────────────

System Requirements

Minimum Requirements

Processor: Intel Core i3 or equivalent

RAM: 4 GB

Storage: 2 GB Free Space

Python: Python 3.8 or higher

Operating System:

• Windows 10/11 • Ubuntu Linux • macOS

Recommended Requirements

Processor: Intel Core i5 or above

RAM: 8 GB or above

Storage: 5 GB Free Space

Python: Python 3.10+

──────────────────────────

Required Software

Install the following software before running the project:

• Python

• Jupyter Notebook

• Visual Studio Code (Optional)

• Git (Optional)

──────────────────────────

Clone Repository

Clone the repository from GitHub.

git clone https://github.com/Patlollavarunteja/-Instagram-User-Analytics-Using-Machine-Learning.git

Move into project directory.

cd -Instagram-User-Analytics-Using-Machine-Learning

──────────────────────────

Create Virtual Environment

Windows

python -m venv venv

venv\Scripts\activate

Linux/macOS

python3 -m venv venv

source venv/bin/activate

──────────────────────────

Install Required Libraries

Install all dependencies.

pip install -r requirements.txt

If requirements.txt is unavailable, install manually:

pip install pandas

pip install numpy

pip install matplotlib

pip install seaborn

pip install scikit-learn

pip install wordcloud

pip install jupyter

──────────────────────────

Project Structure

Instagram-User-Analytics-Using-Machine-Learning

dataset/ │ ├── Instagram_dataset.csv

src/ │ ├── data_preprocessing.py ├── visualization.py ├── model_training.py ├── prediction.py

results/

screenshots/

README.md

requirements.txt

──────────────────────────

Dataset Setup

Place the dataset file inside the dataset folder.

Example:

dataset/Instagram_dataset.csv

Verify the file name matches the name used in the source code.

──────────────────────────

Run Jupyter Notebook

Start Jupyter Notebook.

jupyter notebook

Open:

Instagram_User_Analytics.ipynb

Run all cells sequentially.

──────────────────────────

Run Python Script

Execute the main project file.

python main.py

or

python model_training.py

The program will:

• Load Dataset

• Preprocess Data

• Generate Word Clouds

• Create Regression Plots

• Train Machine Learning Model

• Generate Predictions

──────────────────────────

Expected Outputs

After successful execution, the following outputs will be generated:

• Caption Word Cloud

• Hashtag Word Cloud

• Regression Analysis Graphs

• Prediction Graphs

• Likes Progression Charts

• Model Accuracy Information

──────────────────────────

Troubleshooting

Problem: Module Not Found Error

Solution:

pip install missing_library_name

Example:

pip install pandas

──────────────────────────

Problem: Dataset Not Found

Solution:

Ensure Instagram_dataset.csv exists in the correct folder.

Check file path in source code.

──────────────────────────

Problem: Jupyter Notebook Not Opening

Solution:

pip install notebook

jupyter notebook

──────────────────────────

Problem: Graphs Not Displaying

Solution:

Install matplotlib correctly.

pip install matplotlib

Restart the notebook kernel.

──────────────────────────

Verification Checklist

Before running the project confirm:

✓ Python installed

✓ Dataset available

✓ Dependencies installed

✓ Virtual environment activated

✓ Project files downloaded

✓ Correct file paths

──────────────────────────

Successful Execution

The installation is successful when:

✓ Dataset loads correctly

✓ Visualizations are displayed

✓ Machine learning model trains successfully

✓ Predictions are generated

✓ Performance score is displayed

──────────────────────────

Conclusion

After completing the installation steps, the Instagram User Analytics project will be fully operational and ready for data analysis, visualization, and machine learning-based engagement prediction.
