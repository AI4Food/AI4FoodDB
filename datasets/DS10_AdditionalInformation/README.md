# DS10 - Additional Information

### Manual Data

#### System Usability Scale (SUS)

Participants completed the System Usability Scale (SUS), a 10-item questionnaire designed to evaluate the usability of the digital tools provided during the intervention. The SUS was administered at the end of the intervention to assess adherence and user satisfaction, with responses from 96 participants. The data is stored in the `SUS.csv` file and includes the following variables:

-   `id`: **Anonymized Participant ID**, formatted as `A4F_XXXXX`.
    
-   `visit`: **Visit code**, indicating the timepoint of data collection:
    
    -   `0`: Baseline (V0)
        
    -   `2`: Mid-intervention (V2)
        
    -   `3`: End of intervention (V3)
        
-   `1_like_to_use`
    
-   `2_complex`
    
-   `3_easy_to_use`
    
-   `4_technical_support`
    
-   `5_well_integrated`
    
-   `6_inconsistency`
    
-   `7_quick_to_learn`
    
-   `8_cumbersome`
    
-   `9_confident`
    
-   `10_need_to_learn`
    
-   `positive_score`: Subscore based on positively phrased items.
    
-   `negative_score`: Subscore based on negatively phrased items.
    
-   `sum`: Raw sum of all responses.
    
-   `total_score`: Final SUS score normalized to a 0–100 scale.