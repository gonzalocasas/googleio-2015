# Real-time analytics for mobile and IoT

Google Cloud Dataflow: fully managed bigdata stack to do real-time analytics

How it works:
 - push the code to google cloud
 - they handle load, batching, scaling, everything
 - then check the data on the Monitoring UI

Data Ingestion:
 - Define once, it accepts almost anything: App Engine, Google Analytics Premium, Cloud Logs, Cloud Pub/Sub, Google Cloud Storage

Processing:
 - BigQuery Storage (tables)
 - BigTable (noSQL)
 - Cloud Storage (files)

Analysis:
 - BigQuery Analytics (SQL)

You can use Apache Spark / Hadoop if you feel like.
Pay for what you consume.

DataFlow is a pipeline processor: takes input -> applies transformations -> emits output, goes into next step of flow.
Transformations can be defined in Java

The most interesting part is the ability to do things like join multiple input pipelines and merge and tag events of one based on the other. Demo was using traffic sensor info stream being tagged based on an traffic accident stream based on whether there is an accident registered.

http://cloud.google.com

Introducing Next, a series of events from Google Cloud Platform: http://cloud.google.com/next