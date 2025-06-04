# DS4 - Biomarkers

### Health Professional Data

#### Biomarkers

The file [`biomarkers.csv`](https://github.com/AI4Food/AI4FoodDB/blob/master/datasets/DS4_Biomarkers/biomarkers.csv) contains a wide range of biochemical parameters measured from biological samples collected during study visits:

-   `id`: **Anonymized Participant ID**, formatted as `A4F_XXXXX`.
    
-   `visit`: **Visit code** indicating when the measurements were taken:
    
    -   `0`: Baseline (V0)
        
    -   `2`: Mid-intervention (V2)
        
    -   `3`: End of intervention (V3)
        

#### Hematological Parameters:

-   `leukocytes_10e3_ul`, `plats_10e3_ul`, `lympho_10e3_ul`, `mono_10e3_ul`, `seg_10e3_ul`, `eos_10e3_ul`, `baso_10e3_ul`: Counts of leukocytes, platelets, lymphocytes, monocytes, segmented neutrophils, eosinophils, and basophils, expressed as $10^3/\mu{L}$.
    
-   `erythrocytes_10e6_ul`: Erythrocyte count, measured as $10^6/\mu{L}$.
    
-   `hgb_g_dl`: Hemoglobin concentration (g/dL).
    
-   `hematocrit_perc`: Hematocrit percentage.
    
-   `mcv_fl`, `mpv_fl`: Mean corpuscular volume (MCV) and mean platelet volume (MPV), in femtoliters (fL).
    
-   `mch_pg`, `mchc_g_dl`: Mean corpuscular hemoglobin (MCH) in picograms (pg), and mean corpuscular hemoglobin concentration (MCHC) in g/dL.
    
-   `rdw_perc`: Red cell distribution width (%).
    
-   `lympho_perc`, `mono_perc`, `seg_perc`, `eos_perc`, `baso_perc`: Percentages of lymphocytes, monocytes, segmented neutrophils, eosinophils, and basophils.
    

#### Metabolic and Inflammatory Markers:

-   `hba1c_perc`, `hba1ifcc_mmol_mol`: Glycated hemoglobin as % and in IFCC units (mmol/mol).
    
-   `insulin_uui_ml`: Insulin concentration ($\mu{UI}/mL$).
    
-   `homa`: Homeostatic Model Assessment for Insulin Resistance (HOMA-IR).
    
-   `glu_mg_dl`: Blood glucose (mg/dL).
    
-   `chol_mg_dl`, `tri_mg_dl`, `hdl_mg_dl`, `ldl_mg_dl`: Total cholesterol, triglycerides, HDL, and LDL cholesterol (mg/dL).
    
-   `homocysteine_umol_l`: Homocysteine concentration ($\mu{mol}/L$).
    
-   `alb_g_dl`, `prealbumin_mg_dl`: Albumin (g/dL) and prealbumin (mg/dL).
    
-   `crp_mg_dl`: C-reactive protein (mg/dL).
    

#### Immune and Hormonal Markers:

-   `igg_mg_dl`, `iga_mg_dl`, `igm_mg_dl`, `ige_ui_ml`: Immunoglobulin G, A, and M (mg/dL); IgE (UI/mL).
    
-   `tnf_a_ui_ml`: Tumor Necrosis Factor-α (TNF-α) concentration (UI/mL).
    
-   `adiponectin_ug_ml`: Adiponectin concentration ($\mu{g}/mL$).
    

----------
### Digital Data

#### Blood Glucose Levels

The directory [`glucose_levels`](https://github.com/AI4Food/AI4FoodDB/blob/master/datasets/DS4_Biomarkers/glucose_levels) contains continuous glucose monitoring (CGM) data from each participant. Files are named `A4F_XXXXX_glucose_levels.csv` and record glucose values collected approximately every 15 minutes over the 14-day digital data collection period.

Due to occasional device desynchronization, some values may be missing.

Each file contains:

-   `timestamp`: **Timestamp of the glucose reading**, in the format `YYYY-MM-DD HH:MM:SS+Z`.
    
-   `glucose_value_in_mg_dl`: **Glucose level** at that timestamp, measured in mg/dL.
