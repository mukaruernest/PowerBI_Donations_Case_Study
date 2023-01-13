# Donations-Case-Study

An Organisation receives donations from Different individuals and companies. The data below is provided to answer the questions that follow. 

Table of Content. 

- [Dataset](https://github.com/mukaruernest/Donations-Case-Study/blob/main/README.md#dataset)
- [Relationships](https://github.com/mukaruernest/Donations-Case-Study/blob/main/README.md#relationships)
- [Questions](https://github.com/mukaruernest/Donations-Case-Study/blob/main/README.md#questions)
- [Solutions](https://github.com/mukaruernest/Donations-Case-Study/blob/main/README.md#solution)
- [Dashboard view](https://github.com/mukaruernest/Donations-Case-Study/blob/main/README.md#dashboard-view)

## Dashboard View

![PowerBI](https://user-images.githubusercontent.com/10958742/124785784-d42c1000-df4f-11eb-947d-caeb8f069b9e.jpg)

[Click to Download pbix file](https://github.com/mukaruernest/Donations-Case-Study/blob/main/IRC%20Donation.pbix?raw=true)

## Dataset
Click the Table Name to view the tables. 

<details>
  <summary>Table Name: Donor</summary>
  
| FirstName | LastName                  | Country        | DonorType   | DonorID |
|-----------|---------------------------|----------------|-------------|---------|
| John      | Smith                     | USA            | Individual  | 1       |
| Jane      | Doe                       | France         | Individual  | 2       |
| Peter     | Parker                    | Germany        | Individual  | 3       |
| Bruce     | Wayne                     | South Africa   | Individual  | 4       |
| Bruce     | Banner                    | Mexico         | Individual  | 5       |
| Tony      | Stark                     | USA            | Individual  | 6       |
| Natasha   | Romanoff                  | Russia         | Individual  | 7       |
| Logan     | Howlett                   | Canada         | Individual  | 8       |
| Diana     | Prince                    | Greece         | Individual  | 9       |
| Guy       | Gardner                   | Brazil         | Individual  | 10      |
| Donald    | Blake                     | Norway         | Individual  | 11      |
| Clark     | Kent                      | United States  | Individual  | 12      |
|           | ABC Corp                  | USA            | Corporation | 13      |
|           | MicroMax                  | France         | Corporation | 14      |
|           | WidgetMakers LLC          | UAE            | Corporation | 15      |
|           | International Business Co | Mexico         | Corporation | 16      |
|           | Fence Foundation          | United States  | Foundation  | 17      |
|           | CA Trust                  | Sweden         | Foundation  | 18      |
|           | Benevolent Society        | United Kingdom | Foundation  | 19      |
|           | Charitable Giving, Inc.   | Saudi Arabia   | Foundation  | 20      |

 </details>

<details>
  <summary>Table Name: Donation</summary>


| DonorName                 | Amount   | GiftDate   | CampaignID | GiftID |
|---------------------------|----------|------------|------------|--------|
| John Smith                | 5.25     | 1/1/2018   | 1          | 100    |
| Jane Doe                  | 175      | 2/2/2018   | 1          | 101    |
| Peter Parker              | 340      | 3/6/2018   | 1          | 102    |
| Bruce Wayne               | 123456   | 4/7/2018   | 2          | 103    |
| Bruce Banner              | 725.15   | 5/9/2018   | 2          | 104    |
| Anthony Stark             | 500000   | 6/10/2018  | 2          | 105    |
| Natasha Romanoff          | 325      | 7/12/2018  | 6          | 106    |
| Logan Howlett             | 15       | 8/13/2018  | 6          | 107    |
| Diana Prince              | 50       | 9/14/2018  | 6          | 108    |
| Guy Gardner               | 0.5      | 10/16/2018 | 1          | 109    |
| Donald R Blake            | 150      | 11/17/2018 | 6          | 110    |
| Clark Kent                | 100      | 12/19/2018 | 6          | 111    |
| ABC Corp                  | 1000     | 1/1/2018   | 4          | 112    |
| MicroMax                  | 5000     | 1/15/2018  | 4          | 113    |
| WidgetMakers LLC          | 50000    | 2/2/2018   | 5          | 114    |
| International Business Co | 100000   | 3/6/2018   | 4          | 115    |
| Fence Foundation          | 500      | 4/7/2018   | 5          | 116    |
| CA Trust                  | 20000    | 5/9/2018   | 4          | 117    |
| Benevolent Society        | 100000   | 6/10/2018  | 5          | 118    |
| Charitable Giving, Inc.   | 500000   | 7/12/2018  | 4          | 119    |
| ABC Corp                  | 1000     | 8/13/2018  | 9          | 120    |
| Anthony Stark             | 1000000  | 9/14/2018  | 8          | 121    |
| Benevolent Society        | 500      | 10/16/2018 | 4          | 122    |
| Bruce Banner              | 1        | 11/17/2018 | 1          | 123    |
| Bruce Wayne               | 5000     | 12/19/2018 | 8          | 124    |
| CA Trust                  | 500      | 1/20/2019  | 7          | 125    |
| Charitable Giving, Inc.   | 7000     | 2/21/2019  | 7          | 126    |
| Clark Kent                | 100      | 3/25/2019  | 1          | 127    |
| Diana Prince              | 50       | 4/26/2019  | 1          | 128    |
| Donald R Blake            | 75       | 5/28/2019  | 1          | 129    |
| Fence Foundation          | 1500     | 6/29/2019  | 8          | 130    |
| Guy Gardner               | 10       | 7/31/2019  | 1          | 131    |
| International Business Co | 75000    | 9/1/2019   | 7          | 132    |
| Jane Doe                  | 800      | 10/3/2019  | 1          | 133    |
| John Smith                | 90       | 11/4/2019  | 1          | 134    |
| Logan Howlett             | 50       | 12/6/2019  | 1          | 135    |
| MicroMax                  | 6500     | 1/7/2020   | 4          | 136    |
| Natasha Romanoff          | 50       | 2/8/2020   | 1          | 137    |
| Peter Parker              | 20       | 3/11/2020  | 1          | 138    |
| WidgetMakers LLC          | 10000    | 4/12/2020  | 8          | 139    |
| WidgetMakers LLC          | 20000    | 5/14/2020  | 3          | 140    |
| Peter Parker              | 50       | 6/15/2020  | 1          | 141    |
| Natasha Romanoff          | 40       | 7/17/2020  | 1          | 142    |
| MicroMax                  | 30000    | 8/18/2020  | 3          | 143    |
| Logan Howlett             | 500      | 9/19/2020  | 7          | 144    |
| John Smith                | 300      | 10/21/2020 | 6          | 145    |
| Jane Doe                  | 40       | 11/22/2020 | 7          | 146    |
| International Business Co | 40000    | 12/24/2020 | 3          | 147    |
| Guy Gardner               | 50       | 11/22/2020 | 7          | 148    |
| Fence Foundation          | 750000   | 10/21/2020 | 3          | 149    |
| Donald R Blake            | 1500     | 9/19/2020  | 3          | 150    |
| Diana Prince              | 300      | 8/18/2020  | 7          | 151    |
| Clark Kent                | 500      | 7/17/2020  | 6          | 152    |
| Charitable Giving, Inc.   | 40000    | 6/15/2020  | 3          | 153    |
| CA Trust                  | 1500000  | 5/14/2020  | 3          | 154    |
| Bruce Wayne               | 10000000 | 4/12/2020  | 3          | 155    |
| Bruce Banner              | 100      | 3/11/2020  | 6          | 156    |
| Benevolent Society        | 500000   | 2/8/2020   | 3          | 157    |
| Anthony Stark             | 10000000 | 1/7/2020   | 3          | 158    |

  </details>
  
  <details>
  <summary>Table Name: Campaign</summary>

| DonorName                 | Amount   | GiftDate   | CampaignID | GiftID |
|---------------------------|----------|------------|------------|--------|
| John Smith                | 5.25     | 1/1/2018   | 1          | 100    |
| Jane Doe                  | 175      | 2/2/2018   | 1          | 101    |
| Peter Parker              | 340      | 3/6/2018   | 1          | 102    |
| Bruce Wayne               | 123456   | 4/7/2018   | 2          | 103    |
| Bruce Banner              | 725.15   | 5/9/2018   | 2          | 104    |
| Anthony Stark             | 500000   | 6/10/2018  | 2          | 105    |
| Natasha Romanoff          | 325      | 7/12/2018  | 6          | 106    |
| Logan Howlett             | 15       | 8/13/2018  | 6          | 107    |
| Diana Prince              | 50       | 9/14/2018  | 6          | 108    |
| Guy Gardner               | 0.5      | 10/16/2018 | 1          | 109    |
| Donald R Blake            | 150      | 11/17/2018 | 6          | 110    |
| Clark Kent                | 100      | 12/19/2018 | 6          | 111    |
| ABC Corp                  | 1000     | 1/1/2018   | 4          | 112    |
| MicroMax                  | 5000     | 1/15/2018  | 4          | 113    |
| WidgetMakers LLC          | 50000    | 2/2/2018   | 5          | 114    |
| International Business Co | 100000   | 3/6/2018   | 4          | 115    |
| Fence Foundation          | 500      | 4/7/2018   | 5          | 116    |
| CA Trust                  | 20000    | 5/9/2018   | 4          | 117    |
| Benevolent Society        | 100000   | 6/10/2018  | 5          | 118    |
| Charitable Giving, Inc.   | 500000   | 7/12/2018  | 4          | 119    |
| ABC Corp                  | 1000     | 8/13/2018  | 9          | 120    |
| Anthony Stark             | 1000000  | 9/14/2018  | 8          | 121    |
| Benevolent Society        | 500      | 10/16/2018 | 4          | 122    |
| Bruce Banner              | 1        | 11/17/2018 | 1          | 123    |
| Bruce Wayne               | 5000     | 12/19/2018 | 8          | 124    |
| CA Trust                  | 500      | 1/20/2019  | 7          | 125    |
| Charitable Giving, Inc.   | 7000     | 2/21/2019  | 7          | 126    |
| Clark Kent                | 100      | 3/25/2019  | 1          | 127    |
| Diana Prince              | 50       | 4/26/2019  | 1          | 128    |
| Donald R Blake            | 75       | 5/28/2019  | 1          | 129    |
| Fence Foundation          | 1500     | 6/29/2019  | 8          | 130    |
| Guy Gardner               | 10       | 7/31/2019  | 1          | 131    |
| International Business Co | 75000    | 9/1/2019   | 7          | 132    |
| Jane Doe                  | 800      | 10/3/2019  | 1          | 133    |
| John Smith                | 90       | 11/4/2019  | 1          | 134    |
| Logan Howlett             | 50       | 12/6/2019  | 1          | 135    |
| MicroMax                  | 6500     | 1/7/2020   | 4          | 136    |
| Natasha Romanoff          | 50       | 2/8/2020   | 1          | 137    |
| Peter Parker              | 20       | 3/11/2020  | 1          | 138    |
| WidgetMakers LLC          | 10000    | 4/12/2020  | 8          | 139    |
| WidgetMakers LLC          | 20000    | 5/14/2020  | 3          | 140    |
| Peter Parker              | 50       | 6/15/2020  | 1          | 141    |
| Natasha Romanoff          | 40       | 7/17/2020  | 1          | 142    |
| MicroMax                  | 30000    | 8/18/2020  | 3          | 143    |
| Logan Howlett             | 500      | 9/19/2020  | 7          | 144    |
| John Smith                | 300      | 10/21/2020 | 6          | 145    |
| Jane Doe                  | 40       | 11/22/2020 | 7          | 146    |
| International Business Co | 40000    | 12/24/2020 | 3          | 147    |
| Guy Gardner               | 50       | 11/22/2020 | 7          | 148    |
| Fence Foundation          | 750000   | 10/21/2020 | 3          | 149    |
| Donald R Blake            | 1500     | 9/19/2020  | 3          | 150    |
| Diana Prince              | 300      | 8/18/2020  | 7          | 151    |
| Clark Kent                | 500      | 7/17/2020  | 6          | 152    |
| Charitable Giving, Inc.   | 40000    | 6/15/2020  | 3          | 153    |
| CA Trust                  | 1500000  | 5/14/2020  | 3          | 154    |
| Bruce Wayne               | 10000000 | 4/12/2020  | 3          | 155    |
| Bruce Banner              | 100      | 3/11/2020  | 6          | 156    |
| Benevolent Society        | 500000   | 2/8/2020   | 3          | 157    |
| Anthony Stark             | 10000000 | 1/7/2020   | 3          | 158    |

  </details>
 
## Relationships

 To answer the questions I created relationships between the three tables using star schema model.

-  Fact Table: `Donation`
-  Dimentional Tables: `Campaign` & `Donor`

![image](https://user-images.githubusercontent.com/10958742/124781085-cb393f80-df4b-11eb-93c1-99de51952a66.png)



  ## Questions 
  
1)	How much money was raised month over month for the last three years, by department?
2)	What are the most successful campaigns year over year by Channel and Sub-Channel?
3)	Who are the top five Donors by DonorType for the latest year?
4)	What was the income raised month over month for the last three years by country?
5)	What percent of income was raised outside the US year over year?

## Solution.

Q1)	How much money was raised month over month for the last three years, by department?

Visual: `matrix`

Columns: `Campaign.department` 

Rows: `Donation.Amount`, `donation.gift date`(Month) 

![image](https://user-images.githubusercontent.com/10958742/124780142-0a1ac580-df4b-11eb-8327-719cba4f40fd.png)

Q2) What are the most successful campaigns year over year by Channel and Sub-Channel?

Visual: `Slicer`

Filters: `donation.gift date`(Year)

Select a filter to compare years

![image](https://user-images.githubusercontent.com/10958742/124784099-4865b400-df4e-11eb-95ff-ace159d02dae.png)

Q3) Who are the top five Donors by DonorType for the latest year?

Visual: `Multi row card` 

DAX calculation:
```SQL
Top5Donors = 
TOPN(5 , Donation, [Amount] )
```

![image](https://user-images.githubusercontent.com/10958742/124782886-45b68f00-df4d-11eb-8382-ed4a4774ba15.png)

Q4) What was the income raised month over month for the last three years by country?

Visual: `Matrix`
Columns: Donor.country, 
Rows: donation.amount, donation.gift date(Month) 

![image](https://user-images.githubusercontent.com/10958742/124783099-77c7f100-df4d-11eb-926e-e2552309efd1.png)

Q5) What total income was raised outside the US year over year?

Visual: `Card`

DAX calculation:
```SQL
OutsidetheUSA = 
CALCULATE(SUM(Donation[Amount]), Donor[Country] <> "United States")
```

![image](https://user-images.githubusercontent.com/10958742/124783788-fde43780-df4d-11eb-9709-1bcc12a3ae64.png)





 
