# Tutorial: Intro to AWS Glue

## 1. Create a crawler

You are asked to analyze arrival data for major air carriers to calculate the popularity of departure airports month over month. You have flights data for the year 2016 in CSV format stored in Amazon S3. Before you transform your data, you catalog its metadata in the AWS Glue data catalog.

Let’s add a crawler that infers metadata from these flight logs in Amazon S3 and creates a table in your data catalog.

## 2. Explore table

In the Add crawler tutorial, you created and ran the Flights Data Crawler to create a table definition corresponding to flights data. This tutorial depends on the flightscsv table your crawler created. Let’s view and modify the table that the crawler added to your data catalog.

## 3. Add job

In your journey to perform data analysis using flights data, first you cataloged metadata in your AWS Glue data catalog. This tutorial depends on the flightscsv table you created using the Add crawler tutorial.

Next, you want to convert the CSV files to Parquet format, and drop fields that you do not require your data analysis.

Let’s create an ETL job to extract, transform, and load relevant columns from your flights data from an Amazon S3 source to an Amazon S3 target.

## 4. Results

* the script created by the job is store in this repository
* [download one of parquet files](https://flights-data-transformed.s3.amazonaws.com/part-00000-6db113f1-abf9-48db-9e89-42f7ed84d1d6-c000.snappy.parquet) available on s3


## 5. Additional Reading
Tutorials:
* Tutorial #2: [Legislators database](https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-python-samples-legislators.html)
  - Github repo for [Legislators](https://github.com/aws-samples/aws-glue-samples/blob/master/examples/join_and_relationalize.md)
  - [and instructions](https://github.com/aws-samples/aws-glue-samples/issues/2)
* Tutorial #3: [Medicare Provider payment data](https://github.com/aws-samples/aws-glue-samples/blob/master/examples/join_and_relationalize.md)

Glue Developer Documentation:
* https://docs.aws.amazon.com/glue/latest/dg/start-development-endpoint.html
* https://docs.aws.amazon.com/glue/latest/dg/author-job.html
* https://docs.aws.amazon.com/glue/latest/dg/dev-endpoint.html
