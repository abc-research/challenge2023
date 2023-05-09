---
layout: single
title: Data Description
permalink: /data/
date: 2023-05-8T00:00:00+09:00
---
There are three datasets for this challenge.
- Garmin dataset contains PD patients' heart rate, number of steps, stress level, and sleep pattern.
- Wearing-off periods dataset was based on the Wearing-Off Questionnaire (WoQ-9). PD patients self-report the absence or presence of wearing-off symptoms.
- Drug intake dataset was also based on the WoQ-9. PD patients self-report the time of drug intake, and the effect of the drug to their symptoms.


## Data structure
Datasets will be published in the following directory structure.

![data_structure](/challenge2023/assets/images/data_structure.png)

Inside the training data folder, we have provided files containing Garmin data, wearing-off information, and drug intake information.
If you open the files you can see the following columns for each sheet.

![t1_garmin](/challenge2023/assets/images/t1_garmin.png)

![t2_wearingoff](/challenge2023/assets/images/t2_wearingoff.png)

![t3_drugintake](/challenge2023/assets/images/t3_drugintake.png)


<!-- 
In the accelerometer data folder, the data is not split. So if you want to utilize it you can match it with your train and test care record file to split them as shown in the tutorial.

<p>
  <img src="/challenge2022/assets/images/Accelerometer.png" width="300" class="center"/>
</p>

If you open the files you can see that the data contains: subject_id(nurse/caregiver), datetime(timestamp), and triaxial sensor data (x,y, and z).

![Accel_sheet](/challenge2022/assets/images/Accel_sheet.png)

In the care record data folder, we provided the separated care record data as shown in the table.

<p>
  <img src="/challenge2022/assets/images/Care_record_folder.png" width="300" class="center"/>
</p>


In the test data folder, we have provided each day's data for each user. If you open the files you can see that the data contains: id (label id), user_id(nurse/caregiver), activity_type_id(unique id for each activity type), activity_type (activity name), target_id (patients), activity2user_id, start and finish timestamp of the activity and year-month-date-hour timestamp.

<p>
  <img src="/challenge2022/assets/images/test_data_sheet.png" width="900" class="center"/>
</p>

If you want you can match it with the accelerometer data that was provided. Participants should note that the start and finish time at the care record file may differ from the datetime at the accelerometer file due to the different time zone settings.

