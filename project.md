# Course Project -- American Epilepsy Society Seizure Prediction Challenge


## Null Hypothesis
It's not possible to accurately classify preictal brain states in dogs and humans.

## Alternative Hypothesis
The preictal brain state in dogs and humans does exist and can be accurately classified with naturally occurring epilepsy.

## Background: [Kaggle Competition - Seizure Prediction Challenge](http://www.kaggle.com/c/seizure-prediction)
Seizure forecasting systems have the potential to help patients with epilepsy lead more normal lives. In order for EEG-based seizure forecasting systems to work effectively, computational algorithms must reliably identify periods of increased probability of seizure occurrence. If these seizure-permissive brain states can be identified, devices designed to warn patients of impeding seizures would be possible. Patients could avoid potentially dangerous activities like driving or swimming, and medications could be administered only when needed to prevent impending seizures, reducing overall side effects.

There is emerging evidence that the temporal dynamics of brain activity can be classified into 4 states: Interictal (between seizures, or baseline), Preictal (prior to seizure), Ictal (seizure), and Post-ictal (after seizures). Seizure forecasting requires the ability to reliably identify a preictal state that can be differentiated from the interictal, ictal, and postictal state. The primary challenge in seizure forecasting is differentiating between the preictal and interictal states.


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




## Data Issues

## Plan
* Create 5 Dog tables and 2 Patient tables.
* Load tables with preictal and interictal data.
* Add ictal_ind flag to records where ictal_ind = 1 if record comes from preictal file else 0



