# INGV - Volcanic Eruption Prediction
Challenge hosted by Kaggle in 2020. Discover hidden precursors in geophysical data to help emergency response by National Institute of Geophysics and Volcanology.

## Overview
What if scientists could anticipate volcanic eruptions as they predict the weather? While determining rain or shine days in advance is more difficult, weather reports become more accurate on shorter time scales. A similar approach with volcanoes could make a big impact. Just one unforeseen eruption can result in tens of thousands of lives lost. If scientists could reliably predict when a volcano will next erupt, evacuations could be more timely and the damage mitigated.

Currently, scientists often identify “time to eruption” by surveying volcanic tremors from seismic signals. In some volcanoes, this intensifies as volcanoes awaken and prepare to erupt. Unfortunately, patterns of seismicity are difficult to interpret. In very active volcanoes, current approaches predict eruptions some minutes in advance, but they usually fail at longer-term predictions.

Enter Italy's Istituto Nazionale di Geofisica e Vulcanologia (INGV), with its focus on geophysics and volcanology. The INGV's main objective is to contribute to the understanding of the Earth's system while mitigating the associated risks. Tasked with the 24-hour monitoring of seismicity and active volcano activity across the country, the INGV seeks to find the earliest detectable precursors that provide information about the timing of future volcanic eruptions.

In this competition, using your data science skills, you’ll predict when a volcano's next eruption will occur. You'll analyze a large geophysical dataset collected by sensors deployed on active volcanoes. If successful, your algorithms will identify signatures in seismic waveforms that characterize the development of an eruption.

With enough notice, areas around a volcano can be safely evacuated prior to their destruction. Seismic activity is a good indicator of an impending eruption, but earlier precursors must be identified to improve longer-term predictability. The impact of your participation could be felt worldwide with tens of thousands of lives saved by more predictable volcanic ruptures and earlier evacuations.

## Evalutation Metrics
The model performane is evaluated in the mean absolute error (MAE) between the predicted loss and the actual loss.

## Data description
Detecting volcanic eruptions before they happen is an important problem that has historically proven to be a very difficult. This competition provides you with readings from several seismic sensors around a volcano and challenges you to estimate how long it will be until the next eruption. The data represent a classic signal processing setup that has resisted traditional methods.

Identifying the exact sensors may be possible but would not be in the spirit of the competition nor further the scientific objectives. Please respect the importance of the problem and the time invested by the researchers at INGV in making this problem available by not seeking more metadata or information that would be unavailable in a real prediction context.

## Description of the project
Download the dataset here: https://www.kaggle.com/c/predict-volcanic-eruptions-ingv-oe/data
- Lib/:
    - utils.py: contains the preprocessing of the data and some useful functions to access data
    - decision_tree.py: contains the definition and training of the decision tree with gradient boosting (lightgbm)
- data/:
    - preprocessing/: contains the features extracted from the signals
    - sample_submission.csv: example of the desired output to get scored
    - train.csv: file given in the dataset
    - lgbm_importances-01.png: features ordered by importance according to the decision tree
    
   
## Results:
I was able to reach the second position on the leaderboard with a score of 4780462 (mean absolute error).
