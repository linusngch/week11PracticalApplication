# week11PracticalApplication

Link to notebook: https://github.com/linusngch/week11PracticalApplication/blob/main/whatDrivesACarsPrice.ipynb

This project utilizes data from a kaggle set regarding features of cars and the price of its value. The provided 
dataset contains information on 426K cars to ensure speed of processing. The goal is to understand what factors 
make a car more or less expensive and to provide clear recommendations to aclient -- a used car dealership -- \
as to what consumers value in a used car.

Upon viewing the data, there seemed to be a lot of null values and information that was not necessary to the influence
of a car's price. The ID, VIM and size columns were dropped and categorical columns were turned into numerical. The price
column, the target, was spliced to remove any outliers (high variability). Additionally, it was log() ot better fit the data
because its original format was skewed. 

After the cleanup and scaling, the best model used on this dataset was a Ridge() model with alpha = 10000 and polynomial feature
of 3. This model yielded a test and trianing MSE of 0.13 and showed that the 3 most influential features that influence the price 
of a car were year, title_status, and manufacturer. These values had a positive correlation whereas all other features had 
negative values. Baseed on these findings, it is recommended that the car dealership should look out for cars which have been 
recently made or of an extremely older model. Newer models have more features and have more up to date features which would drive 
their prices up. Older models are no longer manufactured which makes its price go up since people might want to collect them. 
Because these features have a higher impact on the price of the vehicle, car dealers should revise their purchasing/selling
business plan to revolve around these feature for better profits.


