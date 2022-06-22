# Amazon_Vine_Analysis

# Overview of the analysis

The Amazon Vine programm is a service that allows manufactures and product developper to receive reviews for their products.

Companies will pay a fee to Amazon for them to sell their products to members who are then required to leave a review of the product they have received on the website.
We are running this analysis on Amazon's Home Improvement Review to determine if there is any bias in review written by the Amazon Vine Programm since they received incensitives for the reviews they left.

# Resources

- Data Source : https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Home_Improvement_v1_00.tsv.gz
- Software: PySpark, Google Colab, Postgres, PgAdmin, AWS RDS, AWS S3.

# Result

An AWS RDS database was first created with tables in pgAdmin. Using PySpark we then transformed the dataframe to match the tables schema in pgAdmin.
Then, the transformed data has been uploaded into appropriate tables in pgAdmin.

![image](https://user-images.githubusercontent.com/99924850/175111870-5f9c6b39-c2a8-4b91-a4b2-ede8e52b10aa.png)

To run this analysis we had to answer some few questions by running some few codes to filter our data


- How many Vine reviews and non-Vine reviews were there?

The total paid review were 255
The total unpaid review were 36400

![image](https://user-images.githubusercontent.com/99924850/175115438-094335ca-2dd4-4bf4-8136-ec5be7aaf3ef.png)

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

There were 120 paid five stars reviews when the unpaid reviews were 17167

![image](https://user-images.githubusercontent.com/99924850/175115722-29135c95-e8a8-4c42-94a8-2883d0d78fe9.png)

- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

The percentage of paid reviews was 0.33% when the unpaid reviews was 47.16%

![image](https://user-images.githubusercontent.com/99924850/175115872-f1d8994e-33e8-4c75-9351-64eb924c7316.png)

# Summary 

Based on the figures we were able to get by filtering our data based on the vine program there is no evidence that shows a bias in the reviews. The results we got with our analysis showed that only 0.33% of the 5 stars reviews were paid whereby the 47.16& were unpaid. The unpaid reviews make up for almost 99.9% of the reviews which means that there is no strong evidence that prooves that the reviews were biased.

We used alot of filtering to conduct this analysis it would have been helpful to review the dataset as it is as this could have given us more informations and would have allowed us to further support our assumption that the reviews were not biased.



