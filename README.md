## NOTE:

I'm not including the original gzip data set in this repo because of the file size.
Please either run on the included parquet data or grab the data set from Kaggle
and unzip it into the data folder (https://www.kaggle.com/datasets/ethon0426/lending-club-20072020q1?resource=download).

# Objective

As supplementary material for my application to Pay Ready, I'm going to build a
sample pipeline using real-world loan data for finding high-value debtors to prioritize for collections.
I've chosen this problem space because it is close enough to Pay Ready's business to be relevant,
even though it's not identical.

The data set was pulled from Kaggle.
It's publicly available Lending Club data from 2007-2020.


## Approach

I'm going to use PySpark to do some basic data exploration and hopefully I'll be able to
build a basic pipeline that includes some data quality checks and that filters the data down to
what we're ultimately looking for. Since this is supplemental material I haven't been asked to provide,
I'm going to timebox it to 2-3 hours. I'm also pulling some boilerplate code from my previous work
for handling gzip/csv -> parquet conversion. Even if the analysis doesn't dive super deep, hopefully it can
serve as proof of my abilities and my enthusiasm and that I'd be a good fit for the job.

It's also worth noting that this is only a data pipeline in the loosest sense. I'll be using a jupyter notebook and doing mostly manual
analysis because it's what is realistic for a couple hour's worth of work. It's probably closer to data science than
data engineering, but I'm really just hoping to back up my resume with some general proof of ability. I've got the right experience
and if hired would be excited about implementing larger-scale, fully automated data pipelines using some/all of a DAG-based scheduler like Airflow,
high-volume storage like S3, a relational DB of some kind, and data replication to our data warehouse of choice. If we have another interview in the future,
I'd also be happy to dive into this code and talk about some of the decisions I made along the way. This isn't meant to be production-quality,
it's just meant to give a positive signal in addition to things we've covered in our interviews.
