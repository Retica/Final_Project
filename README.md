# Michigan State University Data Analytics Final Project

## Topic Selection
For this project, the topic the team selected was one that is current and affects us all. The housing market is one that all team members are interested in, and the status of the market affects the economic state of the country and therefore, every aspect of people's lives. The cost of houses, mortgage rates, household income and debt, and foreclosure rates are some of the factors to be considered. 
<br>
Additionally, the housing market crash of 2008 is an event that no one wants repeated. With inflation and rising gas prices, considering the 2008 crash is vital to this analysis. Researching the cause of the 2008 crash led the team to an article called <a href= "https://www.uwp.edu/learn/departments/economics/upload/gwartney-summary-of-financial-crisis.pdf" target= "_blank"> "The Crash of 2008: Causes and Lessons to be Learned"</a>. Reading through this confirmed the factors the team was looking at are the correct ones. 

### Presentation 
You may view the team's presentation <a href="https://docs.google.com/presentation/d/1mFdGQxLgh6vyrf8ICaeMgpGHqsTdZ5wPPCPurxvz_3Q/edit?usp=sharing" target= "_blank">here</a>.
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
!!! insert image 
<br>
As well as the foreclosure rates:
!! insert image 
<br>

Viewing the averages shows the passage of time and how drastic the changes are in one image. This gave the team the idea to compare them and then generate a model that could predict the next few years. 
<br>

The most successful models were Random Forest Classifiers and PCA. Logisitic Regression
!!!! insert more here

### Limitations 
Neural Networks were not able to give the team what they were looking for. 
<br>
This analysis was done with a handul of datasets. There are many other data sources that could be found, although it would take more time to simply comb through it. 
Data from the HPI dataset was also dropped due to potential overfitting, after running the machine learning models with the data. Although it would be great to see which parts of the United States has differences in prices, mortgages, detb, etc. it was not feasible for the team to complete and get an accurate analysis. 
<br>

There are other variables that might not have quanitifiable data to analyze, such as the recent (May 2022) issues with Ukraine and Russia. This could affect housing in ways that are yet unknown. After the 2008 crash, laws were passed to ensure that this wouldn't happen again, but how has the effect of those laws changed in the last 15 years? Even with an analysis like this one, the future is still unknown are there are other factors that will affect the results of this dataset that cannot be predicted. 




## Results


### Presentation
    Link to our developing presentation: https://docs.google.com/presentation/d/1mFdGQxLgh6vyrf8ICaeMgpGHqsTdZ5wPPCPurxvz_3Q/edit?usp=sharing
    
