---
layout: single
title: ""
permalink: /faq/
date: 2022-07-14T00:00:00+09:00
---

# Frequently Asked Questions

Submit your questions to abc2022@sozolab.jp with the subject *Nurse Care Challenge 2022*.


You can also check the Tutorial page and recorded tutorial videos as most questions were discussed in there. 

<ul> 
<li><a href="https://colab.research.google.com/drive/1A4zSOSO0IXwc-iB9EFdOr6mUP85KAxFm?usp=sharing"><b>Link to the Tutorial Page</b></a></li>
<li><a href="https://youtu.be/pzuAXzRtkHg"><b>Link to the recorded Japanese Tutorial</b></a></li>
<li><a href="https://youtu.be/9djBag5QZqY"><b>Link to the recorded English Tutorial</b></a></li>
</ul>


## Previous Questions
**Why is there time mismatch in the accelerometer data?**
Time mismatch is part of the challenge. You need to think of ways to utilize as much as data possible. 

**Are we required to use both accelerometer and care record data?**
Our main focus is the care record data and accelerometer data is given as auxiliary information. The participants can use care record only or both data provided.

**Where can we find the test data?**
The test data is uploaded in the same IEEE port with the train data. Please check the Data page.


**What metrics can we check for the train data in preparation for test data evaluation?**
As per the submission form, you are required to specify training performance in terms of Precision, Recall, F1 score and Accuracy.

**Where can we submit the result?**
Check the link to the submission form below. Don't forget to use the file format uploaded in the IEEE dataport (filename Test Submission.zip) when uploading your results.


## Result Submission
Please submit your results via the submission form. [Access the Submission Form here](https://forms.gle/cDEhfHQjiSGKP5Zh6)



<!--
**What is the sampling rate of each device?**

The sampling rate for the accelerometers is a little bit variable as we used Android to collect the samples. Android operates sensors on a “best effort” policy, meaning that even if we set a desired sampling rate, the actual sampling rate will vary during the application time depending on other factors such as battery level or free memory.

That said,  the average sampling rate for the smartwatches (on each wrist) was about 100Hz and for the smartphones (hip and arm) was about 50Hz. That is why you might get different number of samples on the segments but they all represent 1 minute.

The sampling rate of motion capture is 100Hz.

**I noticed that the new Timestamp field is not always ascending for some sensors. How can we interpret this?**

The data is provided as was collected. In this case, the smartwatch transmits via bluetooth to the smartphone and, in some cases, data is missed or arrives late. The timestamp is the time of the measurement, so you can re-order based on it.
Also, we noticed the left-wrist sensor has many missing data, so please consider it.

**Some files have not label associated. There are 516 files but only 288 rows in the labels file**

We had an error in the published dataset but it has now been corrected and updated. Please download the latest version of the dataset.

**There are some duplicated files in the training data**

We had an error in the published dataset but it has now been corrected and updated. Please download the latest version of the dataset.

**Can you provide the names of the markers in motion capture data?**
The markers are in the following order:
Top.Head Front.Head Rear.Head R.Shoulder R.Offset R.Elbow R.Wrist L.Shoulder L.Elbow L.Wrist R.ASIS L.ASIS V.Sacral R.Thigh R.Knee R.Shank R.Ankle R.Heel R.Toe L.Thigh L.Knee L.Shank L.Ankle L.Heel L.Toe R.Knee.Medial R.Ankle.Medial L.Knee.Medial L.Ankle.Medial V_Mid_ASIS V_Pelvis_Origin V_R.Hip_JC V_L.Hip_JC V_R.Knee_JC_Static V_L.Knee_JC_Static V_R.Ankle_JC_Static V_L.Ankle_JC_Static V_R.Knee_JC V_L.Knee_JC V_R.Ankle_JC V_L.Ankle_JC V_Mid_Hip V_Mid_Shoulder V_R.Hand V_L.Hand V_R.Toe_Offset_Static V_L.Toe_Offset_Static V_R.Toe_Offset V_L.Toe_Offset

Notice that we use real markers until L.Toe and others are virtual markers (mainly missing, we should have removed them :S )  
-->
