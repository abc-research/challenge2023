---
layout: single
title: About the 5th ABC Challenge
permalink: /learn/
date: 2023-07-07T00:00:00+09:00
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

 To understand the dataset more clearly, [visit the dataset page](/challenge2023/data/)



## Result Submission
The submission file contains the columns detailed below. 
- timestamp: Base time of forecasting. Forecast whether or not a wearing-off will occur in the next hour after this time.
- participant : Corresponding patient’s ID
- final_wearing_off: 0 or 1
  - 0 means wearing-off will not occur
  - 1 means wearing-off will occur

Participants should forecast wearing-off for for each participant for all the timeframe detailed in the submission csv.

Please submit your results via the submission form. [Access the Submission Form here](https://forms.gle/pX1FCBMr9Tb5FE9n9)

<!--
Table 1 provides the overview of the file. 
You can download the [submission.csv from HERE](/challenge2023/assets/images/forecast_timeframe.png)

Participants should forecast wearing-off for the timeframe detailed in Table 1 for each participant.

![forecast_timeframe](/challenge2023/assets/images/forecast_timeframe.png)

![submission_format](/challenge2023/assets/images/submission_format.png)

The submission file name should be named challenge_[team_name]_result.csv following the format in Table 2.

![submission_file](/challenge2023/assets/images/submission_file.png)



- [Check the tutorial here](https://colab.research.google.com/drive/1A4zSOSO0IXwc-iB9EFdOr6mUP85KAxFm?usp=sharing)

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
All participants may use the data free of charge. [Download the dataset](https://ieee-dataport.org/competitions/5th-abc-challenge-forecasting-parkinsons-disease-patients-wearing-phenomenon-datasets)

<b> May 12 2023 : The data were updated because sleep data were not included.

## Prizes
- The winning team will be awarded 100,000 jpy.
- The registration fee for the 1st and 2nd runner-up teams will be waived.
- Each of the participating teams will be awarded with participation certificate.

