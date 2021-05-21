# Irrigreat

## Problem Definition
* Productivity needs to be increased so that farmers can get more pay from the same piece of land without degrading soil.
* Indian farmers aren’t able to choose the right crop based on their soil requirements depending upon factors like N, P, K, temperature, humidity, rainfall, pH.
* Farmers are generally unaware about the organic fertilizer or standard fertilizer to use as per soil requirements.
* Due to inadequate and imbalanced fertilization, soil degradation is occurring, which leads to nutrient mining and the development of second-generation problems in nutrient management.
* According to a study by the Associated Chambers of Commerce and Industry of India, annual crop losses due to pests amount to Rs. 50,000 crore.

## Objective
* To implement precision agriculture (A modern farming technique that uses research data of soil characteristics, soil types, crop yield data collection and suggests the farmers the right crop based on their site specific parameters to reduce the wrong choice on a crop and increase in productivity). 
* To solve the problem by proposing a recommendation system through an ensemble model with majority voting technique crop for the site specific parameters with high accuracy and efficiency.
* To recommend fertilizer on the basis of N, P, K values and crop.
* To recognize the pest and recommend particular pesticide available in India as per ISO standards.

## Methodology
### Crop Recommendation
1. Dataset Acquisition
2. Taking input values
3. ML Model Training & creating .pkl file
    1. Using Ensembling Technique with majority voting technique
        1. SVM
        2. Random Forest
        3. Naive Bayes
        4. kNN
4. Crop Recommendation
    1. Loading .pkl model file to recommend crop based on input data

### Fertilizer Recommendation
1. Dataset Acquisition
    1. NPK values for different crops
    2. Sources: 
        1. The Fertilizer Association of India, 
        2. Indian Institute of Water Management etc
2. Taking input values
3. Difference b/w desired & actual
    1. High
    2. Low
    3. Upto the mark
4. Dictionary based Suggestions (Solutions from verified sources)

## Pesticide Recommendation
1. Data Acquisition
    1. Image Scraping from Google Images
    2. Providing pest labels
2. Data Cleaning &  Data Augmentation
    1. Data is cleaned to remove not useful content
    2. The dataset is augmented so as to increase the variability
3. DL model creation
4. Pest Detection & Pesticide Recommendation

## Conclusion
India’s farmers are hard at work. They help to feed a nation whose population is nearly 1.4 billion. However their productivity is threatened by some natural factors that can ruin their crops and their livelihoods. So, the solution will benefit farmers to maximize productivity in agriculture, reduce soil degradation in cultivated fields, and have informed advice on organic fertilizers/ other fertilizers and also know about the right crop by considering various attributes. This would provide a comprehensive prediction and hence benefit both farmers and environment. Not only this, but pest control would also be major issue to be solved via this project.

## How to run on your local host?
Prerequisite: Download all files from GDrive Link
1. Download PyCharm
2. Create new environment using command --> conda create -n env_name python==3.7.0
3. Activate environment using command --> conda activate env_name
4. Install requirements by typing (cd ProjectFolder) --> pip install -r requirements.txt
5. Now run app.py by writing command --> python app.py

Website Link: https://irrigreat.herokuapp.com/
