# E-Commerce-Data-Analytics-Using-AWS-Big-Data

## E-commerce company: cadabra.com

1. Requirement 1: Proivde an order history function on the site's mobile app. Simulate order data being generated on ec2 instance and publish that data using Kinesis data stream into an AWS Lambda function which in turn will populate an order DB in Dynamo DB that our app can read from.

2. Requirement 2: Automated Product Recommendations to our customers online which involves training a ML based on aggregate customer purchasing data. To build this we'll publish our order data through Kinesis Firehose into a data lake hosted in Amazon S3 and spin up an Amazon Elastic map reduce cluster to produce recommendations model using Apache Spark.

3. Requirement 3: Transaction Rate Alarm- This is am operational system that alerts us if an unexpected rate of orders comes in all of a sudden. This might indicate some sort of attack that someone needs to deal with immediately. Hence, it must work in real time. To build this we will use Kinesis data stream and Kinesis data analytics to monitor our incoming orders and use a lambda function to fire off alarms using Amazon SNS to a cell phone when something unusual happen. 

4. Requirement 4: Near-real-time log analysis- Analyse server log data in near real time for operational purposes. For this requirement we will use Kinesis firehose to pump Apache log data directly into the Amazon Elastic Search service where we can easily query that data and build dashboards for it using Cabana.

5. Requirement 5: Data warehousing and visulaization- For business analysis purposes by using AWS Glue, Athena, RedShift and QuickSight on top of our S3 data lake.


