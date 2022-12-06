# DMDD-16149-Loan_Enquiry_DB
*This repository contains all the files related to DMDD Assignments and project by team TheBI_Trio .*

**Title : Loan Enquiry System**

**Team Members :**

               Juilee Patil             | patil.ju@northeastern.edu
               Dhriti Sunil Kanchan     | kanchan.dh@northeastern.edu
               Jayesh Tak               | tak.j@northeastern.edu


**Project Description :**

Loan enquiry system aspires to simplify, make transparent and make personal finance decisions conveniently. It will compare rate of interest of financial institutes and help customers who are seeking to choose lowest EMI on loans and looking to avail the best offeres in the market.


**The loan database will consists of various parameters which are related to :** 

* Banks details
* Loan types offered with their corresponding rate of interest .
* Customer details .
* Schemes and policies by government .
* Feedback and reviews on service offered by the bank.


**Blueprint :**




<img width="503" alt="image" src="https://user-images.githubusercontent.com/112820037/191874143-befc5fae-ff5f-4fac-8bab-a4d1b59764a6.png">


**End Product :**

Loan Enquiry System would provide users with immediate, personalized rate quotes on loans. Users can search, compare current rates, and select the best option for themselves.


**Project Steps :**

1.Environment preparation : Import libraries 
2.Finding the right key to scrap the data & Extracting the right information : Extract data from the 
web
3. Data wrangling & Creating DataFrame : Transforming the data according to requirements
4.Creating a tidy python notebook as a report : Cleaning Code
5.Implement it on matplotlib : To display analysis and relation of data


<img width="584" alt="image" src="https://user-images.githubusercontent.com/112820037/205819905-16975f4c-9c20-4518-b2c4-5798a740d59d.png">


**Data Gathering :**

Files: 1. Html_webscrapping 2. DB_file
API : Snscrape
URL’s:
Data Source : URL’s BeautifulSoup
Data Munging
DataFrames
Storing & Saving in 
DB
url_homeLoan = 'https://www.forbes.com/advisor/in/home-loan/current-rates/'
url = 'https://www.bankbazaar.com/personal-loan-interest-rate.html'
url_eduLoan = 'https://www.forbes.com/advisor/in/education-loan/education-loan-interest-rate/'
url_carLoan = 'https://www.creditmantri.com/car-loan-interest-rates/'


**Dependencies :**
The library and modules for this project are:
Requests
Beautiful Soup
Pandas
The request and beautiful soup are used to do the web scrapping of the sites. While Pandas are used 
for the managing the dataframe of the stored data and also stored the data in the csv format. And the 
last sub and decimal are used to transform the data into the desired output.


**CODE :**

After we get the targeted path, we can put it in the code. The code will be:
page= requests.get(url)
table = soup.find('table',class_='hungry-table table-bordered')
div_HL = soup_HL.find_all('div',id='footable_parent_55679')
df = pd.DataFrame(name of your tupple, columns = (name of the columns))
After the various Loan related attributes will be extracted. The data will be stored in the dataframe.
Tables Populated:
1.Dim_Guarantor
2.Dim_Lending_Rates
3.Dim_Loan_Type
4.Fact_Applicant
5.Fact_Bank
6.Fact_Customer_Loan_Details
7.Fact_Loan
8.Fact_Universities
9.Loan Interest

** Test and Results :**


Converting and mapping data from one raw format into another. The purpose of this is to prepare 
the data in a way that makes it accessible for effective use further down the line. Not all data is 
created equal, organized and transformed data in a way that can be easily accessed by others.
1. Interest range converted to Max and Min rates.
2. Purged textual data from numerical field
3. Removed NAN & unwanted data

<img width="589" alt="image" src="https://user-images.githubusercontent.com/112820037/205820357-1d2ddc2d-43ca-4bdd-b88f-cdc1b662c1c4.png">
