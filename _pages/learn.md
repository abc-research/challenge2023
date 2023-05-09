---
layout: single
title: Abouth the 5th ABC Challenge
permalink: /learn/
date: 2023-05-8T00:00:00+09:00
---

## Forecasting Parkinson's Disease Patients' Wearing-Off Phenomenon

Parkinson's disease (PD) is a neurodegenerative disorder caused by the loss of dopamine-producing brain cells.
It primarily affects the patient's motor abilities but also impacts non-motor functions over time.
Patients' symptoms include tremors, muscle stiffness, and difficulty walking and balancing.
Then it disrupts the patients' sleep, speech, and mental functions, affecting their quality of life (QoL).

PD patients who experience the wearing-off phenomenon have their symptoms reappear before their next Levodopa (L-dopa) treatment intake.
L-dopa treatment is a one of the treatments for PD patients by producing dopamine in the brain, which alleviates the symptoms.
Over time, the medicine's effective time shortens, causing discomfort among PD patients.
Thus, patients and clinicians need to monitor and record the patient's symptoms for adequate treatment, since there is no cure for Parkinson's disease.

Patients and clinicians can continuously monitor patients' health with the improvement of wearable devices such as smartphones, fitness trackers, and smartwatches.
We use these technologies to monitor patients' health, record wearing-off periods, and document the impact of L-dopa intake on their symptoms in order to forecast the wearing-off periods in PD patients.

## Challenge Goal 
The goal of this challenge is to forecast the wearing-off in the next hour given past data.
Participants are tasked to create a model that can anticipate the "wearing-off" of anti-PD medication.
In a real-world setting, we used fitness tracker data and self-reported symptoms via a smartphone app.
This will help the doctors to create specific treatment strategies to properly manage Parkinson's disease and its associated symptoms. Participants' task is to develop a model that forecasts wearing-off in the next hour given past data. The original project is one of the [2022 Garmin Health Awards winners](https://www.kyutech.ac.jp/english/en-news/topics/entry-9408.html#prettyPhoto).

## Dataset Overview
There are three datasets for this challenge.
- Garmin dataset contains PD patients' heart rate, number of steps, stress level, and sleep pattern.
- Wearing-off periods dataset was based on the Wearing-Off Questionnaire (WoQ-9). PD patients self-report the absence or presence of wearing-off symptoms.
- Drug intake dataset was also based on the WoQ-9. PD patients self-report the time of drug intake, and the effect of the drug to their symptoms.

<!--
- [Check the tutorial here](https://colab.research.google.com/drive/1A4zSOSO0IXwc-iB9EFdOr6mUP85KAxFm?usp=sharing)
- [To understand the dataset more clearly](/challenge2022/data/)
- [Download the dataset](https://ieee-dataport.org/competitions/nurse-care-activity-recognition-challenge-datasets-2022-0)


edit this part
The training and testing dataset contains accelerometer data and care record data of 5 users ( 8, 13, 14, 15, 25), which were collected on May and June, 2018. Training and testing data were separated in 70~30 ratio based on each user data. Participants are required to propose their pipelines, predict and submit the activity label for the testing dataset.


The goal of the Nurse Care Activity Recognition Challenge is to recognize the daily activities of a caregiver/nurse in a healthcare facility based on the accelerometer data collected from smartphones. Participants utilize accelerometer data and its activity labels in training files, propose the methods to extract features from these data, and then feed to their own model. Finally, each team needs to use their model to predict the activity based on the accelerometer data following by the timestamp in the test data. 



The training and testing dataset contains accelerometer data of 12 users (2, 3, 4, 5, 6, 7, 9, 12, 17, 19, 21, and 22), which were collected on May and June, 2018. The training data is provided with the activities labels, which describe the users’ activities before 18th June, 2018. The testing data was the accelerometer data acquired on 18th June and afterward. Participants are required to propose their pipelines, predict and submit the activity label for the testing dataset.



## Evaluation
Accuracy will be used as the performance measure.
Submissions will be evaluated by the average of the accuracy of macro activity classification (ma) and the average accuracy of micro-activity classification (mi). That is (ma+mi)/2.

The average accuracy of micro-activity classification is based on the multi-label accuracy formula. The accuracy of one sample is given by the number of correct labels predicted divided by the number of total true and predicted labels (cardinality of the union). 

## Evaluation
Participants are required to propose their pipelines, predict and submit the activity label for the testing dataset as shown in the [tutorial](https://colab.research.google.com/drive/1euqLhhsb21bbOETWMY9DkUcue6t33j1j?usp=sharing). The test submission folder contains test time stamps that you need to predict for each user. The files contain time stamps, and activity_type_ids and the columns are filled up with zero as shown in Table 3 below.

![Table3](/challenge2022/assets/images/Table3.png)

The participants are required to put 1 in place of 0 when the activity is supposed to happen and regenerate the files. Please make sure to maintain the shape same as the provided files(any changes that occurred in the submission are not the liability of the organizers, please make sure that there is no difference in shape and activity_type_id with the given file). 

As shown in Table 3, we expect the participants to generate 5 similar files one for each user, and submit them to us. As the occurrence of activities differs in different users we will match with label files of each user and see how many activities were accurately identified to have occurred by the participants.

For evaluation along with counting the percentage of how many activities were predicted for each user, we will also consider Precision, Recall, and F1 Score. We will take an average of all the scores of all the users.The baseline result for each user is shared in the table below.


![Table4](/challenge2022/assets/images/Table4.png)


## Result Submission
Please submit your results via the submission form. [Access the Submission Form here](https://forms.gle/cDEhfHQjiSGKP5Zh6)
-->
## Data use
All participants may use the data free of charge. [Download the dataset]([https://ieee-dataport.org/competitions/nurse-care-activity-recognition-challenge-datasets-2022-0](https://ieee-dataport.org/competitions/5th-abc-challenge-forecasting-parkinsons-disease-patients-wearing-phenomenon-datasets)


## Prizes
- The winning team will be awarded 100,000 jpy.
- The registration fee for the 1st and 2nd runner-up teams will be waived.
- Each of the participating teams will be awarded with participation certificate.

