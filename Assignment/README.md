# Instructions for the MET Machine Learning Assignment

## Coursework Instructions (this is the 3rd coursework within the INDUSTRIAL OPERATIONS MANAGEMENT module)

Belfast City local authorities regularly monitor the trees and collect data about them and their condition. The data set and further more detailed instructions can be found in this location: https://github.com/UniversityOfCambridgeDIAL/IntroToML/tree/master/Assignment. 

You will find information including the type of tree (street tree or park tree), the species, the shape, the location, and condition. Your task is it to check if and to what extent the other information provided in the dataset is sufficient to predict the type of tree ('TYPEOFTREE').

Build an appropriate prediction model for the type of tree ('TYPEOFTREE') using the typical data science pipeline, which is included in course slides. This includes:
- formulating the task as a data science problem,
- data preparation (cleaning, feature selection, normalization – where appropriate, and splitting data into training/cross-validation/testing),
- choosing at least two appropriate Machine Learning methods,
- building and evaluating these Machine Learning models,
- your reflections on the difference in performance between the models, and
- general conclusions, models’ limitations and ideas for possible prediction improvements.

You are required to submit your results in the form of an Azure Notebook (https://notebooks.azure.com/). This is the type of notebook we also work with during our practical coding sessions. The notebook will be in form of a report so that it contains both your code, results of your code (e.g. figures) as well as your written reflections.

Your submission must demonstrate your own reflections about the dataset as well as your understanding of what you are doing in each step and why. You are encouraged to use the Machine Learning and other Python libraries we have worked with in the practical coding sessions. Submit your Azure notebook file named “CourseworkID_Q3.ipynb” and a PDF version of your notebook named “CourseworkID_Q3.pdf”. [12 marks]

## Further more detailed instructions

### How to set up Azure account and notebook

* Please go to: https://notebooks.azure.com
* Please register with Azure or sign in with an existing account
* Click on new library and enter the required information. Please make sure you set the notebook to private by **unticking the "public library" checkbox** before you start your assignment.
* Download the dataset from https://github.com/UniversityOfCambridgeDIAL/IntroToML/Assignment/ to your local machine
* Then upload the dataset to your Azure notebook by clicking "New > Add Files to Library > From Computer".
* Now you can begin your assignment.

### How to print the notebook as PDF

* To print your notebook, please go to "File > Download As... > PDF via Latex" in the Jupyter notebook menu
* Should this fail for whatever reason, you can also print the notebook using the print options of your browser.

### How to download your notebook in an .ipynb format

* To download your notebook in an .ipynb format, please go to "File > Download As... > Notebook (.ipynb)" in the Jupyter notebook menu

### When and how are you expected to submit

Please send the PDF _and_ the .ipynb file to the email address provided in your coursework instructions.

### How you will be assessed

The assignment is designed to challenge you to think about the data science process rather than to simply apply the methods. Your report will be marked how well you worked through the following steps of the process:

|Marking criteria|
|------|
|1. A sensibly conducted exploratory data analysis where you demonstrate how you tried to examine the data|
|2. The formulation of a valid, achievable data science problem|
|3. Data cleaning and preprocessing|
|4. Rationale for the choice of the machine learning methods|
|5. Building and evaluating your Machine Learning model |
|6. Conclusions|

We prepared some questions that might help you to conform to the report requirements:

1. Can the problem be answered through applying machine learning?
2. Is it a unsupervised/supervised and classification/regression/clustering/... problem?
3. Does the dataset contain invalid data entries?
4. Is the dataset skewed or unbalanced?
5. Does the dataset require application of a normalisation method? If yes, which one?
6. What types of variables (e.g. categorical, ...) does the dataset contain?
7. Do chosen machine learning methods work well with the type of dataset that is analysed?
8. Are chosen machine learning methods appropriate for the formulated problem?
9. Did you divide the dataset into train/cross-validation/test subsets?
10. What metrics are you using to evaluate the performance of the model? Are they appropriate for the dataset?
11. Which models perform well on the dataset, which do not, and why?
12. When the model's performance can be considered as sufficient?
13. Does the model solve the original problem?

You are encouraged to use more than just one machine learning method to explore their potential in solving the problem. Bear in mind that the consistency of the data science process you follow is the most important marking criteria. This means it is OK if your model does not perform perfectly well, as long as you can explain why and suggest possible improvements. This assignment is _not_ a competition for the highest accuracy.

## Dataset

You will find the file "odTrees.txt" in the "Assignment" folder. To download the file:

- Click on the file "odTrees.txt" in the "Assignment" folder,
- You will see a message "(Sorry about that, but we can’t show files that are this big right now.)". This is because the file is too big to see the preview. However you can still download it by clicking right mouse button on "Download" and choosing "Download Linked File".

It gathers information about threes located in the Belfast City area and includes the following information:

1. "TYPEOFTREE", which defines whether the tree is a park or street tree
2. "SPECIESTYPE", which defines the family of species
3. "SPECIES", which defines the particular specie of the tree
4. "AGE", which defines the age of the tree (Young/Old etc.)
5. "DESCRIPTION", which defines more granular description of the age of the tree
6. "TREESURROUND", which defines the surrounding in which the tree grows (e.g. Grass or Bare Ground)
7. "VIGOUR", which defines the capacity of the tree to survive in unfavourable conditions
8. "CONDITION", which defines the general health of the tree (e.g. Good/Dying)
9. "DIAMETERinCENTIMETRES", which defines the diameter of the trunk, in centimeters
10. "SPREADRADIUSinMETRES", which defines the size of the crown, in meters
11. "TREELOCATIONX", which defines the location of the tree in local x coordinates
12. "TREELOCATIONY", which defines the location of the tree in local y coordinates
13. "LONGITUDE", which defines geographical longitude where positive values indicate E direction and negative values indicate W direction
14. "LATITUDE", which defines georgaphical latitude where positive values indicate N direction and negative values indicate S direction.
15. "TREETAG", which defines tree identification number
16. "TREEHEIGHTinMETRES", which defines the height of the tree in meters.
