# Description
* The Jupyter Notebook (.ipynb) file contains code for a multiple-output regression problem.
* The code takes in a .csv file (provided) which contains information regarding tuned K24Z7's.
* For every row in the .csv file, the information provided is the car's mod list (Intake, Intake Manifold, Downpipe, Exhaust, and Tuner), as well as its horsepower and torque outputs.
* The features are extracted and encoded from a "Yes/No" format to a binary (1/0) format to indicate its presence, which is then fed to a Random Forest Regressor model.
* The Random Forest Regressor model then determines which of the mods provides the biggest impact (via feature importance) on horsepower and torque outputs for a given tuner.

## Notes
* There is an imbalance of information for each tuner, so the evaluation must be done on a per-tuner basis.
  * Genesis: 64 rows
  * Precision: 41 rows
  * Derf: 3 rows
  * Drob: 3 rows
  * Javi: 1 row
* Dyno numbers cannot be directly translated between tuners, as there may be differences in dyno types and settings.
* By default, the code uses rows where Genesis is the tuner, but it can be changed in line 17.

## To Run
* You do not need to install anything to run this code!
* Visit https://jupyter.org/try-jupyter/tree/
* Create a new folder by clicking  "New" then "New Folder", and give the folder a name.
* Import both the .ipynb and .csv files to the folder you have just created.
* Open the .ipynb file.
* If prompted, select "Python (Pyodide)" as your kernel.
* Click on the ▶️ button, or press Shift + Enter on your keyboard to run the code. 
