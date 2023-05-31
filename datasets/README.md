
# AI4FoodDB Datasets
This directory contains the available datasets from AI4FoodDB stored as tab-delimited files in the corresponding directory. 

- Every table contains an `id` column indicating the anonymized participant ID.
- A `dataset_id` is also included in all datasets with the form `dsX_[vX]_ID`: dataset number, visit number if the measurement was taken more than once, and participant ID. For instance:
    - `ds1_v0_1045` is the dataset ID for the information from dataset 1 recorded at V0 for participant 1045. 
    - `ds2_1045` is the dataset ID for the information from dataset 2 for participant 1045.
- Missing values are stored as `NA` in all cases.

## Table of Contents
* [Participant Information](#participant-information)
* [DS1: Anthropometric Measurements](#ds1-anthropometric-measurements)
* [DS2: Lifestyle and Health](#ds2-lifestyle-and-health)
* [DS3: Nutrition](#ds3-nutrition)
* [DS4: Biomarkers](#ds4-biomarkers)
* [DS6: Vital Signs](#ds6-vital-signs)

## Participant Information
File [`participant.csv`](participant.csv) stores the basic information for each participant: 

- `id`: Anonymized participant ID.
- `group`: Intervention group. Particiants from group 1 started with the traditional/manual data collection methods and then switched to digital data collection. Participants from group 2 started with digital data collection methods and then switched to traditional/manual data collection.
- `sex`: Participant's sex.
- `usual_weight_kg`: Participant's usual weight, measured in kg.
- `weight_5years_kg`: Participant's weight 5 years ago, measured in kg.
- `height_cm`: Participant's height, measured in cm.
- `intervention_diet_kcal`: Recommended daily calorie intake for the particpant, measured in kcal.
- `finished_intervention`: This column has a value of `1` if the participat completed the intervention and `0` otherwise.

## [DS1: Anthropometric Measurements](DS1_AnthropometricMeasurements)
This dataset contains the anthropometric measurements collected by a health professional during visits V0, V2, and V3. File [`anthropometric_measurements.csv`](DS1_AnthropometricMeasurements/anthropometric_measurements.csv) stores the following information:

- `id`: Anonymized participant ID.
- `visit`: Visit when the measurements were taken, either `0`, `2`, or `3`.
- `dataset_id`: Dataset ID.
- `period`: `1` if the participant was undergoing their period or at the previous days to their period, and `0` otherwise. 
- `current_weight_kg`: Participant's weight measured during the nutritionist visit, in kg.
- `bmi_kg_m2`: Participant's Body Mass Index (BMI) at the nutritionist visit, measured in $kg/m^2$.
- `fat_mass_perc`, `muscle_mass_perc`: Participant's percentage of fat mass and muscle mass, respectively.
- `visceral_fat_level`: Participant's visceral fat level.
- `basal_metabolism`: Participant's basal metabolism, measured in kcal.
- `waist_cm`: Participant's waist circumference, measured in cm.
- `hip_cm`: Participant's hip circumference, measured in cm.

## [DS2: Lifestyle and Health](DS2_LifestyleHealth)
### Lifestyle
Information from the lifestyle survey is stored at [`lifestyle.csv`](DS2_LifestyleHealth/lifestyle.csv):

- `id`, `dataset_id`: Participant and dataset ID.
- `appetite`: Appetite level on a scale from 1 to 5.
- `daily meals`, `meals_weekdays_out`, `meals_weekdays_home`, `meals_weekend_out`, `meals_weekend_home`: Number of meals per day, number of meals eaten or cooked at home or outside (i.e., at a restaurant) during weekdays and during the weekend.
- `defecation`, `urination`: Frequency of defecation (daily, every two days, or more) and urination (times per day).
- `water_ml`, `others_ml`: Amount of water and other liquids consumed during the day, in mililiters.
- `cigarettes_day`, `cigars_day`, `pipe_day`: Daily tobacco consumption in the form of cigarettes, cigars, or pipe.
- `alcohol`, `fermented_perc`, `distilled_perc`: Weekly alcohol consumption and relative amount of fermented and distilled alcohol consumed (from 0 to 1).
- `exercise`: Weekly exercise, measured as times per week.
- `stress`, `anxiety`, `depression`, `eating_disorder`, `others_psychological`: These columns have a value of `1` if the participant suffers from stress, anxiety, depression, an eating disorder, or any other psychological illness, and `0` otherwise.
- `no_psychological`: This column has a value of `1` if the participant does not suffer from any psychological illness and `0` otherwise.
- `sleep_weekdays`, `sleep_weekend`: Hours of sleep during weekdays and during the weekend.
- `insomnia`, `somnolence`: These columns have a value of `1` if the participant suffers from insomnia or somnolence and `0` otherwise.

### Health
File [`health.csv`](DS2_LifestyleHealth/health.csv) stores manually-acquired information about frequent medication intake and current diseases:

- `id`, `dataset_id`: Participant and dataset ID.
- `oral_contraceptive`, `ring_contraceptive`, `antidepressants`, `antiacids`, `antihistamines`, `antiinflamatory`, `iron`, `calcium`, `antihypertensives`, `thyroid_hormone`, `antibiotics`, `other_medication`: These columns have a value of `1` if the participant is currently consuming any of the listed medications, or a medication that is not included in this list, and `0` otherwise.
- `no_medication`: This column has a value of `1` if the participant is not taking any medication at the moment and `0` otherwise.
- `hyperthyroidism`, `hypothyroidism`, `hypercholesterolemia`, `triglyceridemia`, `hypertension`, `depression`, `diabetes`, `lactose_intolerance`, `other_illness`: These columns have a value of `1` if the participant suffers from any of the listed or any other illnesses, and `0` otherwise.
- `no_illness`: This column has a value of `1` if the participant does not suffer from any illness at the moment and `0` otherwise.
- `menopause`: This column has a value of `1` if the participant has reached menopause and `0` otherwise.

## [DS3: Nutrition](DS3_Nutrition)

Food images, including meals and drinks, from participants are available at the following [link](http://atvs.ii.uam.es/atvs/AI4FOOD/) due to the large size of the data. For more detail, please see the section [DS3: Nutrition](DS3_Nutrition).

## [DS4: Biomarkers](DS4_Biomarkers)
File [`biomarkers.csv`](DS4_Biomarkers/biomarkers.csv) stores information from several biochemical parameters, measured from biological samples:

- `id`, `visit`, `dataset_id`: Participant, visit where the measurement was taken, and dataset ID.
- `leukocytes_10e3_ul`, `plats_10e3_ul`, `lympho_10e3_ul`, `mono_10e3_ul`, `seg_10e3_ul`, `eos_10e3_ul`, `baso_10e3_ul`: Total number of leukocytes, platelets, lymphocytes, monocytes, segmenters, eosynophils, and basophils, measured as $10^3/\mu{L}$.
- `erythrocytes_10e6_ul`: Total erythrocyte number, measured as $10^6/\mu{L}$.
- `hgb_g_dl`: Hemoglobin concentration, measured in g/dL.
- `hematocrit_perc`: Hematocrit.
- `mcv_fl`, `mpv_fl`: Mean corpuscular volume (MCV) and mean platelet volume (MPV), measured in fL.
- `mch_pg`, `mchc_g_dl`: Mean corpuscular hemoglobin (MCH), measured in pg, and MCH concentration (MCHC), measured in g/dL.
- `rdw_perc`: Red cell distribution width.
- `lympho_perc`, `mono_perc`, `seg_perc`, `eos_perc`, `baso_perc`: Percentage of lymphocytes, monocytes, segmenters, eosynophils, and basophyls.
- `hba1c_perc`, `hba1ifcc_mmol_mol`: Glycated hemoglobin, measured as a percentage and in mmol/mol respectively.
- `insulin_uui_ml`: Insulin concentration, measured in $\mu{UI}/mL$.
- `homa`: HOMA-IR index.
- `glu_mg_dl`: Glucose concentration in mg/dL.
- `chol_mg_dl`, `tri_mg_dl`, `hdl_mg_dl`, `ldl_mg_dl`: Total cholesterol concentration, total triglycerides concentration, high-density lipoprotein (HDL) concentration and low-density lipoprotein (LDL) concentration, measured in mg/dL.
- `homocysteine_umol_l`: Homocysteine concentration, measured in $\mu{mol}/L$.
- `alb_g_dl`, `prealbumin_mg_dl`: Albumin and prealbumin concentrations, measured in g/dL and mg/dL respectively.
- `crp_mg_dl`: C-reactive protein concentration, measured in mg/dL.
- `igg_mg_dl`, `iga_mg_dl`, `igm_mg_dl`, `ige_ui_ml`: Concentrations of immunoglobulins (Ig) IgG, IgA, IgM, measured in mg/dL; and IgE, measured in UI/mL.
- `tnf_a_ui_ml`: TNF-$\alpha$ concentration, measured in UI/mL.
- `adiponectin_ug_ml`: Adiponectin concentration, measured in $\mu{g}/mL$.


## [DS6: Vital Signs](DS6_VitalSigns)
The vital signs measured by a health professional during the nutritionist visits are stored in [`vitalsigns.csv`](DS6_VitalSigns/vitalsigns.csv): 

- `id`, `visit`, `dataset_id`: Participant, visit where the measurement was taken, and dataset ID.
- `systolic_blood_pressure_mmhg`, `dyastolic_blood_pressure_mmhg`: Systolic and dyastolic blood pressure, measured in mmHg.
- `heart_rate_bpm`: Heart rate, measured in beats per minute (bpm).


