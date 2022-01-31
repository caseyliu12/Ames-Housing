# Project 2: Ames Housing Project

## Problem statement

I have datasets of Ames housing. My goal is to use the datasets to predict the price of houses at sale and identify the important factors that have impact on to the value of houses. The Ames Housing Dataset is an exceptionally detailed and robust dataset with over 70 columns of different features relating to houses. I am going to process the data and create a regression model based on the Ames Housing Dataset.


## Data Dictionary

 - Order (Discrete): Observation number
 - PID (Nominal): Parcel identification number - can be used with city web site for parcel review.
 - MS SubClass (Nominal): Identifies the type of dwelling involved in the sale.
 - MS Zoning (Nominal): Identifies the general zoning classification of the sale.
 - Lot Frontage (Continuous): Linear feet of street connected to property
 - Lot Area (Continuous): Lot size in square feet
 - Street (Nominal): Type of road access to property
 - Alley (Nominal): Type of alley access to property
 - Lot Shape (Ordinal): General shape of property
 - Land Contour (Nominal): Flatness of the property
 - Utilities (Ordinal): Type of utilities available
 - Lot Config (Nominal): Lot configuration
 - Land Slope (Ordinal): Slope of property
 - Neighborhood (Nominal): Physical locations within Ames city limits (map available)
 - Condition 1 (Nominal): Proximity to various conditions
 - Condition 2 (Nominal): Proximity to various conditions (if more than one is present)
 - Bldg Type (Nominal): Type of dwelling
 - House Style (Nominal): Style of dwelling
 - Overall Qual (Ordinal): Rates the overall material and finish of the house
 - Overall Cond (Ordinal): Rates the overall condition of the house.
 - Year Built (Discrete): Original construction date
 - Year Remod/Add (Discrete): Remodel date (same as construction date if no remodeling or additions)
 - Roof Style (Nominal): Type of roof
 - Roof Matl (Nominal): Roof material
 - Exterior 1 (Nominal): Exterior covering on house
 - Exterior 2 (Nominal): Exterior covering on house (if more than one material)
 - Mas Vnr Type (Nominal): Masonry veneer type
 - Mas Vnr Area (Continuous): Masonry veneer area in square feet
 - Exter Qual (Ordinal): Evaluates the quality of the material on the exterior
 - Exter Cond (Ordinal): Evaluates the present condition of the material on the exterior
 - Foundation (Nominal): Type of foundation
 - Bsmt Qual (Ordinal): Evaluates the height of the basement
 - Bsmt Cond (Ordinal): Evaluates the general condition of the basement
 - Bsmt Exposure (Ordinal): Refers to walkout or garden level walls
 - BsmtFin Type 1 (Ordinal): Rating of basement finished area
 - BsmtFin SF 1 (Continuous): Type 1 finished square feet
 - BsmtFinType 2 (Ordinal): Rating of basement finished area (if multiple types)
 - BsmtFin SF 2 (Continuous): Type 2 finished square feet
 - Bsmt Unf SF (Continuous): Unfinished square feet of basement area
 - Total Bsmt SF (Continuous): Total square feet of basement area
 - Heating (Nominal): Type of heating
 - HeatingQC (Ordinal): Heating quality and condition
 - Central Air (Nominal): Central air conditioning
 - Electrical (Ordinal): Electrical system
 - 1st Flr SF (Continuous): First Floor square feet
 - 2nd Flr SF (Continuous) : Second floor square feet
 - Low Qual Fin SF (Continuous): Low quality finished square feet (all floors)
 - Gr Liv Area (Continuous): Above grade (ground) living area square feet
 - Bsmt Full Bath (Discrete): Basement full bathrooms
 - Bsmt Half Bath (Discrete): Basement half bathrooms
 - Full Bath (Discrete): Full bathrooms above grade
 - Half Bath (Discrete): Half baths above grade
 - Bedroom (Discrete): Bedrooms above grade (does NOT include basement bedrooms)
 - Kitchen (Discrete): Kitchens above grade
 - KitchenQual (Ordinal): Kitchen quality
 - TotRmsAbvGrd (Discrete): Total rooms above grade (does not include bathrooms)
 - Functional (Ordinal): Home functionality (Assume typical unless deductions are warranted)
 - Fireplaces (Discrete): Number of fireplaces
 - FireplaceQu (Ordinal): Fireplace quality
 - Garage Type (Nominal): Garage location
 - Garage Yr Blt (Discrete): Year garage was built
 - Garage Finish (Ordinal) : Interior finish of the garage
 - Garage Cars (Discrete): Size of garage in car capacity
 - Garage Area (Continuous): Size of garage in square feet
 - Garage Qual (Ordinal): Garage quality
 - Garage Cond (Ordinal): Garage condition
 - Paved Drive (Ordinal): Paved driveway
 - Wood Deck SF (Continuous): Wood deck area in square feet
 - Open Porch SF (Continuous): Open porch area in square feet
 - Enclosed Porch (Continuous): Enclosed porch area in square feet
 - 3-Ssn Porch (Continuous): Three season porch area in square feet
 - Screen Porch (Continuous): Screen porch area in square feet
 - Pool Area (Continuous): Pool area in square feet
 - Pool QC (Ordinal): Pool quality
 - Fence (Ordinal): Fence quality
 - Misc Feature (Nominal): Miscellaneous feature not covered in other categories
 - Misc Val (Continuous): $Value of miscellaneous feature
 - Mo Sold (Discrete): Month Sold (MM)
 - Yr Sold (Discrete): Year Sold (YYYY)
 - Sale Type (Nominal): Type of sale
 - Sale Condition (Nominal): Condition of sale
 - SalePrice (Continuous): Sale price $$# Ames-Housing-Dataset
 
 Source: http://jse.amstat.org/v19n3/decock/DataDocumentation.txt
 
 
## Data Analysis Summary
 
I take the following steps to make data processing and predictions:

- Data Cleaning (fill and replace the empty data)
- Create dummy variables and some new variables which are transform from original variables, identify if a house have the feature
- Exploratory Data Analysis. Create plots to understand the relationship between certain variables and the target sale value.
- Select variables for modeling, scale the data and fit the model. I fit Linear Regression, LassoCV, and RidgeCV models to the training and testing sets and select one of the models.
- Predict the sale price based on the model I select and get the top factors.


## Conclusions and Recommendations
 
From the analysis we provided above, we can see that the following factors have the greatest impact on the sale price of a home:

- Overall quality
- First floor in square feet
- Exterior quality
- Pool area in square feet
- Basement quality
- Kitchen quality
- Masonry veneer area in square feet
- Garage quality
- Screen porch area
- Size of garage in car capacity

In conclusion, the quality of overall, exterior, basement, kitchen and garage is very important on a house value. The area size of first floor, pool, masonry veneer, screen porch and garage (in car capacity) would also impact the sale price. The real estate developers should pay attention on these factors to get higher house value.
