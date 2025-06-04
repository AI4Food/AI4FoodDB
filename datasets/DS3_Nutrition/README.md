
# DS3 - Nutrition

### Digital Data

### FoodNExTDB - Food Images

Food images for each participant are stored in their respective folders. Each image is named using the format A4F_XXXXX_YYYY.jpg, where A4F_XXXXX corresponds to the Anonymized Participant ID, and YYYY indicates the image number. Each participant also has an associated CSV file named A4F_XXXXX_timestamps.csv, which contains a timestamp column indicating when each photo was taken, and another CSV file named A4F_XXXXX_labeled_data.csv, which includes the corresponding labels.

#### Timestamps

For each participant, a CSV file named `A4F_XXXXX_timestamps.csv` provides detailed information about when each food image was captured. This file contains three variables:

-   `id`: **Image ID** in the format `A4F_XXXXX_YYYY.jpg`, where `A4F_XXXXX` corresponds to the **Anonymized Participant ID**, and `YYYY` is the **image number**.
    
-   `timestamp`: **Timestamp of the photo**, in the format `YYYY-MM-DD HH:MM:SS+Z`.
    
-   `original_timestamp_validity`: A boolean indicating whether the timestamp reflects the **actual time the photo was taken** (`True`) or the **time it was uploaded to the platform** (`False`).
    

The `timestamp` value is considered reliable only if `original_timestamp_validity` is set to `True`. Otherwise, it may not correspond to the real moment of food consumption, as it reflects the upload time instead.

#### Labels

Labels for each image are stored in a separate file named `A4F_XXXXX_labeled_data.csv`, detailing the semantic annotation of food items. For details about the labeling process—including definitions of categories, subcategories, and cooking styles—please refer to [our article](https://arxiv.org/abs/2504.06925) and [GitHub repository](https://github.com/AI4Food/FoodNExtDB). The labeling file includes the following variables:


-   `id`: **Image ID** in the format `A4F_XXXXX_YYYY.jpg`, where `A4F_XXXXX` corresponds to the **Anonymized Participant ID**, and `YYYY` is the **image number**.
    
-   `id_labeler`: **Labeler ID** who annotated the image.
    
-   `category`: **Main food category** assigned to the item (e.g., vegetables and fruits, protein source, fast food).
    
-   `subcategory`: **Specific food subcategory** (e.g., fruits, poultry, pizza).
    
-   `cooking_style`: **Preparation or cooking method** used (e.g., grilled, raw, boiled).
