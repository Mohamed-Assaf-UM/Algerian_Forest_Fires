# Algerian Forest Fires 
This project focuses on analyzing and classifying forest fire occurrences in two regions of Algeria: Bejaia and Sidi Bel-Abbes. The dataset, which consists of 244 instances, includes various meteorological and fire weather index components collected from June to September 2012. The data is divided into two classes: fire and not fire. The goal is to clean, preprocess, and analyze the data before applying a classification model to predict the occurrence of fires.

### Dataset Description
The dataset includes 11 input features and 1 output feature:
- **Date**: Represented by day, month, and year (2012).
- **Temperature**: Maximum temperature at noon, ranging from 22°C to 42°C.
- **RH**: Relative Humidity, ranging from 21% to 90%.
- **Ws**: Wind speed in km/h, ranging from 6 to 29 km/h.
- **Rain**: Total daily precipitation, ranging from 0 to 16.8 mm.
- **Fire Weather Index (FWI) Components**:
  - **FFMC**: Fine Fuel Moisture Code (28.6 to 92.5).
  - **DMC**: Duff Moisture Code (1.1 to 65.9).
  - **DC**: Drought Code (7 to 220.4).
  - **ISI**: Initial Spread Index (0 to 18.5).
  - **BUI**: Buildup Index (1.1 to 68).
  - **FWI**: Fire Weather Index (0 to 31.1).
- **Class**: Binary classification into two categories — fire or not fire.

### Data Preprocessing
The dataset was preprocessed to handle missing values and correct inconsistent data entries:
- Rows with null values were identified and removed.
- A new column was added to distinguish between the two regions, with Bejaia labeled as `0` and Sidi Bel-Abbes as `1`.
- Spaces in column names were stripped to ensure clean data representation.
- Data types of key columns, such as day, month, year, temperature, and humidity, were converted from string to integer for more accurate analysis and modeling.

### Feature Transformation and Cleaning
- The dataset contained some rows with inconsistencies, such as placeholder text in numerical fields. These were carefully handled and cleaned.
- An additional region column was added to split the dataset based on location.
- Rows with null or irrelevant values were dropped, resulting in 243 clean instances.
  
### Exploratory Data Analysis
Several analyses were performed to understand the relationships between different meteorological parameters and the occurrence of forest fires:
- Visualization tools like Seaborn and Matplotlib were used to explore the distributions and correlations within the dataset.
- Histograms, scatter plots, and box plots were employed to identify trends and patterns that contribute to fire occurrences.

### Modeling
The cleaned data can be further used for classification tasks using various machine learning algorithms. The objective is to predict fire occurrences based on meteorological conditions and fire weather index components.

This project provides a solid foundation for implementing predictive models and gaining insights into how different environmental factors contribute to forest fire risks in Algeria.
