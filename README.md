# Weather-Data-ETL-Pipeline-with-Slack-and-Email-Notifications

This project implements an ETL pipeline on AWS EC2 to extract weather data, transform it using Python, and store it in S3 buckets. It also features Slack and email notifications for any pipeline failures.

### Description

This Python-based pipeline automates the process of acquiring weather data, applying transformations, and storing the processed data in a scalable and accessible location (S3). It leverages the power of AWS services for efficient execution and notification functionalities.

### Features

* **Data Extraction:** Fetches weather data from a weather API (details to be configured).
* **Data Transformation:** Applies necessary transformations to the data using Python.
* **Data Loading:** Stores the transformed data in designated S3 buckets for further analysis.
* **Failure Notifications:** Sends Slack and email notifications in case of pipeline failures.

### Installation

**Prerequisites:**

* An AWS account with access to EC2, S3, Simple Email Service (SES), and (optionally) AWS Lambda for notifications.
* Python 3.x with required libraries (e.g., requests, boto3, etc.). Configure specific libraries based on your chosen weather API and transformation needs.
* Weather API access (refer to the API provider's documentation for setup).

**Steps:**

1. **Configure AWS Services:**
    * Create an EC2 instance with appropriate permissions to access S3 and other services.
    * Set up S3 buckets to store the weather data.
    * Configure SES for email notifications (optional).
    * Consider setting up AWS Lambda for notification functionalities (optional).
2. **Project Setup:**
    * Clone this repository to your local machine.
    * Install the required Python libraries using `pip install -r requirements.txt`.
3. **Configuration:**
    * Update the `config.py` file with your AWS credentials, S3 bucket names, weather API details, and notification preferences (email addresses and Slack webhook URL, if applicable).

### Usage

1. **Run the Pipeline Script:**
    * Navigate to the project directory in your terminal.
    * Execute the script using `python main.py`. This will initiate the ETL process and store the processed data in S3.

### Contributing

We welcome contributions to this project! Please refer to the `CONTRIBUTING.md` file for guidelines on pull requests, coding standards, and testing procedures.

### License

This project is licensed under the MIT License (see LICENSE.txt).

### Additional Information

* **Authors:** Vishnusai Bhadramraju
* **Contact:** vishnusaibhadramraju1@gmail.com
