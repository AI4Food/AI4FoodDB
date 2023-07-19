
# AI4FoodDB: A Database for Personalized e-Health Nutrition and Lifestyle through Wearable Devices and Artificial Intelligence

The increasing prevalence of diet-related diseases calls for an improvement in nutritional advice. Personalized nutrition aims to solve this problem by adapting dietary and lifestyle guidelines to the unique circumstances of each individual. With the latest advances in technology and data science, researchers can now automatically collect and analyze large amounts of data from a variety of sources, including wearable and smart devices. In this repository, we present the **AI4Food database (AI4FoodDB)**, which gathers data from a nutritional weight loss intervention monitoring 100 overweight and obese participants during one month. Data acquisition involved **manual traditional approaches, novel digital methods, and the collection of biological samples**. 

Moreover, the collected information will yield valuable insights into the relationships between different variables and health outcomes, allowing researchers to generate and test new hypotheses, identify novel biomarkers and digital endpoints, and explore how different lifestyle, biological, and digital factors impact health. 

## Table of Contents
* [Database Description](#database-description)
* [Datasets](#datasets)
* [Citation](#citation)
* [Contact](#contact)

## Database Description
The AI4Food database (AI4FoodDB) gathers data from a nutritional intervention with 100 overweight and obese participants. Data acquisition involved manual traditional approaches, novel digital methods, and the collection of biological samples. An overview of AI4FoodDB is shown below.

![Overview of the AI4FoodDB](https://user-images.githubusercontent.com/129155966/228174005-b2bddfcc-fd07-403b-a83b-8bc304e3b63f.svg)

***Overview of the AI4FoodDB.*** _The database comprises 10 datasets representing different types of data acquired during the nutritional intervention: Anthropometric Measurements (DS1), Lifestyle and Health (DS2), Nutrition (DS3), Biomarkers (DS4), Gut Microbiome (DS5), Vital Signs (DS6), Physical Activity (DS7), Sleep Activity (DS8), Emotional State (DS9), and Additional Information (DS10). Datasets are colored according to the data acquisition method: manual (in orange), clinical (in purple), or digital (in yellow)._

## [Datasets](datasets)
### Available Datasets
The currently available datasets are:
- [**DS1: Anthropometric Measurements.**](datasets/DS1_AnthropometricMeasurements) Manually-collected data available at [`datasets/anthropometric_measurements.csv`](datasets/DS1_AnthropometricMeasurements/anthropometric_measurements.csv).
- [**DS2: Lifestyle and Health.**](datasets/DS2_LifestyleHealth) Manually-collected data available at [`datasets/lifestyle.csv`](datasets/DS2_LifestyleHealth/lifestyle.csv) and [`datasets/health.csv`](datasets/DS2_LifestyleHealth/health.csv).
- [**DS3: Nutrition**](datasets/DS3_Nutrition) Digital-collected data available.
- [**DS4: Biomarkers.**](datasets/DS4_Biomarkers) Clinical data available at [`datasets/biomarkers.csv`](datasets/DS4_Biomarkers/biomarkers.csv). 
- [**DS6: Vital Signs.**](datasets/DS6_VitalSigns) Clinical data available at [`datasets/vitalsigns.csv`](datasets/DS6_VitalSigns/vitalsigns.csv). 

For a more detailed description of each dataset, please access the [`datasets`](datasets) directory.

### Ongoing Datasets
- **DS5: Gut Microbiome.**
- **DS7: Physical Activity**
- **DS8: Sleep Activity**
- **DS9: Emotional**
- **DS10. Additional Information.**

***NOTE: We plan to update the repository frequently, making the remaining files available as soon as possible.***

## Citation
If you use data from this project, please cite the following publication:

```
@article{ai4fooddb2023,
  title={AI4FoodDB: A Database for Personalized e-Health Nutrition and Lifestyle through Wearable Devices and Artificial Intelligence},
  author={Romero-Tapiador, Sergio and Lacruz-Pleguezuelos, Blanca and Tolosana, Ruben and Freixer, Gala and Daza, Roberto and Fernández-Díaz, Cristina M and Aguilar-Aguilar, Elena and Fernández-Cabezas, Jorge and Cruz-Gil, Silvia and Molina, Susana and Crespo, Maria Carmen and Laguna, Teresa and Marcos-Zambrano, Laura Judith and Vera-Rodriguez, Ruben and Fierrez, Julian and Ramírez de Molina, Ana and Ortega-Garcia, Javier and Espinosa-Salinas, Isabel and Morales, Aythami and Carrillo de Santa Pau, Enrique},
  journal={Database: The Journal of Biological Databases and Curation},
  year={2023}
}
```


## Contact
If you have any questions, please contact us at ruben.tolosana@uam.es or enrique.carrillo@imdea.org
