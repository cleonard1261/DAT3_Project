# Course Project -- American Epilepsy Society Seizure Prediction Challenge


## Question
The goal of the competition is to demonstrate the existence and accurate classification of the preictal brain state in dogs and humans with naturally occurring epilepsy.

## Kaggle Link
[Kaggle - Seizure Prediction Challenge](http://www.kaggle.com/c/seizure-prediction)


## Data as described @ Kaggle

[Siezure Data](http://www.kaggle.com/c/seizure-prediction/data)

## Data Dictionary

| Fields               | Description   |
| -------------        |-------------  |
| data                 | a matrix of EEG sample values arranged row x column as electrode x time. |
| data_length_sec      | the time duration of each data row      |
| sampling_frequency   | the number of data samples representing 1 second of EEG data.  |
| channels             | a list of electrode names corresponding to the rows in the data field |
| sequence             | the index of the data segment within the one hour series of clips. For example, preictal_segment_6.mat has a sequence number of 6, and represents the iEEG data from 50 to 60 minutes into the preictal data. |

### Data Files

* preictal_segment_n.mat - the nth preictal training data segment
* interictal_segment_n.mat - the nth non-seizure training data segment
* test_segment_n.mat - the nth testing data segment

NOTE: where n goes from 0 to N  ==> N is the total number of data segments

### Directory Structure

```
├── PROJECT_DIR/data/
│   ├── Dog_1
│   │   ├── preictal_segment_0001.mat
│   │   ├── interictal_segment_0001.mat
│   │   ├── test_segment_0001.mat
|   |   ├── [...] 
│   │   ├── preictal_segment_N.mat
│   │   ├── interictal_segment_N.mat
│   │   ├── test_segment_N.mat
[...]
│   ├── Dog_5
│   │   ├── preictal_segment_0001.mat
│   │   ├── interictal_segment_0001.mat
│   │   ├── test_segment_0001.mat
|   |   ├── [...] 
│   │   ├── preictal_segment_N.mat
│   │   ├── interictal_segment_N.mat
│   │   ├── test_segment_N.mat
│   ├── Patient_1
│   │   ├── preictal_segment_0001.mat
│   │   ├── interictal_segment_0001.mat
│   │   ├── test_segment_0001.mat
|   |   ├── [...] 
│   │   ├── preictal_segment_N.mat
│   │   ├── interictal_segment_N.mat
│   │   ├── test_segment_N.mat
│   ├── Patient_2
│   │   ├── preictal_segment_0001.mat
│   │   ├── interictal_segment_0001.mat
│   │   ├── test_segment_0001.mat
|   |   ├── [...] 
│   │   ├── preictal_segment_N.mat
│   │   ├── interictal_segment_N.mat
│   │   ├── test_segment_N.mat
```




## Project Deliverables

* Problem statement and hypothesis
* Description of your data set and how it was obtained
* Description of any pre-processing steps you took
* What you learned from exploring the data, including visualizations
* How you chose which features to use in your analysis
* Details of your modeling process, including how you selected your models and validated them
* Your challenges and successes
* Possible extensions or business applications of your project
* Conclusions and key learnings




