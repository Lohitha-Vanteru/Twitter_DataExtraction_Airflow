# **Twitter_DataExtraction_Using_Airflow**

This project is designed to extract data from Twitter using the Twitter API and load it into an AWS S3 bucket in CSV format. The pipeline is managed and orchestrated using Airflow.

## Architecture

![image](https://github.com/Lohitha-Vanteru/Twitter_DataExtraction_Airflow/assets/113141006/572c815e-975c-4aa5-b5c5-b0afc2c9966a)


- **Twitter API**: Used to collect data from Twitter.
- **Apache Airflow**: Manages and orchestrates the data pipeline.
- **Amazon S3**: Stores the extracted data in CSV format.
- **Amazon EC2**: Virtual Computer (Ubuntu OS)

### Prerequisites
- A Twitter developer account and API key
- An AWS account and S3 bucket set up
- Python 3
- Airflow
- tweepy
- pandas

## Notes

- The pipeline is currently set to extract data from a specific Twitter handle. Update the `run_twitter_etl` function in `dags/twitter_etl.py` to extract data from other sources.
- The pipeline is currently set to load data into a specific S3 bucket. Update the `bucket_name` variable in `dags/twitter_etl.py` to load data into other S3 buckets or in a different format.
- The pipeline is currently scheduled to run every seven days. Update the `schedule_interval` in the DAG to run more or less frequently.

## Conclusion

This project provides a detailed guide on building a data pipeline using Airflow to extract data from the Twitter API, process it using pandas, and load it into an AWS S3 bucket in CSV format. By following the step-by-step instructions in this README, you should be able to set up and run the pipeline successfully.

## Important Considerations

- This project is intended for educational or testing purposes. Before using the data in production, ensure compliance with Twitter's terms of service and relevant laws and regulations.
- Consider data privacy, security, and compliance in any production implementation.

## References
https://blog.quantinsti.com/python-twitter-api/



