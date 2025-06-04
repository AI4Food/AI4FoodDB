# DS2 - Lifestyle and Health

### Manual Data

#### Lifestyle

Information from the lifestyle questionnaire is available in the file [`lifestyle.csv`](https://github.com/AI4Food/AI4FoodDB/blob/master/datasets/DS2_LifestyleHealth/lifestyle.csv), which includes the following variables:

-   `id`: **Anonymized Participant ID** in the format `A4F_XXXXX`.
    
-   `appetite`: **Self-reported appetite level** on a scale from 1 (low) to 5 (high).
    
-   `daily meals`, `meals_weekdays_out`, `meals_weekdays_home`, `meals_weekend_out`, `meals_weekend_home`: **Meal patterns**, including:
    
    -   Total number of daily meals.
        
    -   Number of meals consumed or prepared **at home** or **outside** (e.g., restaurants) during **weekdays** and **weekends**.
        
-   `defecation`, `urination`: **Frequency of bowel movements** (e.g., daily, every two days) and **urination** (number of times per day).
    
-   `water_ml`, `others_ml`: **Daily fluid intake**, including water and other beverages, measured in milliliters (mL).
    
-   `cigarettes_day`, `cigars_day`, `pipe_day`: **Tobacco use**, recorded as the number of cigarettes, cigars, or pipe uses per day.
    
-   `alcohol`: **Total weekly alcohol consumption**, in servings.
    
-   `fermented_perc`, `distilled_perc`: **Proportion of alcohol intake** attributed to fermented (e.g., wine, beer) and distilled beverages (e.g., spirits), with values ranging from 0 to 1.
    
-   `exercise`: **Physical activity**, measured as the number of exercise sessions per week.
    
-   `stress`, `anxiety`, `depression`, `eating_disorder`, `others_psychological`: Binary indicators (`1` = yes, `0` = no) for **self-reported psychological conditions**, including stress, anxiety, depression, eating disorders, and other conditions.
    
-   `no_psychological`: Binary indicator for the **absence of psychological conditions** (`1` = no psychological condition reported, `0` = at least one reported).
    
-   `sleep_weekdays`, `sleep_weekend`: **Average hours of sleep** per night during **weekdays** and **weekends**, respectively.
    
-   `insomnia`, `somnolence`: Binary indicators (`1` = yes, `0` = no) for the presence of **insomnia** or **daytime sleepiness (somnolence)**.


#### Health

Manually reported information on medication use and current health conditions is provided in the file [`health.csv`](https://github.com/AI4Food/AI4FoodDB/blob/master/datasets/DS2_LifestyleHealth/health.csv), which includes the following variables:

-   `id`: **Anonymized Participant ID** in the format `A4F_XXXXX`.
    
-   `oral_contraceptive`, `ring_contraceptive`, `antidepressants`, `antiacids`, `antihistamines`, `antiinflamatory`, `iron`, `calcium`, `antihypertensives`, `thyroid_hormone`, `antibiotics`, `other_medication`: Binary indicators (`1` = yes, `0` = no) reflecting whether the participant is currently taking any of the listed medications or any **other unspecified medication**.
    
-   `no_medication`: Binary indicator (`1` = no medication currently taken, `0` = at least one medication currently taken).
    
-   `hyperthyroidism`, `hypothyroidism`, `hypercholesterolemia`, `triglyceridemia`, `hypertension`, `depression`, `diabetes`, `lactose_intolerance`, `other_illness`: Binary indicators (`1` = yes, `0` = no) for the presence of the specified **health conditions** or any **other illness** not explicitly listed.
    
-   `no_illness`: Binary indicator (`1` = no illness currently reported, `0` = at least one illness currently reported).
    
-   `menopause`: Binary indicator (`1` = participant has reached menopause, `0` = otherwise).
