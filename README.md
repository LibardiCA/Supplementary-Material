# Supplementary-Material
Repository dedicated to archiving supplementary materials, including mathematical formulas and primarily Python code, used in the scientific productions of Nathalia Fernanda Dias. For more information, refer to her Lattes curriculum: http://lattes.cnpq.br/6901117134684357
Step-by-Step Guide: Running the Association Analysis and Stacked Bar Chart Scripts in Python

This guide provides comprehensive instructions for setting up your environment and running the two Python scripts used for statistical visualization and data analysis.
The first script generates a heatmap-like table summarizing association tests (e.g., Chi-square, p-value, and Cramer’s V).
The second script produces a stacked bar chart displaying sex-based distributions of study characteristics.

Follow the steps below carefully to ensure a smooth execution.

1. Install Python

To execute the scripts, you must have Python installed on your system.

Download and Install Python

Visit the official Python website: https://www.python.org/downloads/

Download the latest stable version compatible with your operating system (Windows, macOS, or Linux).

During installation, ensure that the option “Add Python to PATH” is checked before clicking “Install Now”.

Wait until the installation completes successfully.

Verify Installation

After installation, open your terminal (macOS/Linux) or Command Prompt (Windows) and type:

python --version


You should see the installed Python version, confirming a successful installation.

2. (Optional) Install an Integrated Development Environment (IDE)

Although the scripts can be executed using any text editor, using an IDE significantly improves workflow.
A good free option is Visual Studio Code (VS Code).

Download and Install VS Code

Visit: https://code.visualstudio.com/

Download and install it following the on-screen instructions.

Install the Python Extension

Open VS Code.

Go to Extensions (Ctrl + Shift + X).

Search for Python and click Install.

3. Install Required Python Libraries

Both scripts rely on standard scientific computing and visualization libraries.
To install them, open a terminal or command prompt and run:

pip install pandas numpy matplotlib seaborn scipy

Explanation of Packages

pandas – for handling and organizing data tables.

numpy – for numerical computations.

matplotlib – for producing high-quality scientific figures.

seaborn – for additional visualization tools.

scipy – for statistical analyses (if required for related scripts).

If you plan to use Jupyter Notebook, also install:

pip install jupyter

4. Running the Scripts

Both scripts can be executed independently. Each one produces a specific type of visualization.

A. Association Matrix Visualization

This script generates a rectangular grid summarizing statistical associations among variables using Chi-square (χ²), p-values, and Cramer’s V.
The grid cells are color-coded according to the strength of association.

Execution Steps

Create a new file named association_matrix.py.

Copy and paste the entire first script (starting from import pandas as pd up to plt.show()).

Save the file.

In your terminal or VS Code, navigate to the folder containing the file:

cd path/to/your/script


Run the script with:

python association_matrix.py


The program will display a color-coded figure representing the associations.
The color intensity corresponds to the Chi-square magnitude, and a colorbar is displayed on the right-hand side.

B. Stacked Bar Chart Visualization

This script generates a stacked bar chart representing the percentage distribution of categories (“Female”, “Male”, “Female and Male”) across three study descriptors:

Sex of participants

Sex of the first author

Sex of the last author

Execution Steps

Create a new file named stacked_bar_plot.py.

Copy and paste the entire second script (from import matplotlib.pyplot as plt to the end).

Save the file.

Run the script as follows:

python stacked_bar_plot.py


A pop-up file dialog will appear asking where to save the figure.
After selecting the desired location, the script automatically saves three high-resolution versions of the figure:

.jpg

.tiff

.eps

Output Details

The bars are normalized to 100%, and the Y-axis values include the percentage symbol (%).

The legend appears horizontally below the chart, from right to left (Female → Male → Female and Male).

Transparency (alpha) and tone adjustments (fator_tom) control the brightness and opacity of the bar colors.

5. Troubleshooting

If you encounter issues, refer to the following common solutions:

Issue	Possible Cause	Solution
ModuleNotFoundError	Missing dependencies	Run pip install pandas numpy matplotlib seaborn scipy
python not recognized	Python not added to PATH	Reinstall Python ensuring “Add Python to PATH” is selected
Graph not displaying	Backend issue in some OS	Add plt.show() at the end of the script
Saving error	No permission or invalid path	Choose another directory when prompted
6. Conclusion

By following this guide, you can replicate the statistical visualizations and figures used in the analyses with precision and reproducibility.
Both scripts are written in Python 3, follow academic coding standards, and produce publication-quality figures suitable for inclusion in scientific manuscripts or presentations.

Happy coding and data analysis!
