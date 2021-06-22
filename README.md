# Project 2 - Ames Housing Data and Kaggle Challenge

## Contents:
- [Background Summary](#Background-Summary)
- [Problem Statement](#Problem-Statement)
- [Data Dictionary](#Data-Dictionary)
- [Conclusions](#Conclusions)
- [Recommendations](#Recommendations)

## Background Summary

Provided with Ames housing data, there many contributing features that could possibly be of great impact or less in influencing housing prices. With this insight, house buyers could look into the more prominent and proper type of feature to make a judgement to assist propery companies to make a better rated pricing for houses. With this awareness of selectivity in the contributing predictive features, a proposed model will be constructed to allow an economical or a competitive pricing to be improved for potential house buyers and sellers.  

Kaggle Challenge Site: https://www.kaggle.com/c/dsi-us-11-project-2-regression-challenge/data

## Problem Statement

There are many feature predictors based on which may potentially greatly affect the sales price of houses in Ames. The focus for this project is to streamline it down from all the feature predictors to the top 5 features that may greatly be of a potential impact to the sales price of housing in Ames.

## Data Dictionary

| No | Features/ ID        | Type        | Description                                                                                    |
|----|---------------------|-------------|-----------------------------------------------------------------------------------------------|
| 0  |   id                | int         | ID number                                                                                      |
| 1  |   pid               | int         |  Parcel identification number  - can be used with city web site for parcel review.             |
| 2  |   ms_subclass       | int         | Identifies the type of dwelling involved in the sale.                                        |
| 3  |   ms_zoning         | categorical | Identifies the general zoning classification of the sale.                                    |
| 4  |   lot_frontage      | float       | Linear feet of street connected to property                                                    |
| 5  |   lot_area          | int         | Lot size in square feet                                                                        |
| 6  |   street            | categorical | Type of road access to property                                                                |
| 7  |   lot_shape         | categorical | General shape of property                                                                      |
| 8  |   land_contour      | categorical | Flatness of the property                                                                      |
| 9  |   utilities         | categorical | Type of utilities available                                                                    |
| 10 |   lot_config        | categorical | Lot configuration                                                                              |
| 11 |   land_slope        | categorical | Slope of property                                                                              |
| 12 |   neighborhood      | categorical | Physical locations within Ames city limits (map available)                                   |
| 13 |   condition_1       | categorical | Proximity to various conditions                                                                |
| 14 |   condition_2       | categorical | Proximity to various conditions (if more than one is present)                                  |         
| 15 |   bldg_type         | categorical | Type of dwelling                                                                              |
| 16 |   house_style       | categorical | Style of dwelling                                                                              |
| 17 |   overall_qual      | int         | Rates the overall material and finish of the house                                        |
| 18 |   overall_cond      | int         | Rates the overall condition of the house                                                      |
| 19 |   year_built        | int         | Original construction date                                                                    |
| 20 |   year_remod/add    | int         | Remodel date (same as construction date if no remodeling or additions)                     |
| 21 |   roof_style        | categorical | Type of roof                                                                                  |
| 23 |   exterior_1st      | categorical | Exterior covering on house                                                                    |
| 24 |   exterior_2nd      | categorical | Exterior covering on house (if more than one material)                                    |
| 25 |   mas_vnr_type      | categorical | Masonry veneer type                                                                            |
| 26 |   mas_vnr_area      | float       | Masonry veneer area in square feet                                                            |
| 27 |   exter_qual        | categorical | Evaluates the quality of the material on the exterior                                     |
| 28 |   exter_cond        | categorical | Evaluates the present condition of the material on the exterior                              |
| 29 |   foundation        | categorical | Type of foundation                                                                            |
| 30 |   bsmt_qual         | categorical | Evaluates the height of the basement                                                          |
| 31 |   bsmt_cond         | categorical | Evaluates the general condition of the basement                                                |
| 32 |   bsmt_exposure     | categorical | Refers to walkout or garden level walls                                                        |
| 33 |   bsmtfin_type_1    | categorical | Rating of basement finished area                                                              |
| 34 |   bsmtfin_sf_1      | int         | Type 1 finished square feet                                                                    |
| 35 |   bsmtfin_type_2    | categorical | Rating of basement finished area (if multiple types)                                       |
| 36 |   bsmtfin_sf_2      | int         | Type 2 finished square feet                                                                    |
| 37 |   bsmt_unf_sf       | int         | Unfinished square feet of basement area                                                        |
| 38 |   total_bsmt_sf     | int         | Total square feet of basement area                                                            |
| 39 |   heating           | categorical | Type of heating                                                                                |
| 40 |   heating_qc        | categorical | Heating quality and condition                                                                  |
| 41 |   central_air       | categorical | Central air conditioning                                                                      |
| 42 |   electrical        | categorical | Electrical system                                                                              |
| 43 |   1st_flr_sf        | int         | First Floor square feet                                                                        |
| 44 |   2nd_flr_sf        | int         | Second floor square feet                                                                      |
| 45 |   low_qual_fin_sf   | int         | Low quality finished square feet (all floors)                                                  |
| 46 |   gr_liv_area       | int         | Above grade (ground) living area square feet                                                  |
| 47 |   bsmt_full_bath    | int         | Basement full bathrooms                                                                        |
| 48 |   bsmt_half_bath    | int         | Basement half bathrooms                                                                        |
| 49 |   full_bath         | int         | Full bathrooms above grade                                                                    |
| 50 |   half_bath         | int         | Half baths above grade                                                                        |
| 51 |   bedroom_abvgr     | int         | Bedrooms above grade (does NOT include basement bedrooms)                                    |
| 52 |   kitchen_abvgr     | int         | Kitchens above grade                                                                          |
| 53 |   kitchen_qual      | categorical | Kitchen quality                                                                                |
| 54 |   totrms_abvgrd     | int         | Total rooms above grade (does not include bathrooms)                                   |
| 55 |   functional        | categorical | Home functionality (Assume typical unless deductions are warranted)                    |
| 56 |   fireplaces        | int         | Number of fireplaces                                                                          |
| 57 |   fireplace_qu      | categorical | Fireplace quality                                                                              |
| 58 |   garage_type       | categorical | Garage location                                                                                |
| 59 |   garage_yr_blt     | float       | Year garage was built                                                                          |
| 60 |   garage_finish     | categorical | Interior finish of the garage                                                                  |
| 61 |   garage_cars       | int         | Size of garage in car capacity                                                                |
| 62 |   garage_area       | int         | Size of garage in square feet                                                                  |
| 63 |   garage_qual       | categorical | Garage quality                                                                                |
| 64 |   garage_cond       | categorical | Garage condition                                                                              |
| 65 |   paved_drive       | categorical | Paved driveway                                                                                |
| 66 |   wood_deck_sf      | int         | Wood deck area in square feet                                                                  |
| 67 |   open_porch_sf     | int         | Open porch area in square feet                                                                |
| 68 |   enclosed_porch    | int         | Enclosed porch area in square feet                                                            |
| 69 |   3ssn_porch        | int         | Three season porch area in square feet                                                        |
| 70 |   screen_porch      | int         | Screen porch area in square feet                                                              |
| 71 |   pool_area         | int         | Pool area in square feet                                                                      |
| 72 |   pool_qc           | categorical | Pool quality                                                                                  |
| 73 |   fence             | categorical | Fence quality                                                                                  |
| 74 |   misc_feature      | categorical | Miscellaneous feature not covered in other categories                                   |
| 75 |   misc_val          | int         | Value of miscellaneous feature                                                                |
| 76 |   mo_sold           | int         | Month Sold (MM)                                                                                |
| 77 |   yr_sold           | int         | Year Sold (YYYY)                                                                              |
| 78 |   sale_type         | categorical | Type of sale                                                                                  |
| 79 |   saleprice         | int         | Condition of sale                                                                              |
| 80 |   alley             | categorical | Type of alley access to property                                                              |
| 81 |   prop_age          | int         | Age of Property in years                                                                      |
| 81 |   remod_age         | int         | Age of remodel/add in years                                                                    |

### Data Description

train.csv -- this data contains all of the training data for your model.
The target variable (SalePrice) is removed from the test set!

test.csv -- this data contains the test data for your model. You will feed this data into your regression model to make predictions.

sample_sub_reg.csv -- An example of a correctly formatted submission for this challenge (with a random number provided as predictions for SalePrice. Please ensure that your submission to Kaggle matches this format.

train_clean -- cleaned training data

train_clean_enc -- cleaned and encoded training

test_clean -- cleaned test data

test_clean_enc -- cleaned and encoded test data 

merged_clean -- cleaned training and test data merged

merged_clean_enc -- cleaned and encoded training and test data merged


## Conclusions

## Model comparison

Ridge regression has the better R2 test score yet at 88.88% with RMSE at 27003.54 although it is not too far of from Lasso regression which has a R2 test score of 88.87% with RMSE at 27033.17 which shows that both regression models are applicable in this context to achieve results. With 33 features now, it is now more ideal and easy to explain to relevant stakeholders.  

Ridge Regression model also does not look to be overfitted as they perform better on the test score. 

### Top 5 features from Ridge Regression model 

The top feature that highly influences the price at a coefficient of 48643.08 is a property located at Stone Brooks neighbourhood. It is no wonder the best predictor as this neighbourhood is very convenient and is the closest to Iowa State University, the largest university in Iowa state. [[1]](https://en.wikipedia.org/wiki/Iowa_State_University) It is also very close to downtown and is just about a 10 minute drive away. The other two neighbourhoods, Northridge Heights and Northridge are situated close together and is slightly further away to then University but is equidistant to downtown as compared to Stone Brook neighbourhood. 
Moreover all three neighbourhoods are very close to elementary, middle and high schools and have amenities really close by. [[2]](https://www.google.com/maps/dir/304+Main+Street,+Ames,+IA/Northridge+Lane,+Ames,+IA/@42.0286767,-93.6589652,14.28z/data=!4m14!4m13!1m5!1m1!1s0x87ee7079a7344bb5:0xda5a2e61aea06f0d!2m2!1d-93.614092!2d42.024838!1m5!1m1!1s0x87ee70c37ac346ef:0x5c6a8eb7cb2ce524!2m2!1d-93.6467454!2d42.0478309!3e0?hl=en-US)

However, it is interesting to note that the land contour that is hilly is valued more than the other land contour features. It is perhaps has a good privacy rating among home dwellers in Ames. 

At top five, Overall Quality of the property takes the spot and is no suprise that it is one of the top predictors in property prices, though the coefficient is much lower than being in the top three neighbourhoods. 


| Feature              | Coefficient | Model |
|----------------------|-------------|-------|
| neighborhood_StoneBr | 48643.08    | Ridge |
| neighborhood_NridgHt | 35089.63    | Ridge |
| neighborhood_NoRidge | 34101.80    | Ridge |
| land_contour_HLS     | 15144.81    | Ridge |
| overall_qual         | 11663.70    | Ridge |

Therefore, it can be concluded that having a property in those top three neighbourhoods is way more important in highly influencing property prices than Overall Quality. 

### Recommendations

It is important to note that the above conclusions are only based on the Ames housing dataset. More detailed analysis is not possible as the data provided are actual sale prices of houses. In order to complement the above findings, more detailed data such as buyer data and coordinates of home sales would be beneficial to deep dive into analysis such as buyer behaviour or neighbourhood studies. This could enable home owners or property developers to better target buyers, or to even educate buyers on the kind of houses they should look out for. 

With the right data, it can potentially be an exciting area to look into. 