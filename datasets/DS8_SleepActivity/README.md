# DS8 - Sleep Activity

Sleep-related data was collected through both manual assessments and digital recordings using a smartwatch device.

----------

### Manual Data

Sleep habits were manually assessed using the [**Oviedo Sleep Questionnaire (OSQ)**](https://github.com/AI4Food/AI4FoodDB/blob/master/datasets/DS8_SleepActivity/OviedoSleepQuestionnaire.csv) at two timepoints: the beginning and the end of the traditional-based intervention. The OSQ is a semi-structured interview that facilitates the diagnosis of insomnia and hypersomnia over the past month, based on DSM-IV and ICD-10 criteria.

Data is stored in the `OviedoSleepQuestionnaire.csv` file and includes the following parameters for each participant:

-   `id`: **Anonymized Participant ID**, formatted as `A4F_XXXXX`.
    
-   `visit`: **Visit code**, indicating the timepoint of data collection:
    
    -   `0`: Baseline (V0)
        
    -   `2`: Mid-intervention (V2)
        
    -   `3`: End of intervention (V3)
        

**Main questionnaire items:**

-   `1_satisfaction_sleep`: General satisfaction with sleep.
    
-   `2_1_initiate_sleep`: Difficulty initiating sleep.
    
-   `2_2_remain_asleep`: Difficulty remaining asleep.
    
-   `2_3_restorative_sleep`: Perceived restorative quality of sleep.
    
-   `2_4_usual_waking_up`: Usual time of waking up.
    
-   `2_5_excessive_somnolence`: Daytime sleepiness or drowsiness.
    
-   `3_fall_asleep`: Time needed to fall asleep.
    
-   `4_wake_up_night`: Number of nocturnal awakenings.
    
-   `5_wake_up_earlier`: Frequency of waking up earlier than desired.
    
-   `6a_hours_sleep`: Total hours of sleep per night.
    
-   `6b_hours_bed`: Total time spent in bed.
    
-   `6c_sleep_efficiency`: Sleep efficiency (ratio of sleep time to time in bed).
    
-   `7_tiredness_not_sleep`: Daytime tiredness not related to sleep duration.
    
-   `8_somnolence_days`: Number of days with excessive somnolence.
    
-   `9_somnolence_effects`: Impact of somnolence on daily functioning.
    
-   `10a_snoring`: Frequency of snoring.
    
-   `10b_snoring_suffocation`: Perceived breathing interruptions during sleep.
    
-   `10c_leg_movements`: Leg movements during sleep.
    
-   `10d_nightmares`: Frequency of nightmares.
    
-   `10e_others`: Other sleep disturbances.
    
-   `11_sleep_aids`: Use of sleep aids or medications.
    

**Derived scores:**

-   `sleep_satisfaction_score`: Score summarizing satisfaction-related items.
    
-   `insomnia_score`: Score reflecting insomnia symptoms.
    
-   `somnolence_score`: Score for daytime sleepiness.
    
-   `total_score`: Overall sleep disturbance score.

----------
### Digital Data

Sleep activity was also monitored digitally using smartwatch devices, which continuously recorded sleep-related parameters throughout the intervention. The digital data is organized into six main components:

----------

#### [Additional Sleep Data](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS8_SleepActivity/additional_sleep_data)

The `additional_sleep_data` directory contains detailed nightly sleep reports for each participant. Each file is named `A4F_XXXXX_additional_sleep_data.csv` and includes information about sleep timing and duration across different sleep stages (deep, light, and REM):

-   `sleep_id`: Unique identifier for the sleep session.
    
-   `start_time`: Sleep start time in the format `YYYY-MM-DD HH:MM:SS+Z`.
    
-   `end_time`: Wake-up time in the format `YYYY-MM-DD HH:MM:SS+Z`.
    
-   `duration`: Total duration of the sleep session.
    
-   `minutes_asleep`: Total minutes asleep.
    
-   `minutes_awake`: Total minutes awake during the session.
    
-   `minutes_in_bed`: Total minutes spent in bed.
    
-   `main_sleep`: Indicates whether the session corresponds to the main nighttime sleep (`True`) or to naps/secondary sessions (`False`).
    
-   `minutes_in_deep_sleep`: Duration of deep sleep stage.
    
-   `minutes_in_light_sleep`: Duration of light sleep stage.
    
-   `minutes_in_rem`: Duration of REM sleep stage.
    

----------

#### [Heart Rate Variability](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS8_SleepActivity/heart_rate_variability)

The `heart_rate_variability` directory contains data on heart rate dynamics during sleep. Each file is named `A4F_XXXXX_heart_rate_variability.csv` and includes nightly measurements of autonomic nervous system activity:

-   `timestamp`: Timestamp of the measurement in the format `YYYY-MM-DD HH:MM:SS+Z`.
    
-   `rmssd`: Root Mean Square of the Successive Differences—an index of short-term heart rate variability.
    
-   `nrem_hr`: Average heart rate during non-REM (NREM) sleep stages.
    
-   `entropy`: A measure of heart rate signal complexity during the night.


#### [Oxygen Saturation](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS8_SleepActivity/oxygen_saturation)

The `oxygen_saturation` directory contains nightly measurements of blood oxygen saturation levels for each participant. Data is split into two files per participant:

-   **`A4F_XXXXX_daily_oxygen_saturation.csv`**: Contains nightly summary statistics of oxygen saturation.
    
    -   `timestamp`: Timestamp of the measurement in the format `YYYY-MM-DD HH:MM:SS+Z`.
        
    -   `sleep_average_oxygen_saturation`: Average oxygen saturation during sleep.
        
    -   `lower_bound_oxygen_saturation`: Minimum oxygen saturation recorded during sleep.
        
    -   `upper_bound_oxygen_saturation`: Maximum oxygen saturation recorded during sleep.
        
-   **`A4F_XXXXX_oxygen_saturation_by_minute.csv`**: Contains minute-by-minute oxygen saturation data throughout the night.
    
    -   `timestamp`: Timestamp of the measurement in the format `YYYY-MM-DD HH:MM:SS+Z`.
        
    -   `oxygen_saturation_by_minute`: Oxygen saturation percentage measured at each minute.
        

----------

#### [Respiratory Rate](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS8_SleepActivity/respiratory_rate)

The `respiratory_rate` directory contains data on breathing rates during sleep, recorded in breaths per minute. Each file is named `A4F_XXXXX_respiratory_rate.csv` and includes average breathing rates across different sleep stages for each night:

-   `timestamp`: Timestamp of the measurement in the format `YYYY-MM-DD HH:MM:SS+Z`.
    
-   `full_sleep_breathing_rate`: Average breathing rate during the full sleep session.
    
-   `full_sleep_standard_deviation`: Standard deviation of breathing rate during the full sleep session.
    
-   `full_sleep_signal_to_noise`: Signal-to-noise ratio for the full sleep session.
    
-   `deep_sleep_breathing_rate`: Average breathing rate during deep sleep.
    
-   `deep_sleep_standard_deviation`: Standard deviation during deep sleep.
    
-   `deep_sleep_signal_to_noise`: Signal-to-noise ratio during deep sleep.
    
-   `light_sleep_breathing_rate`: Average breathing rate during light sleep.
    
-   `light_sleep_standard_deviation`: Standard deviation during light sleep.
    
-   `light_sleep_signal_to_noise`: Signal-to-noise ratio during light sleep.
    
-   `rem_sleep_breathing_rate`: Average breathing rate during REM sleep.
    
-   `rem_sleep_standard_deviation`: Standard deviation during REM sleep.
    
-   `rem_sleep_signal_to_noise`: Signal-to-noise ratio during REM sleep.
    

----------

#### [Skin Temperature](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS8_SleepActivity/skin_temperature)

The `skin_temperature` directory contains two types of files that monitor temperature fluctuations on the wrist throughout the day and night:

-   **`A4F_XXXXX_wrist_temperature.csv`**: Records minute-by-minute variations in wrist temperature.
    
    -   `timestamp`: Timestamp of the measurement in the format `YYYY-MM-DD HH:MM:SS+Z`.
        
    -   `temperature_difference`: Minute-level difference in wrist temperature.
        
-   **`A4F_XXXXX_computed_temperature.csv`**: Provides nightly computed temperature features during sleep periods.
    
    -   `start_sleep`: Start time of the sleep period.
        
    -   `end_sleep`: End time of the sleep period.
        
    -   `temperature_samples`: Number of temperature readings collected during sleep.
        
    -   `nightly_temperature`: Average nightly skin temperature.
        
    -   `baseline_relative_sample_sum`: Sum of temperature differences relative to baseline.
        
    -   `baseline_relative_sample_sum_of_squares`: Sum of squared differences relative to baseline.
        
    -   `baseline_relative_nightly_standard_deviation`: Nightly standard deviation of relative temperature.
        
    -   `baseline_relative_sample_standard_deviation`: Standard deviation of all temperature samples relative to baseline.
    
#### [Sleep Quality](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS8_SleepActivity/sleep_quality)

The `sleep_quality` directory contains nightly sleep quality assessments for each participant. Data is stored in files named `A4F_XXXXX_sleep_quality.csv`, and includes a variety of sleep quality-related features such as start and end times, overall sleep quality scores, and detailed subscores. The scores include composition, revitalization, and duration components. Additionally, the file records the participant’s resting heart rate during sleep and their level of restlessness.

-   `sleep_id`: Unique identifier for each sleep record.
    
-   `start_time`: Timestamp indicating when the sleep session started in the format `YYYY-MM-DD HH:MM:SS+Z`.
    
-   `end_time`: Timestamp indicating when the sleep session ended in the format `YYYY-MM-DD HH:MM:SS+Z`.
    
-   `overall_score`: Composite score representing the overall quality of sleep.
    
-   `composition_score`: Score reflecting the balance and structure of sleep stages.
    
-   `revitalization_score`: Score indicating how refreshing the sleep was.
    
-   `duration_score`: Score based on the total duration of sleep.
    
-   `resting_heart_rate`: Average heart rate while at rest during sleep.
    
-   `restlessness`: Measure of movement or disruptions during sleep.
