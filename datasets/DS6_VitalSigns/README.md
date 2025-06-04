# DS6 - Vital Signs

### Health Professional Data

#### Vital Signs

The file [`vital_signs.csv`](https://github.com/AI4Food/AI4FoodDB/blob/master/datasets/DS6_VitalSigns/vital_signs.csv) contains vital signs measured by healthcare professionals during nutritionist visits at various stages of the study:

-   `id`: **Anonymized Participant ID**, formatted as `A4F_XXXXX`.
    
-   `visit`: **Visit code** indicating the timepoint of measurement:
    
    -   `0`: Baseline (V0)
        
    -   `2`: Mid-intervention (V2)
        
    -   `3`: End of intervention (V3)
        
-   `systolic_blood_pressure_mmhg`, `diastolic_blood_pressure_mmhg`: Systolic and diastolic blood pressure, measured in mmHg.
    
-   `heart_rate_bpm`: Heart rate, measured in beats per minute (bpm).
    

----------
### Digital Data

#### Heart Rate

This subdirectory contains continuous heart rate recordings collected from participants during the 14-day digital data collection period. Each file is named `A4F_XXXXX_heart_rate.csv` and contains heart rate values sampled approximately every 5 to 10 seconds.

Each file includes:

-   `timestamp`: **Timestamp of the heart rate reading**, formatted as `YYYY-MM-DD HH:MM:SS+Z`.
    
-   `heart_rate`: **Heart rate**, measured in beats per minute (bpm).
    

#### [Electrocardiogram (ECG)](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS6_VitalSigns/electrocardiogram)

This subdirectory includes electrocardiogram session data for each participant, stored in files named `A4F_XXXXX_electrocardiogram.csv`. Each file documents ECG sessions conducted during the digital data collection period.

Each file includes:

-   `timestamp`: **Timestamp of the ECG session**, in the format `YYYY-MM-DD HH:MM:SS+Z`.
    
-   `result_classification`: **Outcome of the ECG session**, typically "Normal Sinus Rhythm (NSR)", "Atrial Fibrillation (AF)",  or "Unclassifiable" (in cases of low signal quality or indeterminate rhythm).
    
-   `average_heart_rate`: **Average heart rate** during the ECG session (bpm).
    
-   `heart_rate_alert`: **Alert flag** indicating any abnormalities in heart rate detected during the session.
    
-   `waveform_samples`: A list of raw data samples representing the complete ECG waveform captured during the session.
