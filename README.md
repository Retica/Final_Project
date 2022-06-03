# Michigan State University Data Analytics Final Project

## Topic Selection
For this project, the topic the team selected was one that is current and affects us all. The housing market is one that all team members are interested in, and the status of the market affects the economic state of the country and therefore, every aspect of people's lives. The cost of houses, mortgage rates, household income and debt, and foreclosure rates are some of the factors to be considered. 
<br>
Additionally, the housing market crash of 2008 is an event that no one wants repeated. With inflation and rising gas prices, considering the 2008 crash is vital to this analysis. Researching the cause of the 2008 crash led the team to an article called <a href= "https://www.uwp.edu/learn/departments/economics/upload/gwartney-summary-of-financial-crisis.pdf" target= "_blank"> "The Crash of 2008: Causes and Lessons to be Learned"</a>. Reading through this confirmed the factors the team was looking at are the correct ones. 

### Presentation 
You may view the team's presentation <a href="https://docs.google.com/presentation/d/1AfdtdySqur9ehjTxvcnTzLTNBDWX6JnLH4DBKe0W3bI/edit#slide=id.g96c5e74a8e_0_1339" target= "_blank">here</a>.
## Questions to Consider and Data Sources
The main question is whether or not the housing market has the potential to crash again. As well as the following questions:

- What trends lead to the 2008 crash? 
- What was done to prevent another crash? 
- What current trends are repeating? 
- How do they line up with 2008 trends? 
- What new trends are prominent?
      
 Questions will be answered using data sourced from: 
 
 - https://www.fhfa.gov/DataTools/Downloads/Pages/House-Price-Index-Datasets.aspx

 - https://catalog.data.gov/dataset?q=fhfa

 - https://www.federalreserve.gov/releases/z1/dataviz/household_debt/state/map/#year:2020
 
 - https://www.fincen.gov/fincen-mortgage-fraud-sar-database

 - Federal Reserve Economic Data (FRED) fred.stlouisfed.org

## Technology Used for Analysis
The team used Visual Studio Code and Jupyter Notebook to clean the data sources, with the Pandas Library to clean datasets, remove missing rows, and extract the files. The data was then imported into PgAdmin using SQL, and joined using SQL. The data was split into years to view the Housing Price Index (HPI) and household debt. Multiple libraries were used to conduct the Machine Learning portion of the analysis. 

Below are images of data using SQL and a sample code from PgAdmin:

<img width="1076" alt="hpi_table" src="https://user-images.githubusercontent.com/65638310/167280128-950385b3-e316-4dc2-be2f-32605b486d4f.png">

<img width="746" alt="sampleofcodeforsql" src="https://user-images.githubusercontent.com/65638310/168510424-f8b87f84-f470-4c1d-b307-a86bfa43aa1f.png">

## Machine Learning
### Data Preprocessing
An initial machine learning model was done prior to preprocessing to see what needed to be cleaned and split. It was then determined that spliting the data into each year from 1991-2022 was needed to see the difference between each year. Following that, the team looked at five specific years out of the thirty year dataset to conduct machine learning on: 1991, 2000, 2008, 2015, and 2022. This was done to see how the predictions from these models line up with the actual data from those years. 
<br>

### Models Used
The results the team is looking for required them to test multiple machine learning models:
- K-Means 
- Principal Component Analysis (PCA)
- Random Forest Classifiers
- Logistic Regression
- Neural Networks

While all these methods were attempted, not all of the models gave them the answers they were looking for. 
<br>

### Analyzing the Data
The HPI dataset was also transformed into the average index from each year and put into a graph:

<img width="746" alt="machinelearning_hpi" src="https://user-images.githubusercontent.com/65638310/170892877-b13b697c-1e19-46c7-91c8-db51be0b45cd.png">

<br>
As well as the foreclosure rates:
<img width="746" alt="machinelearning_foreclosure" src="https://user-images.githubusercontent.com/65638310/170892848-438b0802-2b40-46f3-a5b5-e634a1e5ee61.png">

<br>
We also looked at household debt rates:

<img width="746" alt="machinelearning_debt" src="https://user-images.githubusercontent.com/65638310/170892860-5050e915-6f18-4efa-9e97-83dadefd4ec4.png">

 
<br>


Viewing the averages shows the passage of time and how drastic the changes are in one image. This gave the team the idea to compare them and then generate a model that could predict the next few years. 
<br>

The most successful models were Random Forest Classifiers and PCA. 
HPI and foreclosure


<img width="746" alt="machinelearning_hpi_foreclosure" src="https://user-images.githubusercontent.com/65638310/170892903-153498be-cbc2-45c8-8541-2a4a8d39104f.png">

HPI and Household Income



<img width="746" alt="machinelearning_hpi_and_debt" src="https://user-images.githubusercontent.com/65638310/170892915-751403bb-9620-4404-a2a6-a52596e8db0a.png">


### Limitations 
Neural Networks were not able to give the team what they were looking for. 
<br>
This analysis was done with a handul of datasets. There are many other data sources that could be found, although it would take more time to simply comb through it. 
Data from the HPI dataset was also dropped due to potential overfitting, after running the machine learning models with the data. Although it would be great to see which parts of the United States has differences in prices, mortgages, detb, etc. it was not feasible for the team to complete and get an accurate analysis. 
<br>


## Results

The analysis shows that the market has the potential to crash again in the near future. The HPI is four times what it was in 1991. Currently, 2022 shows that it is in class 2 compared to class 1 the couple of years before and on 2008. The foreclosure rates compared are also in class 2 for 2022 and class 1 in 2008. Once again in 2008 compared to 2022, we are one class difference. The foreclosure rates in 2022 is in class 3 compared to 2008 which is in class 2. 
When looking at the machine learning module for HPI and foreclosure, we can see that the classes are similar in results as HPI and household income. 

## Dashboard

https://public.tableau.com/app/profile/benjamin.j.carter/viz/HousingMarketAnalysis_16538884963830/HousingMarketDataStory?publish=yes

## Final Thoughts 
    
There are other variables that might not have quanitifiable data to analyze, such as the recent (May 2022) issues with Ukraine and Russia. This could affect housing in ways that are yet unknown. After the 2008 crash, laws were passed to ensure that this wouldn't happen again, but how has the effect of those laws changed in the last 15 years? Even with an analysis like this one, the future is still unknown are there are other factors that will affect the results of this dataset that cannot be predicted. 
