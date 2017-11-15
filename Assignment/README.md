# Instructions for the MET Machine Learning Assignment

## What you are expected to submit

You are required to submit your results in form of an [Azure Notebook](https://notebooks.azure.com/). This is the type of notebook we also work with during our practical coding sessions.

The notebook shall be in form of a report so that it contains both your code, results of your code (figures, ...) as well as your written reflections (as you would provide in a normal report).

Please submit your work in form of a PDF version of your notebook, and provide a URL to your Azure Notebook in addition to the PDF so that we can access the notebook directly.

Your submission MUST be your own work and must demonstrate your own reflections about the dataset as well as your understanding of what you are doing in each step and why. You are allowed and encouraged to use the Machine Learning and other Python libraries we have worked with in the practical coding sessions.

### When and how are you expected to submit

Please send the PDF and the URL to [**add email**] by [**add date / time**].
Please note that the URL alone is not sufficient; we need the PDF in any case.

### How you will be assessed

The assignment is designed to challenge you to think about the data science process rather than to simply apply the methods. Your report will be marked how well you worked through the following steps of the process:

|Marking criteria|Points|
|------|------|
|1. A sensibly conducted exploratory data analysis where you demonstrate how you tried to examine the data|x pts|
|2. The formulation of a valid, achievable data science problem|x pts|
|3. Data cleaning and preprocessing|x pts|
|4. Rationale for the choice of the machine learning methods|x pts|
|5. Building and evaluating your Machine Learning model |x pts|
|6. Conclusions|x pts|

We prepared some questions that might help you to conform to the report requirements:

1. Can the problem formulated be answered through applying machine learning?
2. Is it a unsupervised/supervised and classification/regression/clustering/... problem?
3. Does the dataset contain invalid data entries?
4. Is the dataset skewed?
5. Does the dataset require application of a normalisation method? If yes, which one?
6. What types of variables (e.g. categorical, ...) does the dataset contain?
7. Do chosen machine learning methods work well with the type of dataset that is analysed?
8. Are chosen machine learning methods appropriate for the formulated problem?
9. Did you divide the dataset into train/cross-validation/test subsets?
10. What metrics are you using to evaluate the performance of the model? Are they appropriate for the dataset?
11. Which models perform well on the dataset, which do not, and why?
12. When the model's performance can be considered as sufficient?
13. Does the model solve the original problem formulated?

You are encouraged to use more than just one machine learning method to explore their potential in solving the problem. Bear in mind that the consistency of the data science process you follow is the most important marking criteria. This means it is OK if your model does not perform perfectly well, as long as you can explain why and suggest possible improvements. This assignment is _not_ a competition for the highest accuracy.

You are encouraged to experiment, explore different options and report interesting findings in the assignment even if they are not directly linked to the chosen problem.

## Traffic Accidents in Leeds

### Problem specification (Fictional)
The Leeds City Council is running a programme "Safer Streets in Leeds". They were collecting accident data in years 2013 - 2016 and now they would like to engage a team of data scientists to explore the usefulness of the dataset. You were asked to advise the local authorities on the strategy and how data science could be used in the programme. The City Council sees the opportunity to improve one of the following problem areas:

1. The City Council feels that future accidents could be prevented by increasing people's situational awareness. The authorities believe that the campain will be effective only when a group of citizens that are most likely to be involved in accidents is targeted. You are asked to advise them whether machine learning could help to devise their campain strategy.

2. There has been a database error which resulted in removal of the 'Road Surface' feature for some of the entires in the 2017 dataset. The Leeds City Council believes that machine learning can help them to fill-in the gaps caused by the IT failure.

3. When an accident happens the local hospital mobilises medical units as soon as the accident is reported. However, it happened in the past that the ambulance was not equipped with enough resources to treat everyone without having to go back to the hospital, or call for another unit. The City Council feels that machine learning could help the local hospital to estimate how many people were hurt in a crash based on the information reported by the witnesses. *HINT: you might need to merge columns that refer to the same accident to estimate number of casualties per accident*.

The Leeds City Council has limited time to engage your team in the project, therefore they asked you to help them in only ** *ONE* ** of the problem areas. However, you are free to propose them what other data science problems could be addressed through the data.

### The dataset

The dataset provided is *Leeds_RTC.csv*, it covers data on traffic accidents in the city of Leeds in years 2013 - 2016. Please download it from the course repository.

It contains the following features:
1. Accident reference number
2. Y-coordinates of the place of the accident
3. X-coordinates of the place of the accident
4. Number of vehicles engaged in the accident
5. Accident date
6. Time of the accident expressed as a number e.g. 1600 corresponds to 4pm.
7. The class of the road on which accident happened
8. Lightning conditions during the accident
9. Weather conditions during the accident
10. Casualty class - who was affected by the accident
11. Casualty severity - the impact of the accident on the person involved.
12. Age of the casualty
13. Type of vehicle involved in the accident

Traffic Accident Data, (c) Leeds City Council, 2017, https://datamillnorth.org/dataset/road-traffic-accidents. This information is licensed under the terms of the Open Government Licence.
