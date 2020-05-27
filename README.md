# How-to-practice-Spark-by-open-database-on-AWS-S3

As a new grad or entry level data engineer, 
you might want to learn more about AWS/ETL/big data analytics, 
then AWS could be a good fit for you as a overall provider. 

This is just an introduction of building your first data engineering study platform on AWS
Let's get start it!

### What you might need for building a  machine learning model:

    * data: data sources, data storage, data wrangling
    * data modeling by pyspark
    * machine learning by tensorflow


### Get Start!

1. Open a free-tier AWS account
      * I would prefer east-1 and east-2, ohio & Vrigina
      * reason: slightly different on price, so choose the area based on speed, influeced by physical distance.

2. Find a open source big data set*

    a. AWS Data Exchange: (access to the third party data)
    
      * AWS data exchange program is a market for people to provide their own data, and to purchase data.
        There are a lot data sale for free in 12 months, you need to subscribe them.
      * I don't recommand get data from kaggle for budget reason.
        but you can refer to this, download/upload to S3 from kaggle by commandline 
        [https://github.com/floydwch/kaggle-cli](https://github.com/floydwch/kaggle-cli)
    
    b. Export data from Data Exchange to E3
    
      * get the updated once the data origin updated:
      * [Refer to step by step](https://aws.amazon.com/blogs/big-data/find-and-acquire-new-data-sets-and-retrieve-new-updates-automatically-using-aws-data-exchange/)
    
   


3. Services you need on AWS
```

    ** S3 : Seen as simple storage 
            Store the data you retrived from 'Exchange Data' and created the Aimed bucket for storing cleaned data
    ** Athena: Run SQL Queries, data modeling, Generate the tables you need
               Results of Queries on Athena will be stored in the S3 bucket you set.
    
    
    ** Glue:
      * Clawer :  horizontally connect you to S3 and Athena by automatic clawer, generated the catelog 
      * Catelog:  a automatic tool to build a data warehouse to store
      * ETL: dynamic or editable scripts by built-in Spark(in Scala or python) for devloper to create based on need
      * Job Scheduler
```

