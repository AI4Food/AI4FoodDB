# DS9 - Emotional State

### Manual Data

#### [DASS-21](https://github.com/AI4Food/AI4FoodDB/blob/master/datasets/DS9_EmotionalState/DASS-21.csv)

Participants completed the self-reported Depression, Anxiety, and Stress Scale (DASS-21), which assesses emotional wellbeing and mood status. The data is stored in the `DASS-21.csv` file and includes the following variables:

-   `id`: **Anonymized Participant ID**, formatted as `A4F_XXXXX`.
    
-   `visit`: **Visit code**, indicating the timepoint of data collection:
    
    -   `0`: Baseline (V0)
        
    -   `2`: Mid-intervention (V2)
        
    -   `3`: End of intervention (V3)
        
-   `1_wind_down`
    
-   `2_mouth_dryness`
    
-   `3_no_positive_feelings`
    
-   `4_difficulty_breathing`
    
-   `5_no_initiative`
    
-   `6_overreact`
    
-   `7_trembling`
    
-   `8_nervous_energy`
    
-   `9_panic`
    
-   `10_no_prospects`
    
-   `11_agitation`
    
-   `12_no_relax`
    
-   `13_downhearted`
    
-   `14_intolerance`
    
-   `15_close_to_panic`
    
-   `16_no_enthusiasm`
    
-   `17_selfworth`
    
-   `18_touchy`
    
-   `19_heart`
    
-   `20_scared`
    
-   `21_meaningless`
    
-   `depression_score`:
    
-   `stress_score`:
    
-   `anxiety_score`:
    
-   `total_score`:
    

----------

### Digital Data

During the two-week digital data collection period, emotional state was monitored through FitBit-generated stress indicators, including ElectroDermal Activity (EDA) sessions and derived daily stress scores.

#### [EDA Sessions](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS9_EmotionalState/eda_sessions)

The `eda_sessions` directory contains skin conductance levels recorded during EDA sessions. Data is stored in files named `A4F_XXXXX_eda_sessions.csv`, which include:

-   `timestamp`: Timestamp of the measurement in the format `YYYY-MM-DD HH:MM:SS+Z`.
    
-   `average_heart_rate`: Average heart rate during the session.
    
-   `start_heart_rate`: Heart rate at the beginning of the session.
    
-   `end_heart_rate`: Heart rate at the end of the session.
    
-   `hrv_baseline`: Baseline heart rate variability.
    
-   `skin_conductance_levels`: Skin conductance level recorded during the session.
    

#### [Stress Score](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS9_EmotionalState/stress_score)

The `eda_sessions` directory also contains daily stress management scores based on 10 physiological and behavioral factors, including sleep and heart rate data. These are stored in files named `A4F_XXXXX_stress_score.csv`, and include:

-   `timestamp`: Timestamp of the measurement in the format `YYYY-MM-DD HH:MM:SS+Z`.
    
-   `stress_score`: Overall daily stress score.
    
-   `sleep_points`: Score contribution from sleep quality and patterns.
    
-   `responsiveness_points`: Score contribution from physiological responsiveness.
    
-   `exertion_points`: Score contribution from physical exertion.
