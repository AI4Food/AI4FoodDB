# AI4FoodDB Datasets
This directory contains the available datasets from AI4FoodDB stored as CSV files in the corresponding directory. 

- Every table contains an **`id` column indicating the anonymized participant ID with the form `A4F_XXXXX`**.
- Missing values are represented as either **"NA" or an empty string ("")**.
- Note that **not all datasets** contain data from every participant.
- **Each dataset includes example data from one participant to illustrate the structure and content**.

## Table of Contents
* [Participant Information](#participant-information)
* [DS1 - Anthropometric Measurements](#ds1---anthropometric-measurements)
* [DS2 - Lifestyle and Health](#ds2---lifestyle-and-health)
* [DS3 - Nutrition](#ds3---nutrition)
* [DS4 - Biomarkers](#ds4---biomarkers)
* [DS5 - Gut Microbiome](#ds5---gut-microbiome)
* [DS6 - Vital Signs](#ds6---vital-signs)
* [DS7 - Physical Activity](#ds7---physical-activity)
* [DS8 - Sleep Activity](#ds8---sleep-activity)
* [DS9 - Emotional State](#ds9---emotional-state)
* [DS10 - Additional Information](#ds10---additional-information)

----------

## Participant Information
File [`participant_information.csv`](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/participant_information.csv) stores the basic information for each participant: 

-   `id`: **Anonymized Participant ID**. Each participant is identified using a unique code in the format `A4F_XXXXX`.
-   `group`: **Intervention Group Assignment**. Participants were divided into two groups:
    -   **Group 1** began with traditional/manual data collection methods and later transitioned to digital methods.
    -   **Group 2** began with digital data collection methods and later transitioned to traditional/manual methods.
-   `sex`: **Sex of the Participant (Female or Male)**.    
-   `usual_weight_kg`: **Usual Weight**. Self-reported or previously recorded weight of the participant, measured in kilograms (kg).    
-   `weight_5years_kg`: **Weight Five Years Ago**. Self-reported weight of the participant five years prior to the intervention, measured in kilograms (kg).    
-   `height_cm`: **Height**. Height of the participant, measured in centimeters (cm).    
-   `intervention_diet_kcal`: **Prescribed Caloric Intake**. Daily recommended energy intake for the participant during the intervention, measured in kilocalories (kcal).    
-   `finished_intervention`: **Intervention Completion Status**. A value of `1` indicates that the participant completed the full intervention, while `0` indicates non-completion.

----------

## [DS1 - Anthropometric Measurements](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS1_AnthropometricMeasurements)

### Health Professional Data

This dataset contains anthropometric data collected by healthcare professionals during three intervention timepoints: baseline (V0), mid-intervention (V2), and end of intervention (V3). Measurements include body weight and height, from which BMI is calculated, as well as waist and hip circumference. Additionally, body composition metrics such as fat and muscle mass percentages and visceral fat levels were obtained using bioelectrical impedance analysis (BIA).

----------

## [DS2 - Lifestyle and Health](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS2_LifestyleHealth)

Includes information on participants' lifestyle habits (e.g., smoking, alcohol intake, medication use) and general health status, including disease history.

### Manual Data

#### Lifestyle

This dataset includes responses to a lifestyle questionnaire completed by participants at the baseline visit. It covers topics such as appetite, meal patterns, alcohol and tobacco use, physical activity, sleep habits, and various psychological indicators. 

#### Health

Medical history data were collected at baseline, including regular medication intake, existing health conditions, and family medical history. The original questionnaire contained both structured and open-ended fields. . The dataset also includes information on menopause status where applicable.

----------

## [DS3 - Nutrition](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS3_Nutrition)

### Digital Data

This dataset contains food and drink images collected during a ~14-day digital intervention, where participants documented their dietary intake by uploading pictures via a dedicated web platform.  Each image is accompanied by a timestamp and its corresponding labels. Further details about the labeling schema and methodology, as well as the database itself, can be found in the [associated research article](https://arxiv.org/abs/2504.06925) and [GitHub repository](https://github.com/AI4Food/FoodNExtDB).

#### Timestamps

A separate CSV file is provided for each participant, recording the timestamp corresponding to each image. These files enable temporal analysis of dietary patterns throughout the intervention.

#### Labels

Food images have been manually annotated with semantic labels to identify food types, ingredients, and preparation methods. These labels are provided in individual CSV files per participant. 

----------

## [DS4 - Biomarkers](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS4_Biomarkers)

Encompasses clinical and biochemical data obtained from blood and urine samples, such as glucose, cholesterol levels, and inflammatory markers. Also, blood glucose levels were tracked over 14 days using a glucose device.

### Health Professional Data

This dataset includes biological markers derived from blood, urine, and saliva samples collected at two timepoints: **V1 (start)** and **V3 (end)** of the intervention. These measurements capture a broad range of immune, biochemical, and genetic indicators relevant to nutrition, metabolism, and general health.


### Digital Data

#### Blood Glucose Levels

Participants wore a Continuous Glucose Monitoring (CGM) device during the digital phase of the study, enabling high-resolution tracking of blood glucose fluctuations over ~14 days. The data, collected at 15-minute intervals, are categorized into standard glycemic ranges and include computed indicators such as glucose variability and the Glucose Management Indicator (GMI).

## [DS5 - Gut Microbiome](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS5_GutMicrobiome)

Stool samples were also collected at V1 and V3  to characterize the gut microbiome composition and functionality via shotgun metagenomics and untargeted metabolomics. Whole-genome shotgun sequencing data are available at the European Nucleotide Archive with accession code [PRJEB87701](https://www.ebi.ac.uk/ena/browser/view/PRJEB87701).

## [DS6 - Vital Signs](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS6_VitalSigns)

Includes measurements of physiological signals such as blood pressure, heart rate, respiratory rate, and body temperature. Electrocardiograms and continuous heart rate data were collected using the smartwatch.

### Health Professional Data

This dataset includes clinical measurements of **heart rate (HR)**, **systolic blood pressure**, and **diastolic blood pressure** taken during study visits **V0**, **V2**, and **V3**. These values were manually recorded by healthcare professionals. 


### Digital Data

#### Heart Rate

Participants wore a smartwatch equipped with photoplethysmography (PPG) sensors to continuously measure HR during the 14-day digital data collection phase. HR data is recorded every 5–10 seconds and includes automatic classification into four activity zones: **below zone 1**, **zone 1**, **zone 2**, and **zone 3**, which reflect increasing levels of physical activity.


#### Electrocardiogram (ECG)

Each participant was asked to perform a **30-second ECG test** once per day, preferably at night. These tests produced waveform data (sampled at 250 Hz), average HR, and a test classification: **normal sinus rhythm**, **atrial fibrillation**, or **inconclusive/unclassifiable**. 

----------

## [DS7 - Physical Activity](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS7_PhysicalActivity)

This dataset contains both manually reported and smartwatch-collected data regarding participants’ physical activity over the course of the study.

### Manual Data

#### International Physical Activity Questionnaire (IPAQ)

Participants completed the **Spanish version of the short IPAQ questionnaire** twice: at the beginning and end of the intervention. This questionnaire evaluates physical activity across **vigorous**, **moderate**, and **walking** categories, reporting both the **frequency (days per week)** and **duration (minutes per day)** of activity. Additionally, the questionnaire captures **sedentary behavior** through daily sitting time.

Each activity is converted into **MET-minutes** (Metabolic Equivalent of Task), and participants are classified into three physical activity categories:

-   **Inactive**: <600 MET-min/week
    
-   **Minimally Active**: ≥600 MET-min/week, meeting minimum thresholds
    
-   **Active**: ≥1500 or ≥3000 MET-min/week, depending on intensity
    

Quantitative (MET-minutes) and qualitative (activity category) variables, along with notes from healthcare professionals, are included.


### Digital Data

Data collected via smartwatch during the 14-day digital phase includes:

-   **Active Minutes**: Records the amount of time participants spent in different levels of physical activity, distinguishing between exercise intensity zones (fat burn, cardio, peak) and general daily activity levels (sedentary to very active).
    
-   **Physical Activity Reports**: Provides summaries of individual physical activity sessions, including metrics like duration, calories burned, distance covered, and heart rate zones. Some activities contain additional data, such as swim strokes and lap times.
    
-   **Estimated VO₂ Max**: Offers estimations of each participant’s maximum oxygen uptake during exercise, including filtered values and associated error margins.
    
-   **Additional Physical Activity Data**: Captures broader daily metrics such as total calories burned, steps taken, altitude, and distance walked, all logged at a high temporal resolution.

----------

## [DS8 - Sleep Activity](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS8_SleepActivity)
The **Sleep Activity** dataset includes both manually collected and digitally recorded data on participants' sleep habits and activity


### Manual Data
The **Oviedo Sleep Questionnaire (OSQ)** was used for manual assessment of sleep habits at the beginning and end of the intervention. This questionnaire assesses sleep satisfaction, insomnia symptoms, hypersomnia, and the use of sleep aids, with data stored in both numeric and text formats. The manual data provides context for understanding the digital sleep data and serves as a baseline for evaluating changes in sleep patterns over time.


### Digital Data
Digital data was captured continuously via smartwatch devices, which monitored various sleep-related parameters throughout the intervention. The smartwatch recorded data such as heart rate, respiratory rate, oxygen saturation, and skin temperature, as well as detailed sleep stage information and sleep quality assessments.
The digital data is organized into several main directories, each corresponding to different aspects of sleep activity. These directories contain time-series data that was recorded continuously throughout the intervention.

-   **Additional Sleep Data**: This directory contains detailed reports on sleep timing, including the duration of different sleep stages (deep, light, and REM sleep) for each participant. The data provides insights into the overall sleep patterns and stages for each night.
    
-   **Heart Rate Variability**: This directory holds data on the variations in heart rate during sleep, which provides insights into the autonomic nervous system activity. It includes measurements of heart rate variability (HRV) over the course of each night, helping to assess the impact of sleep on heart rate dynamics.
    
-   **Oxygen Saturation**: This directory contains measurements of blood oxygen saturation levels during sleep. The data helps monitor participants' respiratory function while sleeping, including any potential hypoxemia episodes.
    
-   **Respiratory Rate**: This directory includes data on the average number of breaths per minute during each participant's sleep. The data is broken down by different sleep stages and provides information about breathing patterns throughout the night.
    
-   **Skin Temperature**: This directory contains data on wrist temperature, recorded every minute throughout the day and night. It includes both overall temperature trends and specific features related to temperature fluctuations during sleep.
    
-   **Sleep Quality**: This directory contains data related to overall sleep quality, including scores for duration, revitalization, and composition of sleep. It also tracks additional parameters like resting heart rate during sleep and restlessness, which can indicate disruptions in sleep patterns.

----------

## [DS9 - Emotional State](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS9_EmotionalState)

The **Emotional State** dataset includes both manual and digital measurements of participants' emotional wellbeing throughout the study.


### Manual Data
Manual data was collected using the **DASS-21** (Depression, Anxiety, and Stress Scale), a validated self-report questionnaire completed by participants twice during the study. This questionnaire assesses the participants' levels of depression, anxiety, and stress over the past week through three subscales, each containing seven items. The **DASS-21** is the primary source of manual emotional state data. It contains self-reported information on depression, anxiety, and stress, with scores calculated for each subscale based on the participant's responses. This data is stored in a CSV file that includes the scores for each scale.

### Digital Data

Digital data was collected via FitBit devices, which continuously measured physiological indicators of stress and emotional state during the intervention. The devices tracked various stress-related metrics, including heart rate, electrodermal activity (EDA), and overall stress management based on lifestyle factors such as sleep and physical activity. The digital data collected through FitBit devices provides insights into the participants' emotional state based on physiological measurements, such as heart rate and skin conductance levels. The data is organized into two main components:

-   **EDA Sessions**: This directory contains data on the participants' electrodermal activity (EDA) sessions, which are used to measure skin conductance levels (SCL). The data is stored in CSV files and includes information about the SCL levels recorded during each session, providing insights into the body's response to stress.
    
-   **Stress Score**: This directory includes the daily stress management scores derived from 10 factors related to sleep, heart rate, and physical activity. The final score, ranging from 1 to 100, indicates the level of stress management. Higher scores reflect better stress management, with fewer physical signs of stress.

----------

## [DS10 - Additional Information](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets/DS10_AdditionalInformation)

### Manual Data
The **Additional Information** dataset contains supplementary data on various aspects related to cognitive function, COVID-19 symptoms, and system usability. We provide the **System Usability Scale (SUS)**, where participants completed the System Usability Scale (SUS) to evaluate their experience with the digital tools used during the study. The survey consisted of 10 items, and responses from 96 participants are stored in the dataset. The data is stored in a CSV file that includes participant responses to the 10 items of the SUS survey, assessing the usability and user satisfaction with the digital tools used during the intervention.

