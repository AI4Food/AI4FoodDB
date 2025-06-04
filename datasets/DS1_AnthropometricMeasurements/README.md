# DS1 - Anthropometric Measurements

### Health Professional Data

This dataset contains anthropometric measurements collected by a healthcare professional during three key visits: **V0 (baseline)**, **V2 (mid-intervention)**, and **V3 (end of intervention)**. The data is stored in the [`anthropometrics.csv`](https://github.com/AI4Food/AI4FoodDB/blob/master/datasets/DS1_AnthropometricMeasurements/anthropometric_measurements.csv) file and includes the following fields:

-   `id`: **Anonymized Participant ID** in the format `A4F_XXXXX`.
    
-   `visit`: **Visit Code** indicating when the measurements were taken. Possible values are:
    
    -   `0`: Baseline (V0)
        
    -   `2`: Mid-intervention (V2)
        
    -   `3`: End of intervention (V3)
        
-   `period`: **Menstrual Period Status**. A value of `1` indicates the participant was experiencing their menstrual period or the days immediately preceding it at the time of measurement; `0` otherwise.
    
-   `current_weight_kg`: **Current Weight**, measured during the visit, in kilograms (kg).
    
-   `bmi_kg_m2`: **Body Mass Index (BMI)**, calculated during the visit, in kilograms per square meter ($kg/m^2$).
    
-   `fat_mass_perc`: **Body Fat Percentage** (%).
    
-   `muscle_mass_perc`: **Muscle Mass Percentage** (%).
    
-   `visceral_fat_level`: **Visceral Fat Level**, as assessed by the nutritionist.
    
-   `basal_metabolism`: **Basal Metabolic Rate**, estimated in kilocalories (kcal).
    
-   `waist_cm`: **Waist Circumference**, measured in centimeters (cm).
    
-   `hip_cm`: **Hip Circumference**, measured in centimeters (cm).

