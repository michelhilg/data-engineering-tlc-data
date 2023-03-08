# Cloud Data Engineering - TLC Trip Record Data

## 1. Introduction

This repository has the goal to present the pipeline documentation and code to a data engineering task performed on a cloud based platform for the TLC Trip Record Data.

The challenge was to build a pipeline that automatically imports the TLC datasets from the web page [TLC NYC Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page), after, transforms, and loads following best practices on data engineering field.

To perform this task, a cloud data provider was selected. The ideia behind the cloud environment was bring the application more closely to the modern status of data engineering solutions.

## 2. What is the TLC data?

The New York City Taxi and Limousine Commission (TLC), created in 1971, is the agency responsible for licensing and regulating New York City's Medallion (Yellow) taxi cabs, for-hire vehicles (community-based liveries, black cars and luxury limousines), commuter vans, and paratransit vehicles.

This project uses open-source datasets from the NYC TLC by technology providers authorized under the Taxicab & Livery Passenger Enhancement Programs (TPEP/LPEP). The datasets could be checked at: https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page.

Note: This project was made first locally and then added to git.

## 3. Repository Structure

The repository contain the following deliverables:

**Markdown Files**
1. Description and definition of single steps of the pipeline
2. Instructions on how to run and deploy the pipeline
3. Definition of ouput datasets (schema)
4. Future Steps

**Folders**
1. Python Notebooks with pipeline transformation code
2. Validation queries
