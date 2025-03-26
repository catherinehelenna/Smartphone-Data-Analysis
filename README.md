# Welcome to Value-Buy Smartphone Data Analysis: Insights from Leading Brand Project

This program explores the existing smartphone products with price range from 1 to 5 million IDR to create a new smartphone product with similar features. A smartphone company wants to develop a new, value-buy smartphone to customers by identifying which smartphone features are available within that price range.

---------------------------------------------------------------------------------

#### Case Study:
A lot of Indonesian citizens are tech-lovers; they just cannot resist the temptation of changing their smartphones periodically when a new version has been released. Some considerations to get a new smartphone include design, camera, and specs. With that being said, current smartphones are increasing in variety, fulfilling market demands based on affordability. As the saying goes, there is a price for a value, customers still would like to purchase a value-buy smartphone so it would not bring too much financial problems.

Your company, X, would like to innovate a new smartphone product with a reasonable quality and price so it can label the product as "value buy" for the next release campaign. Your company has been producing smartphones for economic level (price range from 0.5 to 1 million IDR) and wondering to set up a slightly higher price to gain more revenue with its brand new product.

As a data analyst working in company X, you should dig more information about other smartphone brands so you can help your company figuring out what are key features it should include in its new product and how to set up a good price.

---------------------------------------------------------------------------------

#### If you're interested in finding out the data visualization result, click the dashboard link below here!

[Tableau Dashboard Link](https://public.tableau.com/app/profile/catherine.mulyadi/viz/ValueBuySmartphoneDataAnalysis/dashboard)

---------------------------------------------------------------------------------
#### About the data extraction and cleaning process
1. I have scrapped the general product information and its product details from Tokopedia. You can find the csv files.
2. Then, I merged the data to get the dirty_merged_data.csv.
3. Finally, I cleaned the data using several techniques that you can find on the Data Cleaning notebook.
4. When I did analysis, there were some data inconsistencies for IsRated and rating columns found due to my decision on the first round of cleaning (fill in null values wrongly). So, I made the second version of cleaned data. Please use the new_rating column for more accurate data in your analysis.
---------------------------------------------------------------------------------
#### About the data (final_cleaned_data_v2.csv)
| Column Name        | Description                     |
|--------------------|---------------------------------|
| `link`             | Product link                    |
| `name`             | Product name                    |
| `price`            | Product price                   |
| `rating`           | Original product rating         |
| `store_name`       | OL store name                   |
| `store_location`   | OL store location               |
| `product_desc..`   | Product description             |
| `cus_satisfac..`   | Customer satisfaction           |
| `IsRated`          | Flag for null value in rating   |
| `total_rating`     | Number of ratings received      |
| `num_reviews`      | Number of reviews received      |
| `rev_rat_ratio`    | Number of reviews received      |
| `brand_name`       | Brand of the product            |
| `new_rating`       | Updat on product rating         |

Note: The new_rating is calculated by customer satisfaction that shows the proportion of customers giving rate 4 to 5.
So, the following equation was implemented:

```equation
estimated rating = 4.5 * customer_satisfaction/100 + 2.5*(1-customer_satisfaction)/100
```

---------------------------------------------------------------------------------
#### Conclusion from the study
1. Real-life data have many challenges including incompleteness, inconsistent formatting, and redundancy records. For this reason, automating data extraction and cleaning are very challenging since the source link structure changes over time and the available data stored in various formats.
2. The current processed dataset size is still quite small (258 records) for representing the real market situation of smartphones in OL platform (Tokopedia). The data were mostly concentrated by the online stores in Jakarta. However, the findings in this project show which brands dominate presence in the platform, pricing and marketing strategies for selling the product.
3. It is possible, however, challenging to sell a new smartphone brand with price range from 1 to 5 million IDR online considering the reasons:

- The current market share is already highly dominated by the famous brands: Samsung, TECNO, VIVO, and Xiaomi. The other brands (Prince, Advan, EVERCROSS, Nokia, etc.) could only take less than 10% of the total market share for selling similar smartphones.

- Depending on the company's budget, the company needs to consider which key features need to be included in their smartphone product so they can sell within the competitive price range , that is about 1 to 2 million IDR, as how the 50% of total data.

- The company needs to consider selling their new product through other platforms both offline and online to extend their market reach for introducing a new product. In instance, participate in pop-up shops or events, collaborate with social media influencers, in-store promotions can be stimulative for introducing new product to the market. While Jakarta seems to have a high demand, it comes with great competition. So, it would be recommended to explore other cities including Medan, Depok, and Bekasi that also have quite high sales. 
---------------------------------------------------------------------------------
I am open to any feedbacks to improve this project, so you can reach me out at 
catherinehelenna888@gmail.com!
