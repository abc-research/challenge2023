---
layout: single
title: About the Fourth Nurse Care Activity Recognition Challenge
permalink: /learn/
date: 2022-07-1T00:00:00+09:00
---

Human Activity Recognition (HAR) is the process of handling information from sensors and/or video capture devices under certain circumstances to correctly determine human activities. Traditionally, the HAR can be achieved by human observation through the visualization of video recording devices. However, it is time and labor consuming. Nowadays, this traditional way could be replaced by other simple and automatic methods based on sensors and Artificial Intelligence platforms. For instance, your smartphone or other smart wearable devices have the ability to recognize some of your movements such as walking or running based on the inside accelerometer sensor.

In addition, HAR has several remarkable applications in the real world, especially in the healthcare field. Besides the elderly/patient’s activity monitoring, the caregiver’s activity recognition plays an important role to improve the healthcare quality. Moreover, specifically in developed countries, the number of the elderly increases rapidly due to population aging, while the number of nurses can not satisfy. The greater the pressure on nurses, the more uncertain the healthcare quality is. Therefore, nurse care activity recognition is implemented to help the caregiver/nurse well manage and improve the quality of their work. In this challenge, based on the accelerometer data collected from the smartphone, the cheapest and easy-to-implement way, we aim to recognize the daily nurse care activities taking place at the nursing care facility.

## Challenge Goal 
The goal of this year’s Nurse Care Activity Recognition Challenge is to predict the hourly activities of a caregiver/nurse in a healthcare facility based on the care records file and accelerometer data collected from smartphones. Along with the time data from the care records we expect participants to utilize accelerometer data to predict the future occurrence of the activities (future prediction). The activity labels can be found in care record files. Participants should suggest ways for extracting features from these data, using alternative windowing approaches if possible, and then feeding them into their own model. Finally, each team needs to use their model to predict the activity followed by the timestamp in the test data. You can check out the basic [HAR tutorial here](https://abc-research.github.io/nurse2021/tutorial/tutorial.html).

- [Check the tutorial here](https://colab.research.google.com/drive/1A4zSOSO0IXwc-iB9EFdOr6mUP85KAxFm?usp=sharing)
- [To understand the dataset more clearly](/challenge2022/data/)
- [Download the dataset](https://ieee-dataport.org/competitions/nurse-care-activity-recognition-challenge-datasets-2022-0)

Time mismatch is part of the challenge. You need to think of ways to utilize as much as data possible. Our main focus is the care record data and accelerometer data is given as auxiliary information. The participants can use both or either of the data provided.


<!--edit this part
The training and testing dataset contains accelerometer data and care record data of 5 users ( 8, 13, 14, 15, 25), which were collected on May and June, 2018. Training and testing data were separated in 70~30 ratio based on each user data. Participants are required to propose their pipelines, predict and submit the activity label for the testing dataset.


The goal of the Nurse Care Activity Recognition Challenge is to recognize the daily activities of a caregiver/nurse in a healthcare facility based on the accelerometer data collected from smartphones. Participants utilize accelerometer data and its activity labels in training files, propose the methods to extract features from these data, and then feed to their own model. Finally, each team needs to use their model to predict the activity based on the accelerometer data following by the timestamp in the test data. 



The training and testing dataset contains accelerometer data of 12 users (2, 3, 4, 5, 6, 7, 9, 12, 17, 19, 21, and 22), which were collected on May and June, 2018. The training data is provided with the activities labels, which describe the users’ activities before 18th June, 2018. The testing data was the accelerometer data acquired on 18th June and afterward. Participants are required to propose their pipelines, predict and submit the activity label for the testing dataset.
-->

<!--old
## Evaluation
Accuracy will be used as the performance measure.
Submissions will be evaluated by the average of the accuracy of macro activity classification (ma) and the average accuracy of micro-activity classification (mi). That is (ma+mi)/2.

The average accuracy of micro-activity classification is based on the multi-label accuracy formula. The accuracy of one sample is given by the number of correct labels predicted divided by the number of total true and predicted labels (cardinality of the union). 
-->
## Evaluation
Participants are required to propose their pipelines, predict and submit the activity label for the testing dataset as shown in the [tutorial](https://colab.research.google.com/drive/1euqLhhsb21bbOETWMY9DkUcue6t33j1j?usp=sharing). The test submission folder contains test time stamps that you need to predict for each user. The files contain time stamps, and activity_type_ids and the columns are filled up with zero as shown in Table 3 below.

![Table3](/challenge2022/assets/images/Table3.png)

The participants are required to put 1 in place of 0 when the activity is supposed to happen and regenerate the files. Please make sure to maintain the shape same as the provided files(any changes that occurred in the submission are not the liability of the organizers, please make sure that there is no difference in shape and activity_type_id with the given file). 

As shown in Table 3, we expect the participants to generate 5 similar files one for each user, and submit them to us. As the occurrence of activities differs in different users we will match with label files of each user and see how many activities were accurately identified to have occurred by the participants.

For evaluation along with counting the percentage of how many activities were predicted for each user, we will also consider Precision, Recall, and F1 Score. We will take an average of all the scores of all the users.The baseline result for each user is shared in the table below.


![Table4](/challenge2022/assets/images/Table4.png)


## Result Submission
Please submit your results via the submission form. [Access the Submission Form here](https://forms.gle/cDEhfHQjiSGKP5Zh6)

## Data use
All participants may use the data free of charge. [Download the dataset](https://ieee-dataport.org/competitions/nurse-care-activity-recognition-challenge-datasets-2022-0)


## Prizes
- The winning team will be awarded 100,000 jpy.
- The registration fee for the 1st and 2nd runner-up teams will be waived.
- Each of the participating teams will be awarded with participation certificate.

