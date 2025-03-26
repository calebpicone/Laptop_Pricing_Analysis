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

### Key Highlights

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

### Key Highlights:

#### Handling Missing Data:
Identified missing values in Screen_Size_cm and Weight_kg columns.
Replaced missing Weight_kg values with the column's mean.

#### Data Cleaning & Standardization:
Rounded Screen_Size_cm values to two decimal places.
Converted categorical data into numerical indicator variables.

#### Data Visualization:
Used binning to group numerical data and plotted grouped bar graphs.

#### Libraries Used:
pandas, numpy, matplotlib, and skillsnetwork for dataset retrieval.

----------------------------------------------------------------------------------------------------------------------------------------------------
## Notebook 3 - Exploratory Data Analysis

----------------------------------------------------------------------------------------------------------------------------------------------------
## Notebook 4 - Model Development

----------------------------------------------------------------------------------------------------------------------------------------------------
## Notebook 5 - Model Evaluation and Refinement
