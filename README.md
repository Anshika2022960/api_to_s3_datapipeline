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
# Tech Stack
Python
Pandas
Requests
AWS S3
Boto3
