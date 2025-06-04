
# DS7 - Physical Activity

This dataset contains both manually reported and digitally collected information on participants' physical activity throughout the study period.

----------

### Manual Data

#### [International Physical Activity Questionnaire (IPAQ)](https://github.com/AI4Food/AI4FoodDB/blob/master/datasets/DS7_PhysicalActivity/IPAQ.csv)

Participants completed the self-reported International Physical Activity Questionnaire (IPAQ), which includes questions about physical activity performed over the past few days. This questionnaire calculates multiple scores based on activity intensity and duration. The data is stored in the `IPAQ.csv` file and includes the following variables:

-   `id`: **Anonymized Participant ID**, formatted as `A4F_XXXXX`.
    
-   `visit`: **Visit code**, indicating the timepoint of data collection:
    
    -   `0`: Baseline (V0)
        
    -   `2`: Mid-intervention (V2)
        
    -   `3`: End of intervention (V3)
        
-   `vigorous_n_days`: Number of days with vigorous activity.
    
-   `vigorous_min_day`: Minutes per day of vigorous activity.
    
-   `vigorous_met`: Metabolic Equivalent of Task (MET) value for vigorous activity.
    
-   `moderate_n_days`: Number of days with moderate activity.
    
-   `moderate_min_day`: Minutes per day of moderate activity.
    
-   `moderate_met`: MET value for moderate activity.
    
-   `walking_n_days`: Number of days with walking activity.
    
-   `walking_min_day`: Minutes per day of walking.
    
-   `walking_met`: MET value for walking activity.
    
-   `total_met`: Total MET-minutes/week across all activities.
    
-   `categorical_score`:  Represents the overall activity level (low, moderate, or high), calculated from the total MET values. Each activity is converted into **MET-minutes** and participants are categorized as follows:

-   **Low**: <600 MET-min/week
    
-   **Moderate**: ≥600 MET-min/week, meeting minimum activity thresholds
    
-   **High**: ≥1500 MET-min/week (or ≥3000 MET-min/week, depending on activity intensity)
    

----------

### Digital Data

#### [Active Minutes](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS7_PhysicalActivity/active_minutes)

The `active_minutes` directory contains files named `A4F_XXXXX_active_minutes.csv`, which detail the number of minutes spent at various physical activity levels. The data distinguishes between activity during exercise (fat burn, cardio, and peak minutes) and general activity throughout the day (sedentary, lightly active, moderately active, and very active minutes):

-   `timestamp`: **Timestamp of the ECG session**, in the format `YYYY-MM-DD HH:MM:SS+Z`.
    
-   `fat_burn_minutes`: Minutes in the fat burn zone.
    
-   `cardio_minutes`: Minutes in the cardio zone.
    
-   `peak_minutes`: Minutes in the peak zone.
    
-   `sedentary_minutes`: Time spent being sedentary.
    
-   `lightly_active_minutes`: Light activity duration.
    
-   `moderately_active_minutes`: Moderate activity duration.
    
-   `very_active_minutes`: Vigorous activity duration.
    

----------

#### [Additional Physical Activity Data](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS7_PhysicalActivity/additional_physical_activity_data)

The `additional_physical_activity_data` directory contains files named `A4F_XXXXX_additional_physical_activity_data.csv`, which include broader metrics on physical activity and exertion:

-   `timestamp`: **Timestamp of the ECG session**, in the format `YYYY-MM-DD HH:MM:SS+Z`.
    
-   `resting_heart_rate`: Resting heart rate (bpm).
    
-   `altitude`: Altitude variation (meters).
    
-   `calories`: Total calories burned.
    
-   `steps`: Steps taken.
    
-   `distance`: Distance covered (km).
    
-   `minutes_below_default_zone_1`, `minutes_in_default_zone_1`, `minutes_in_default_zone_2`, `minutes_in_default_zone_3`: Time spent in different custom-defined heart rate zones.
    

----------

#### [Estimated VO₂ Max](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS7_PhysicalActivity/estimated_VO2)

The `estimated_vo2` directory includes files named `A4F_XXXXX_estimated_vo2.csv`, estimating each participant’s VO₂ max—the maximum oxygen consumption during physical activity:

-   `timestamp`: **Timestamp of the ECG session**, in the format `YYYY-MM-DD HH:MM:SS+Z`.
    
-   `demographic_vo2_max`: Estimated VO₂ max based on demographic data.
    
-   `demographic_vo2_max_error`: Estimation error.
    
-   `filtered_demographic_vo2_max`: Smoothed VO₂ max estimate.
    
-   `filtered_demographic_vo2_max_error`: Error of the filtered estimate.
    

----------

#### [Physical Activity Reports](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS7_PhysicalActivity/physical_activity_reports)

The `physical_activity_reports` directory provides detailed summaries of individual physical activity sessions in files named `A4F_XXXXX_physical_activity_reports.csv`. Each file includes metrics such as duration, steps, calories, and heart rate data for different activity zones:

-   `timestamp`: **Timestamp of the ECG session**, in the format `YYYY-MM-DD HH:MM:SS+Z`.
    
-   `activity_name`: Name or type of the activity.
    
-   `average_heart_rate`: Mean heart rate during the activity.
    
-   `duration`, `active_duration`: Total and active duration (minutes).
    
-   `calories`: Calories burned.
    
-   `steps`: Steps taken during the activity.
    

**Heart Rate Zones (each with time, min/max HR, and calories burned):**

-   `sedentary_minutes`
    
-   `lightly_active_minutes`
    
-   `fairly_active_minutes`
    
-   `very_active_minutes`
    
-   `out_of_range_minutes`, `out_of_range_minimum_heart_rate`, `out_of_range_maximum_heart_rate`, `out_of_range_calories`
    
-   `fat_burn_minutes`, `fat_burn_minimum_heart_rate`, `fat_burn_maximum_heart_rate`, `fat_burn_calories`
    
-   `cardio_minutes`, `cardio_minimum_heart_rate`, `cardio_maximum_heart_rate`, `cardio_calories`
    
-   `peak_minutes`, `peak_minimum_heart_rate`, `peak_maximum_heart_rate`, `peak_calories`