Participants are required to propose their pipelines, predict and submit the activity label for the testing dataset as shown in the  [tutorial](https://colab.research.google.com/drive/1euqLhhsb21bbOETWMY9DkUcue6t33j1j?usp=sharing). The test submission folder contains test time stamps that you need to predict for each user. The files contain time stamps, and activity_type_ids and the columns are filled up with zero as shown in Table 3 below.

![Table3](/challenge2022/assets/images/Table3.png)

The participants are required to put 1 in place of 0 when the activity is supposed to happen and regenerate the files. Please make sure to maintain the shape same as the provided files(any changes that occurred in the submission are not the liability of the organizers, please make sure that there is no difference in shape and activity_type_id  with the given file)


## Data use
All participants may use the data free of charge.
[Download the dataset](https://ieee-dataport.org/competitions/nurse-care-activity-recognition-challenge-datasets-2022-0)

## Result Submission
Please submit your results via the submission form. [Access the Submission Form here](https://forms.gle/cDEhfHQjiSGKP5Zh6)


<!-- 
![Table1](/challenge2022/assets/images/Table1.png)
![TrainData](/challenge2022/assets/images/TrainData.png)
![Accelerometer](/challenge2022/assets/images/Accelerometer.png)
![Accel_sheet](/challenge2022/assets/images/Accel_sheet.png)
![Care_record_folder](/challenge2022/assets/images/Care_record_folder.png)
![Care_rec_sheet](/challenge2022/assets/images/Care_rec_sheet.png)
![Test_data](/challenge2022/assets/images/Test_data.png)
![test_data_sheet](/challenge2022/assets/images/test_data_sheet.png)


Here A1, A2, A3, and A4 represents the activity_type_id and year-month-date-hour column values should be same the values given in the text file(any changes occurred in the submission is not the liability of the organizers, please make sure that there is no difference in the timestamp with the given file). The 1 shown in table 3 defines that that activity occurred in that certain hour. More explanations can be found in the tutorial.


If you open the files you can see that the data contains: id (label id), user_id(nurse/caregiver), activity_type_id(unique id for each activity type), activity_type (activity name), target_id (patients), activity2user_id, start and finish timestamp of the activity and year-month-date-hour timestamp.

<p>
  <img src="/challenge2022/assets/images/Care_rec_sheet.png" width="850" class="center"/>
</p>

The accelerometer data has been collected using one smartphone carried by subjects, which are caregivers and nurses, when they were conducting daily works at a healthcare facility. The smartphone was carried in an arbitrary position such as a pocket. There are a total of 27 activities divided into 4 groups. All the activities are listed per category below.

<style>
tr,
td {
    border: none;
}

</style>
<table style="border: none">
  <tr>
    <th style="text-align: left"><h3>Activities of direct care</h3></th>
  </tr>
    <tr><td>1: Vital</td></tr>
    <tr><td>7: Morning gathering/ exercises</td></tr>
    <tr><td>13: Family/guest response</td></tr>
    <tr><td>2: Meal/medication</td></tr>
    <tr><td>8: Rehabilitation / recreation</td></tr>
    <tr><td>14: Outing response</td></tr>
    <tr><td>3: Oral care</td></tr>
    <tr><td>9: Morning care</td></tr>
    <tr><td>19: Get up assistance</td></tr>
    <tr><td>4: Excretion</td></tr>
    <tr><td>10: Daytime user response</td></tr>
    <tr><td>20: Change dressing assistance</td></tr>
    <tr><td>5: Bathing/wiping</td></tr>
    <tr><td>11: Night care</td></tr>
    <tr><td>21: Washing assistance</td></tr>
    <tr><td>6: Treatment</td></tr>
    <tr><td>12: Nighttime user response</td></tr>
    <tr><td>27: Emergency response such as accident</td></tr>
</table>

<table>
  <tr>
    <th style="text-align: left"><h3>Activities of residence cleaning</h3></th>
  </tr>
    <tr><td>15: Linen exchange</td></tr>
    <tr><td>23: Preparation and checking of goods</td></tr>
    <tr><td>24: Organization of medications</td></tr>
    <tr><td>16: Cleaning</td></tr>
</table>

<table>
  <tr>
    <th style="text-align: left"><h3>Documentation/Communication activities</h3></th>
  </tr>
    <tr><td>17: Handwriting recording</td></tr>
    <tr><td>22: Doctor visit correspondence</td></tr>
    <tr><td>25: Family/doctor contact</td></tr>
    <tr><td>18: Delegating/meeting</td></tr>
</table>

<table>
  <tr>
    <th style="text-align: left"><h3>Other activities</h3></th>
  </tr>
    <tr><td>26: Break</td></tr>
    <tr><td>28: Special remarks/notes</td></tr>
</table>


## Data structure
The training and testing dataset contains accelerometer data and care record data of 5 users ( 8, 13, 14, 15, 25), which were collected on May and June, 2018. Training and testing data were separated in 70~30 ratio based on each user data.

The provided each user folder includes the accelerometer data files for whole time, training care record file and testing care record file. In training care record we have activity information but in testing care record we remove it. Your work is to predict these activities and generate files.

In each accelerometer data file, we have 4 columns: datetime and 3 coordinates of the accelerometer data.

![data-acc](/nurse2021/assets/data-acc.png)

In the care record file, we have 12 columns: id (label id), user_id, role, activity_type_id, activity_type (name in japanese), activity_type_e (name in english), date, start time, finish time (of the activity), target_id (patients), target_role, activity2user_id. Participants should note that the start and finish time at the label_train file may differ from the datetime at the accelerometer file due to the different time zone.



## Test Data Setting
This dataset was used in our previous work, titled [“Integrating Activity Recognition and Nursing Care Records: The System, Deployment, and a Verification Study”](https://dl.acm.org/doi/abs/10.1145/3351244). The authors of this work proposed a theory that  extension of start and ending time of the activities can increase the prediction rate. The reason behind the theory is that many of the nurses provided the labels before or after completing an activity. In the paper they verified and proved this theory. Following the theory, in the test data the time is extended for both start and end of an activity for 20 minutes. As the time is extended, there are some overlaps for the activity labels for some samples. So, the submission of the participants will be evaluated per activity following the same test setting as the paper. The final score will be calculated by taking the prediction average of all the activities.
--->

