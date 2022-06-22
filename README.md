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

To run this analysis we had to answer some few questions by running some few codes
