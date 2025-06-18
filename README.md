 # AI4FoodDB: A Database for Personalized e-Health Nutrition and Lifestyle through Wearable Devices and Artificial Intelligence 

### Article 📄: [AI4FoodDB: A Database for Personalized e-Health Nutrition and Lifestyle through Wearable Devices and Artificial Intelligence (10.1093/database/baad049)](https://academic.oup.com/database/article/doi/10.1093/database/baad049/7226275)
## Download AI4FoodDB 🗂️

📌 **The AI4FoodDB dataset can be accessed at the following link:**  
[https://bidalab.eps.uam.es/static/AI4FoodDB/AI4FoodDB.zip](https://bidalab.eps.uam.es/static/AI4FoodDB/AI4FoodDB.zip)

**This .zip file includes all datasets except Dataset 3 (DS3) – Nutrition, and Dataset 5 (DS5) – Gut Microbiome.**

- **Dataset 3 (DS3) - Nutrition** can be accesed at the following link: [https://bidalab.eps.uam.es/static/AI4FoodDB/FoodNExtDB.zip](https://bidalab.eps.uam.es/static/AI4FoodDB/FoodNExtDB.zip)
- **Dataset 5 (DS5) - Gut Microbiome** can be accesed at the following link: [https://www.ebi.ac.uk/ena/browser/view/PRJEB87701](https://www.ebi.ac.uk/ena/browser/view/PRJEB87701)

**The AI4FoodDB database will only be used for research purposes and will not be used nor included in commercial applications in any form (e.g., original files, encrypted files, files containing extracted features, etc).**

## Table of Contents
* [Database Description](#database-description)
* [Datasets](#datasets)
* [Citation](#citation)
* [Contact](#contact)

## Database Description
The increasing prevalence of diet-related diseases calls for an improvement in nutritional advice. Personalized nutrition aims to solve this problem by adapting dietary and lifestyle guidelines to the unique circumstances of each individual. With the latest advances in technology and data science, researchers can now automatically collect and analyze large amounts of data from a variety of sources, including wearable and smart devices. In this repository, we present the **AI4Food database (AI4FoodDB)**, which gathers data from a nutritional weight loss intervention monitoring 100 overweight and obese participants during one month. Data acquisition involved **manual traditional approaches, novel digital methods, and the collection of biological samples**. For more information about the project and the nutritional intervention, refer to our [article](https://academic.oup.com/database/article/doi/10.1093/database/baad049/7226275) published in *Database: The Journal of Biological Databases and Curation*.

Moreover, the collected information will yield valuable insights into the relationships between different variables and health outcomes, allowing researchers to generate and test new hypotheses, identify novel biomarkers and digital endpoints, and explore how different lifestyle, biological, and digital factors impact health. 

The AI4Food database (AI4FoodDB) gathers data from a nutritional intervention with 100 overweight and obese participants. Data acquisition involved manual traditional approaches, novel digital methods, and the collection of biological samples. An overview of AI4FoodDB is shown below.

![Overview of the AI4FoodDB](https://user-images.githubusercontent.com/129155966/228174005-b2bddfcc-fd07-403b-a83b-8bc304e3b63f.svg)

***Overview of the AI4FoodDB.*** _The database comprises 10 datasets representing different types of data acquired during the nutritional intervention: Anthropometric Measurements (DS1), Lifestyle and Health (DS2), Nutrition (DS3), Biomarkers (DS4), Gut Microbiome (DS5), Vital Signs (DS6), Physical Activity (DS7), Sleep Activity (DS8), Emotional State (DS9), and Additional Information (DS10). Datasets are colored according to the data acquisition method: manual (in orange), clinical (in purple), or digital (in yellow)._

## [Datasets](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets)
### For a more detailed description of each dataset, please access the [`datasets`](https://github.com/AI4Food/AI4FoodDB/tree/master/datasets) directory.
The currently available datasets are:
- **DS1 - Anthropometric Measurements:** Contains basic body measurements such as weight, height, BMI, waist circumference, and other anthropometric indicators that reflect body composition and size.
- **DS2 - Lifestyle and Health:** Includes information on participants' lifestyle habits (e.g., smoking, alcohol intake, medication use) and general health status, including disease history.
- **DS3 - Nutrition:** Contains all food images captured by participants during the ~14-day digital intervention, representing the meals they consumed. Each image is accompanied by a timestamp and its corresponding labels.
- **DS4 - Biomarkers:** Encompasses clinical and biochemical data obtained from blood and urine samples, such as glucose, cholesterol levels, and inflammatory markers. Also, blood glucose levels were tracked over 14 days using a glucose device.
- **DS5 - Gut Microbiome:** Stool samples were also collected to characterize the gut microbiome composition and functionality via shotgun metagenomics and untargeted metabolomics. 
- **DS6 - Vital Signs:** Includes measurements of physiological signals such as blood pressure, heart rate, respiratory rate, and body temperature. Electrocardiograms and continuous heart rate data were collected using the smartwatch.
- **DS7 - Physical Activity:** Contains data on participants' physical activity levels (e.g., steps, intensity, duration). Information was gathered using self-reported questionnaires (International Physical Activity Questionnaire -IPAQ) as well as smartwatches.
- **DS8 - Sleep Activity:** Sleep habits were manually assessed using the Oviedo Sleep Questionnaire (OSQ), while the smartwatch recorded various sleep-related parameters.
- **DS9 - Emotional State:** Includes self-reported and sensor-based assessments of mood and emotional well-being collected via questionnaires (Depression, Anxiety and Stress Scale, DASS-21) and smartwatches.
- **DS10 - Additional Information:** Includes responses to the System Usability Scale (SUS), a 10-item questionnaire completed by 96 participants at the end of the intervention to assess adherence to digital data collection devices.



***IMPORTANT NOTE: We plan to update the repository frequently, making the remaining files available as soon as possible.***

## Citation

**Any work made public, whatever the form, based directly or indirectly on any part of the AI4FoodDB database will include the following references:**

**The following publications:**

- S. Romero-Tapiador, B. Lacruz-Pleguezuelos, R. Tolosana, G. Freixer, R. Daza, C. M. Fernández-Díaz, E. Aguilar-Aguilar, J. Fernández-Cabezas, S. Cruz Gil, S. Molina-Arranz, M. C. Crespo, L. J. Marcos-Zambrano, R. Vera-Rodriguez, J. Fierrez, A. Ramirez de Molina, J. Ortega-Garcia, I. Espinosa-Salinas, A. Morales and E. Carrillo de Santa Pau., “AI4FoodDB: a database for personalized e-Health nutrition and lifestyle through wearable devices and artificial intelligence”, Database: The Journal of Biological Databases and Curation, vol baad049, doi: [10.1093/database/baad049](https://academic.oup.com/database/article/doi/10.1093/database/baad049/7226275), 2023.
 
```
@article{ai4fooddb2023,
  title={AI4FoodDB: A Database for Personalized e-Health Nutrition and Lifestyle through Wearable Devices and Artificial Intelligence},
  author={Romero-Tapiador, Sergio and Lacruz-Pleguezuelos, Blanca and Tolosana, Ruben and Freixer, Gala and Daza, Roberto and Fernández-Díaz, Cristina M and Aguilar-Aguilar, Elena and Fernández-Cabezas, Jorge and Cruz Gil, Silvia and Molina-Arranz, Susana and Crespo, Maria Carmen and Laguna-Lobo, Teresa and Marcos-Zambrano, Laura Judith and Vera-Rodriguez, Ruben and Fierrez, Julian and Ramírez de Molina, Ana and Ortega-Garcia, Javier and Espinosa-Salinas, Isabel and Morales, Aythami and Carrillo de Santa Pau, Enrique},
  journal={Database: The Journal of Biological Databases and Curation},
  volume={2023},
  pages={baad049},
  year={2023}
}
```

   - B. Lacruz-Pleguezuelos, Guadalupe X. Bazán, S. Romero-Tapiador, G. Freixer, R. Tolosana, R. Daza, C. M. Fernández-Díaz, S. Molina, M. C. Crespo, T. Laguna, L. J. Marcos-Zambrano, E. Aguilar-Aguilar, J. Fernández-Cabezas, S. Cruz Gil, L. P. Fernández, R. Vera-Rodriguez, J. Fierrez, A. Ramirez de Molina, J. Ortega-Garcia, A. Morales, E. Carrillo de Santa Pau, and I. Espinosa-Salinas, “AI4Food, a feasibility study for the implementation of automated devices in the nutritional advice and follow up within a weight loss intervention”, Clinical Nutrition, 48:80-89, doi: [10.1016/j.clnu.2025.03.003](https://www.sciencedirect.com/science/article/pii/S0261561425000718), 2025. 

```
@article{lacruz2025ai4food,
  title={AI4Food, a feasibility study for the implementation of automated devices in the nutritional advice and follow up within a weight loss intervention},
  author={Lacruz-Pleguezuelos, Blanca and Baz{\'a}n, Guadalupe X and Romero-Tapiador, Sergio and Freixer, Gala and Tolosana, Ruben and Daza, Roberto and Fern{\'a}ndez-D{\'\i}az, Cristina M and Molina, Susana and Crespo, Mar{\'\i}a Carmen and Laguna, Teresa and others},
  journal={Clinical Nutrition},
  volume={48},
  pages={80--89},
  year={2025}
}
```


## Contact
If you have any questions, please contact us at ruben.tolosana@uam.es or enrique.carrillo@imdea.org.
