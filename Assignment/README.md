# MET Machine Learning Assignment

## General Instructions

### You choose ONE of the problems to work on

To pass the MET Machine Learning Course, you will be required to write a report describing proposed solution to **only one** of the case studies given below. Each case study lists few suggested problems you can solve, however it is general enough to encourage you to propose your own ideas.

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

## 1. Traffic Accidents in Leeds (Problem Option 1)

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

## 2. Steel plates (Problem Option 2)

### Background information

The dataset describes results from the quality control of stainless steel plates.
A number of measurements have been made for each steel plate and you are also provided with the information if the steel plate was found to have one of the six possible defects.

### Description of the dataset

There are 34 fields. 

The first 27 fields contain measurements of each steel plate. In this case, you are not given more background information about the meaning of each measurement but we can assume they describe the geometric shape and other sensor measurements.

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
1. TypeOfSteel_A300
1. TypeOfSteel_A400
1. Steel_Plate_Thickness
1. Edges_Index
1. Empty_Index
1. Square_Index
1. Outside_X_Index
1. Edges_X_Index 
1. Edges_Y_Index 
1. Outside_Global_Index 
1. LogOfAreas 
1. Log_X_Index 
1. Log_Y_Index 
1. Orientation_Index 
1. Luminosity_Index 
1. SigmoidOfAreas

The last seven columns contain the fault type for each steel plate. If, for example, a plate has been found to have "bumps", there will be a 1 in the "Bump" column, and 0s in all other columns.

1. Pastry
1. Z_Scratch
1. K_Scatch
1. Stains
1. Dirtiness
1. Bumps
1. Other_Faults

## 3. Problem 3
