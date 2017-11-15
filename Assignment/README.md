# MET Machine Learning Assignment

## General Instructions

### You choose ONE of the problems to work on

To pass the MET Machine Learning Course, you will be required to write a report describing proposed solution to **one** of the case studies given below. Each case study lists few suggested problems you can solve, however it is general enough to encourage you to propose your own ideas.

Your selection of the dataset option has no impact on the achievable marks. We provide some background information on each dataset below.

### What you are expected to submit

The format of the report will be a Jupyter/Azure Notebook. These are the notebooks we also use for the coding session.
In any case, we need a readable PDF version of your notebook. You may also provide a URL to your notebook in addition to the PDF so that we can access the notebook directly.

Your submission MUST be your own work and must demonstrate your own reflection about the dataset as well as your understanding of what you are doing in each step and why.

### When and how are you expected to submit

Please send the PDF (and the URL if you wish) to pw351@cam.ac.uk by [date / time].
Please note that the URL alone is not sufficient; we need the PDF in any case.

### How you will be assessed

The assignment is designed to challenge you to think about the data science process rather than to simply apply the methods. Your report will be marked whether it contains the following ingredients:

|Marking criteria|Points|
|------|------|
|1. A sensibly conducted exploratory data analysis where you demonstrate how you tried to examine the data|x pts|
|2. The formulation of a valid, achievable data science problem|x pts|
|3. Data cleaning and preprocessing|x pts|
|4. Rationale of choice for the machine learning methods|x pts|
|5. Building models|x pts|
|6. Optimising models|x pts|
|7. Conclusions|x pts|

We prepared some questions that might help you to conform to the report requirements.

1. Can the problem formulated be answered through applying machine learning?
2. Is it a unsupervised/supervised and classification/regression/clustering/... problem?
3. Does the dataset contain invalid data entries?
4. Is the dataset skewed?
5. Does the dataset require application of a normalisation method?
6. What types of variables (e.g. categorical, ...) does the dataset contain?
7. Do chosen machine learning methods work well with the type of dataset that is analysed?
8. Are chosen machine learning methods appropriate for the formulated problem?
9. Is the dataset divided into train/cross-validation/test subsets?
10. What metrics are used to evaluate the performance of the model? Are they appropriate for the dataset?
11. Which models perform well on the dataset, which do not, and why?
12. When the model optimisation process can be stopped?
13. Does the model solve the original problem formulated?

You are encouraged to use more than just one machine learning method to explore their potential in solving the problem you have formulated. Bear in mind that the consistency of the data science process you follow is the most important marking criteria. This means that your model might perform poorly, as long as you can explain why and suggest possible improvements.

You are encouraged to also leave included reasonable analyses that you conducted but that did not lead to major findings.

** Here should be some tips on formulating the problem **

## 1. Traffic Accidents in Leeds

### Problem specification
The Leeds City Council is running a programme "Safer Streets in Leeds". They were collecting accident data in 2016 and now they would like to engage a team of data scientists to explore the usefulness of the dataset. You were asked to advise the local authorities on the strategy and how data science could be used in the programme. The City Council already has some ideas in mind:

1. Developing awareness campain that is tailored for people that are most likely to be engaged in the accident, or
2. Identify roads/junctions in which road design/speed restrictions could be improved, or
3. Develop an accident casualty predictive model to be able to mobilise police/medical forces more effectively.

However, you are free to propose other solutions.

### The dataset

The dataset provided is *Leeds_RTC_2016.csv*, please download it from the course repository. You can also download the data from: https://data.gov.uk/dataset/road-traffic-accidents

It contains the following features:
1. Accident reference number
2. Y-coordinates of the place of the accident
3. X-coordinates of the place of the accident
4. Number of vehicles engaged in the accident
5. The area and year in which the accident happened
6. Accident date
7. Time of the accident expressed as a number e.g. 1600 corresponds to 4pm.
8. The class of the road on which accident happened
9. Lightning conditions during the accident
10. Weather conditions during the accident
11. Casualty class - who was affected by the accident
12. Casualty severity - the impact of the accident on the person involved.
13. Age of the casualty
14. Type of vehicle involved in the accident

## 2. Problem 2

### Background information

The original aim of the research was to correctly classify the type of surface defects in stainless steel plates, with six types of possible defects (plus "other"). The Input vector was made up of 27 indicators that approximately [describe] the geometric shape of the defect and its outline. According to the research paper, Semeion was commissioned by the Centro Sviluppo Materiali (Italy) for this task and therefore it is not possible to provide details on the nature of the 27 indicators used as Input vectors or the types of the 6 classes of defects.

### Description of the dataset

There are 34 fields. The first 27 fields describe some kind of steel plate faults seen in images. Unfortunately, there is no other information that I know of to describe these columns.
1. X_Minimum
1. X_Maximum
1. Y_Minimum
1. Y_Maximum
1. Pixels_Areas
1. X_Perimeter
1. Y_Perimeter
1. Sum_of_Luminosity
1. Minimum_of_Luminosity
1. Maximum_of_Luminosity
1. Length_of_Conveyer
* TypeOfSteel_A300
* TypeOfSteel_A400
* Steel_Plate_Thickness
* Edges_Index
* Empty_Index
* Square_Index
* Outside_X_Index
* Edges_X_Index 
* Edges_Y_Index 
* Outside_Global_Index 
* LogOfAreas 
* Log_X_Index 
* Log_Y_Index 
* Orientation_Index 
* Luminosity_Index 
* SigmoidOfAreas

The last seven columns are one hot encoded classes, i.e. if the plate fault is classified as "Stains" there will be a 1 in that column and 0's in the other columns. If you are unfamiliar with one hot encoding, just know that the last seven columns are your class labels.
Pastry Z_Scratch K_Scatch Stains Dirtiness Bumps Other_Faults


## 3. Problem 3
