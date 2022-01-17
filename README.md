# Data-Pipeline-using-Apache-Spark-and-AWS-EMS-S3-Redshift-Spectrum

## Pre-Requisites(Mac OS)

### 1. Docker
https://docs.docker.com/engine/install/

### 2. PostgresSQL (Using Brew)

Installing Brew
-- /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

Updating Brew
-- brew doctor
-- brew update

Installing Postgres
-- brew install postgresql

### 3. AWS

### 4. AWS CLI
Installing CLI

-- curl "https://awscli.amazonaws.com/AWSCLIV2.pkg" -o "AWSCLIV2.pkg"
-- sudo installer -pkg AWSCLIV2.pkg -target /

## Objective

We will be using Airflow to orchestrate the following tasks:

    1. Classifying movie reviews with Apache Spark.
    2. Loading the classified movie reviews into the data warehouse.
    3. Extracting user purchase data from an OLTP database and loading it into the data warehouse.
    4. Joining the classified movie review data and user purchase data to get user behavior metric data.
 ![alt text](https://github.com/ddahiya16/Data-Pipeline-using-Apache-Spark-and-AWS-EMS-S3-Redshift-Spectrum-/blob/main/images/diag_data_flow.png)
 
## Design

![alt text](https://github.com/ddahiya16/Data-Pipeline-using-Apache-Spark-and-AWS-EMS-S3-Redshift-Spectrum/blob/main/images/diag_design.png)
