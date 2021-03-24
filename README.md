![Zillow Header](https://theme.zdassets.com/theme_assets/512712/5675f10a90572d0f4140b0b39e72e4905bce34ee.jpg)
# Estimating Home Value
## Project Description
### What is Zillow?
> "Zillow is the leading real estate and rental marketplace dedicated to empowering consumers with data, inspiration and knowledge around the place they call home, and connecting them with the best local professionals who can help." [zillow.com](https://www.zillow.com/z/corp/about/)
### Background
Scenario:  Hello, Junior Data Scientist!  Us Senior Data Scientists at Zillow need your help to find the drivers behind tax value for our one unit properties.  Be sure to pull data from our hottest months (May 2017 - August 2018).  We also need tax rate distribution for the counties in your data set.  Thanks so much!
### Goals 
1. Predict the values of single unit properties that the tax district asssess using the property data from those whose last transaction was May-June 2017
2.  Determine distribution of tax rates for each county
  
### Deliverables
1. Presentation
- 3-5 slides
- 5 minute presentation
2. Github repository containing all work
- 1 final jupyter notebook 
- 1 explore notebook
- 1 model notebook
3. README.md file
### Data Dictonary
| Feature | Description | Data Type |
|-|-|-|
| bathroomcnt | Number of bathrooms in home including fractional bathrooms | int |
| bedroomcnt | Number of bedrooms in home | int |
| buildingqualitytypeid | Overall assessment of condition of the building from best (lowest) to worst (highest) | int |
| calculatedfinishedsquarefeet | Calculated total finished living area of the home | float  |
| fips | Federal Information Processing Standard code | object |
| parcelid | Unique identifier for parcels (lots) | float |
| regionidneighborhood | Neighborhood in which the property is located | int |
| unitcnt | Number of units the structure is built into (i.e. 2 = duplex, 3 = triplex, etc...) | float |
| yearbuilt | The Year the principal residence was built | int |
| taxvaluedollarcnt | The total tax assessed value of the parcel | float |
| taxamount | The total property tax assessed for that assessment year | float |
## Hypotheses
### Initial Hypotheses (Prepare Phase)
1. Is there a linear correlation between square footage and tax value?
2. Is there a linear correlation between number of bathrooms and tax value?
3. Is there a linear correlation between number of bedrooms and tax value?

## Project Planning
### [Zillow Project Plan Board](https://trello.com/invite/b/NIMAxzMz/ebdd6a8c55a5008aa5d5d9a90efe8aa0/zillow-project-workflow)
### Aquire
* Gather data from Codeup database using SQL 
* Create function with python that gathers data from SQL and reads it into a dataframe
* Create acquire.py file with function to acquire data
### Prepare
* Clean up:  missing values, data integrity issues, data types, invalid data
* Scale: numeric data (if necessary)
* Plot: individual distributions of individual variables
* Split:  split dataset into train, validate, and test
* Create prepare.py file that contains all functions used to prepare data
### Explore
* Perform at least 1 t-test and 1 correlation test 
* Visualize all combinations of variables
* Determine variables that are correlated with each other
* Summarize takeaways and conclusions
### Model
* Establish and evaluate baseline model
* Use various algorithms to develop model that beats baseline
* Create a model.py file that includes functions to fit, predict, and evaluate final model on the test data set
## How to Reproduce
1. Clone or fork this repository
2. Download the following files into the directory you wish to work in: aquire.py, prepare.py, explore.py, and zillow_regression.ipynb
3. Run the zillow_regression jupyter notebook in its entirety
4. Modify features/models/etc how you see fit
