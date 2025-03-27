# Laptop_Pricing_Analysis
Labs using mock laptop data to perform data analysis using Python. Jupyter Notebooks are part of IBM's "Data Analysis with Python" course.

----------------------------------------------------------------------------------------------------------------------------------------------------
## Overview - Laptop Pricing Data Set
The following is an overview of the provided data set used for the labs:

### Parameters
The parameters used in the dataset are:

#### Manufacturer
The company that manufactured the laptop

#### Category
The category to which the laptop belongs: This parameter is mapped to numerical values in the following way:

|  Category    |  Assigned Value  |
|--------------|------------------|
|  Gaming	     |  1               |
|  Netbook     |  2               |
|  Notebook	   |  3               |
|  Ultrabook   |  4               |
|  Workstation |  5               |

#### GPU
The manufacturer of the GPU. This parameter is mapped to numerical values in the following way:

|  GPU         |  Assigned Value  |
|--------------|------------------|
|  AMD	       |  1               |
|  Intel       |  2               |
|  NVidia	     |  3               |

#### OS
The operating system type (Windows or Linux): This parameter is mapped to numerical values in the following way:

|  OS          |  Assigned Value  |
|--------------|------------------|
|  Windows	   |  1               |
|  Linux       |  2               |

#### CPU_core
The type of processor used in the laptop: This parameter is mapped to numerical values in the following way:

|  CPU_core          |  Assigned Value  |
|--------------------|------------------|
|  Intel Pentium i3	 |  3               |
|  Intel Pentium i5  |  5               |
|  Intel Pentium i7	 |  7               |

#### Screen_Size_cm
The size of the laptop screen is recorded in cm.

#### CPU_frequency
The frequency at which the CPU operates, in GHz.

#### RAM_GB
The size of the RAM of the system in GB.

#### Storage_GB_SSD
The size of the SSD storage in GB is installed in the laptop.

#### Weight_kg
The weight of the laptop is in kgs.

#### Price
The price of the laptop is in USD.

----------------------------------------------------------------------------------------------------------------------------------------------------
## Notebook 1 - Importing Data Sets

### Key Highlights:

#### Data Handling:
Loaded a dataset containing 238 laptop entries with 12 columns covering manufacturer, specifications, and pricing.

#### Exploratory Data Analysis (EDA): 
Used df.info() to inspect column data types, non-null counts, and memory usage.

#### Identifying Data Issues: 
Detected missing values in Screen_Size_inch and Weight_kg columns.

#### Python & Pandas Techniques:
Imported datasets using pandas.read_csv().
Used df.info() for dataset structure analysis.
Recognized numerical (int64, float64) and categorical (object) data types.

This lab serves as a foundation for further data analysis exercises, reinforcing skills in data exploration, cleaning, and preprocessing.

----------------------------------------------------------------------------------------------------------------------------------------------------
## Notebook 2 - Data Wrangling

### Key Skills Covered:
- Handling missing data in different ways
- Correcting incorrect data types
- Standardizing and normalizing dataset attributes
- Visualizing data using binning
- Converting categorical data into numerical indicators

### Setup & Libraries Used:
- pandas (data manipulation)
- numpy (mathematical operations)
- matplotlib (data visualization)
- skillsnetwork (dataset download)

### Key Tasks & Insights:
#### 1. Importing Required Libraries:
- numpy, pandas, and matplotlib are loaded for data processing.

#### 2. Loading the Dataset:
- The dataset is downloaded and loaded into a Pandas DataFrame using pd.read_csv().
- The dataset contains 238 rows and 13 columns, including attributes like Manufacturer, Category, Screen_Size_cm, Weight_kg, and Price.

#### 3. Handling Missing Data:
- Identified missing values in Screen_Size_cm (4 missing values) and Weight_kg (5 missing values).
- Replaced missing Weight_kg values with the mean of the column.

#### 4. Data Type Correction & Standardization:
- Rounded Screen_Size_cm values to two decimal places for consistency.

#### 5. Further Data Processing:
- Future tasks in the lab involve standardizing and normalizing data, visualizing attributes using binning, and converting categorical data into numerical indicators.

----------------------------------------------------------------------------------------------------------------------------------------------------
## Notebook 3 - Exploratory Data Analysis

### Key Skills Covered:

- Visualizing feature patterns

- Running descriptive statistical analysis

- Using groups and pivot tables to analyze categorical variables

- Measuring correlation using Pearson’s method

### Setup & Libraries Used:

pandas, numpy, seaborn, matplotlib, scipy

### Key Tasks & Insights:
#### 1. Visualizing Feature Patterns
Regression Plots for continuous variables (CPU_frequency, Screen_Size_inch, Weight_pounds) vs. Price

##### Findings:

- CPU_frequency has a moderate positive correlation (0.37)

- Screen_Size_inch and Weight_pounds show weak correlations with price

- Box Plots for categorical variables (Category, GPU, OS, CPU_core, RAM_GB, Storage_GB_SSD)

- Differences in median price observed across these categories

#### 2. Descriptive Statistical Analysis
- Summary statistics for numerical and categorical features
- Identified distribution trends and variations in laptop pricing

#### 3. Measuring Correlations
- Used Pearson correlation matrix
- CPU_frequency had the highest positive correlation with price
- Other features had minimal impact

----------------------------------------------------------------------------------------------------------------------------------------------------
## Notebook 4 - Model Development

----------------------------------------------------------------------------------------------------------------------------------------------------
## Notebook 5 - Model Evaluation and Refinement
