# Title
# Automated API to AWS S3 Data Pipeline
This project extracts data from a Randomusers API, transforms JSON into structured format using pandas, and uploads the processed data to AWS S3.
## Overview

This project demonstrates a real-world data engineering workflow where data is extracted from a public REST API, transformed using Python and Pandas, and uploaded to Amazon S3 cloud storage.

This simulates how businesses ingest external API data into cloud infrastructure for analytics, reporting, and further processing.

The pipeline includes:

- Data Extraction from REST API
- JSON Normalization and Transformation
- In-memory CSV generation
- Upload to AWS S3 Bucket
# Architecture Diagram
Randomuses API → Python → Pandas → AWS S3
### Flow

1. Client sends HTTP request (Upload / Download)
2. API authenticates and validates the request
3. API interacts with Amazon S3 using AWS SDK
4. IAM role restricts permissions (PutObject / GetObject)
5. Files are stored securely in a private S3 bucket

## What is the API Used?
## 🌐 About the API

This project uses the **RandomUsers Public API**:

API Endpoint:
https://api.freeapi.app/api/v1/public/randomusers

The API generates random user profile data including:

- Name
- Email
- Gender
- Location
- Phone Number
- Profile Picture
- Date of Birth

The API supports pagination using:
?page=1&limit=500

In this project, we fetch 500 user records in JSON format.

## What is RandomUsers Data?

RandomUsers API generates synthetic user data for testing and development purposes.

This type of data is commonly used for:

- Testing data pipelines
- Practicing ETL workflows
- API integration testing
- Data warehouse ingestion
- Dashboard and analytics development

The data structure is nested JSON and requires transformation before storage.
## 🐍 Why Python?
Python is widely used in Data Engineering because:

- Strong support for REST API handling (requests library)
- Powerful data transformation using pandas
- Seamless AWS integration using boto3
- Automation capabilities
- Large ecosystem of data tools

In this project, Python performs:

1. API Call
2. JSON Parsing
3. Data Normalization
4. Cloud Upload
## ☁️ What is AWS S3?
Amazon Simple Storage Service (S3) is a scalable cloud object storage service provided by AWS.

S3 is commonly used for:

- Data lake storage
- Raw data ingestion
- Backup and archival
- Storing ETL outputs
- Machine learning datasets

In this project, the transformed CSV data is uploaded to an S3 bucket for storage.
## Real-World Use Case
This pipeline simulates:

- Startup ingesting customer data from external API
- Marketing data automation
- ETL ingestion layer
- Cloud-based analytics pipeline
  
# Tech Stack
Python
Pandas
Requests
AWS S3
Boto3
