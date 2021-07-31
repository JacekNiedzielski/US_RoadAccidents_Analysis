# Analysis of the USA Road Accidents
### Descriptive and Inferential Statistics Conducted on the Kaggle's US Road Accidents Data Set.
***Project includes the following files:***  
***- US_RoadAccidents.ipynb -> jupyter notebook file containing whole analysis***  
***- US_Accidents_Dec20.csv -> csv file with records as of Decemeber 2020***

#### The motivation of the project is two-branch. In the first part I try to answer questions posed with regard to USA accidents' hot spots. The objective is to try to figure it out, what kind of characteristics define an accident hot spot and which roads among all routes in USA seem to be most dangerous. In the second part I deal with supervised learning model, were I try to predict the severity of an accident (in terms of traffic obstructions)

***This project serves in the first line the fulfillment of the exercise requirements of the first part of the Udacity's "Data Scientist" Nanodegree. Nevertheless, the data set used for this exercise contains actuall records and can be used to drag insights leading to real applications. 
The data set can be retrived from the following link (acutal version) https://www.kaggle.com/sobhanmoosavi/us-accidents  
Version used for my analysis has been attached in form of csv file to this repository  <br/><br/><br/><br/>
Acknowledgements:  <br/><br/>
"Moosavi, Sobhan, Mohammad Hossein Samavatian, Srinivasan Parthasarathy, and Rajiv Ramnath. “A Countrywide Traffic Accident Dataset.”, 2019.  
"Moosavi, Sobhan, Mohammad Hossein Samavatian, Srinivasan Parthasarathy, Radu Teodorescu, and Rajiv Ramnath. "Accident Risk Prediction based on Heterogeneous Sparse Data: New Dataset and Insights." In proceedings of the 27th ACM SIGSPATIAL International Conference on Advances in Geographic Information Systems, ACM", 2019.***  <br/><br/><br/><br/>

### The code is written in Python 3.7.3. Required libraries to run the project:

Python basic libraries:
- math
- random  <br/><br/>

Python data science libraries:
- pandas
- numpy

Python visualistion libraries:
- matplotlib
- seaborn <br/><br/>

Python machine learning libraries:
- sklearn <br/><br/>

Python geospatial data science libraries:
- geopandas
- geoplot (Python 3.6+ only!) <br/><br/>  

Possible installation is via Anaconda Prompt. For all libraries the command `conda install "library_name"` will work. The geoplot has to be installed over the Forge Channel:  `conda install geoplot -c conda-forge` <br/><br/><br/>

## Insights Summary: </br></br>
### Accidents' Hot Spots
- I was able to distinguish three roads with accident pile ups. Of course these are not the only ones, however they seem to be outstanding from the others.
Please refer to the following picutres:  


</br>
- Amenities and environmental conditions connected to the accidents' frequency:

### Application of Neural Network for predicting the Severity of an Accident
- Producing the algorithm to predicit the accidents' severity is hampered due to strongly unbalanced number of different labels in the data set. Since the mode (severity class 2) makes around 70% percent of all records, an accuracy level of around 75% (obtained by model fitted onto original data) does not bring much. One could get nearly the same just by picking up the mode. Less represented classes could not be predicted properly. Therefore, the data set has been balanced so all of the classes contained the same number of records. Such an approach enhenced the models capability to predict among less numerous classes, however got worse while predicting class 2 beeing now underrepresented. Please compare the results below:
![percentage_of_missed_values_balanced](https://user-images.githubusercontent.com/64994740/127740815-3fad01c8-1220-470a-8c73-07c5f1342698.png)

