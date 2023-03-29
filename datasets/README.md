# AI4FoodDB Datasets
This directory contains the available datasets from AI4FoodDB stored in tab-delimited files. 

- Every table contains an `id` column indicating the anonymized participant ID.
- A `dataset_id` is also included in all datasets with the form `dsX_[vX]_ID`: dataset number, visit number if the measurement was taken more than once, and participant ID. For instance:
    - `ds1_v0_1045` is the dataset ID for the information from dataset 1 recorded at V0 for participant 1045. 
    - `ds2_1045` is the dataset ID for the information from dataset 1 for participant 1045.
- Missing values are stored as `NA` in all cases.

## Table of Contents
* [Participant Information](#participant-information)
* [DS1: Anthropometric Measurements](#ds1-anthropometric-measurements)
* [DS2: Lifestyle and Health](#ds2-lifestyle-and-health)
* [DS4: Biomarkers](#ds4-biomarkers)
* [DS6: Vital Signs](#ds6-vital-signs)

## Participant Information
File `participant.tsv` stores the basic information for each participant: 

- `id`: Anonymized participant ID.
- `group`: Intervention group. Particiants from group 1 started with the traditional/manual data collection methods and then switched to digital data collection. Participants from group 2 started with digital data collection methods and then switched to traditional/manual data collection.
- `sex`: Participant's sex.
- `usual_weight_kg`: Participant's usual weight, measured in kilograms.
- `weight_5years_kg`: Participant's weight 5 years ago, measured in kilograms.
- `height_cm`: Participant's height, measured in cm.
- `intervention_diet_kcal`: Recommended daily calorie intake for the particpant, measured in kilocalories.
- `finished_intervention`: This column has a value of `1` if the participat completed the intervention and `0` otherwise.

## DS1: Anthropometric Measurements
This dataset contains the anthropometric measurements collected during visits V0, V2, and V3. File `anthropo.tsv` stores the following information:

- `id`: Anonymized participant ID.
- `visit`: Visit when the measurements were taken, either `0`, `2`, or `3`.
- `dataset_id`: Dataset ID.
- `period`: `1` if the participant was undergoing their period or at the previous days to their period, and `0` otherwise. 
- `current_weight_kg`: Participant's weight measured during the nutritionist visit, in kilograms.
- `bmi_kg_m2`: Participant's Body Mass Index (BMI) at the nutritionist visit, measured in $kg/m^2$.
- `fat_mass_perc`, `muscle_mass_perc`: Participant's percentage of fat mass and muscle mass, respectively.
- `visceral_fat_level`: Participant's visceral fat level.
- `basal_metabolism`: Participant's basal metabolism, measured in kilocalories.
- `waist_cm`: Participant's waist circumference, measured in cm.
- `hip_cm`: Participant's hip circumference, measured in cm.

## DS2: Lifestyle and Health
### Lifestyle
Lifestyle information is stored at `lifestyle.tsv`:


## DS4: Biomarkers

## DS6: Vital Signs
