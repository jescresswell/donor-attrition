# donor-attrition
Predicting which donors will continue or cease to donate to Toronto charity.

This work was done for the Data For Good Datathon on May 4, 2019, hosted at CapCo in Toronto, in support of the charity Youth Without Shelter, and in collaboration with Ashwin Jha, Don Nguyen, Reena Shaw, Habib Jaffer, and Will Edwards.

Donor attrition is a major problem for charities, and correcting it can lead to much greater overall fundraising performance. We were asked to find patterns in the charity's donation data to predict which donors may be at risk of lapsing (ceasing to donate). We cleaned and prepared their data to feed into various machine learning models. 

The target variable was whether or not a donor had lapsed, defined as not donating since Jan 01, 2017. 

A major part of the work was converting the limited data that was available into usable formats for our models. The data contains information on individual donations, each associated to a unique donor id. Examples of features in the data include donation amount, date, and donor postal code. We needed to convert these features for individual donations into aggregaate features for the donors themselves. For example, postal codes were converted into a distance from the charity headquarters. 

After feature engineering, we used decision trees with hyperparameter optimization to predict lapse. We found the most significant features in the model to be total number of donations, total donation amount, and distance from charity. The results and recommendations were presented to employees of Youth Without shelter.

Due to privacy issues, the data has not been included in this repo.
