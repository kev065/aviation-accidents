# Aviation Accidents Analysis
!["Image of plane with the text the future of travel"](images/plane-the-future-of-travel.jpg)

View an interactive dashboard for this project [here](https://public.tableau.com/app/profile/kelvin.murithi/viz/Aviation_Expansion_Dashboard_17178564462710/AverageInjuriesByMake) and presentation slides [here](https://www.canva.com/design/DAGHfLmoKU0/6oduvEozUpzvoglQvJ7GXA/view?utm_content=DAGHfLmoKU0&utm_campaign=designshare&utm_medium=link&utm_source=editor)

## **Business Understanding**
### **Background**
As part of our strategic initiative to diversify our company's portfolio, we are venturing into the aviation industry. This expansion involves purchasing and operating airplanes for both commercial and private enterprises. Given the high stakes associated with aviation, understanding the potential risks and ensuring the highest standards of safety is paramount for the success and sustainability of this new business endeavor.

### **Objective**
My primary objective is to identify the aircraft models that present the lowest risk in terms of safety and operational reliability. This involves a comprehensive analysis of historical aviation accident data to evaluate the safety performance of various aircraft manufacturers and models. The goal is to provide actionable insights that will guide the decision-making process for the acquisition of aircraft, ensuring that we select models with proven safety records.

## **Data Understanding**
To achieve this objective, I have utilized the National Transportation Safety Board (NTSB) [dataset](https://www.kaggle.com/datasets/khsamaha/aviation-accident-database-synopses), which includes detailed information on civil aviation accidents from 1962 to 2023. The analysis focuses on key metrics such as fatality rates, injury rates, and the number of uninjured passengers and crew in accidents. These metrics are crucial for assessing the overall safety performance of different aircraft models.

The decision on which aircraft to purchase will be based on the following criteria derived from our analysis:
1. **Uninjured Rate** - The proportion of passengers and crew who remain uninjured in the event of an accident.
2. **Fatality Rate** - The number of fatalities per accident involving the aircraft.
3. **Variety and Availability** - The range of models available from the manufacturer and their suitability for our intended operations i.e. commercial and private travel.

## **Data Cleaning Process**

Ensuring the quality and consistency of our data is paramount. I undertook the following data cleaning steps to prepare the dataset for analysis:

1. **Checking for Duplicates**: My first step was to check for duplicate values in the dataset. Ensuring the uniqueness of our records is crucial to avoid skewed results. This check however found that the dataset does not contain any duplicate entries.

2. **Cleaning Column Names**: To make the dataset easier to work with, I standardized our column names. I replaced dots with underscores and capitalized the first letter of each word. This makes the column names more readable and easier to work with in our code.

3. **Cleaning 'Model' Column Values**: To ensure consistency, I've converted all values in this column to strings. Additionally, I replaced spaces with hyphens to avoid any potential issues with spaces in our data.

## **Data Reduction**
In our analysis of aviation accidents, I aim to focus on the most relevant data to enable making of informed recommendations. As such, I have decided to perform data reduction by dropping certain columns from this dataset. This step will simplify our data and make it easier to handle, without losing the information that is crucial to our analysis.

The columns I dropped are:

1. **Latitude**: While geographical data could be interesting in some analyses, our focus does not require the specific latitude of accidents.
2. **Longitude**: Similar to Latitude, Longitude is not necessary for the current analysis.
3. **Schedule**: The schedule of the flight does not contribute significantly to the analysis of injury rates and safety features.
4. **Air_Carrier**: This analysis is focused on aircraft manufacturers rather than air carriers.
5. **Aircraft_Category**: We are looking at specific aircraft models in our analysis, making the broader category less relevant.
6. **Far_Description**: This column contains regulatory info that is not directly related to our analysis.

By reducing our data in this way, I can focus more closely on the factors that are most relevant to this project. This will help draw more accurate conclusions and help me make meaningful recommendations to present to the new aviation honcho.
