# Chicago 311 Calls and Accidents Analysis
As part of my Data Mining Project for the Northeastern University, my group and I pulled data from the Chicago Open Data Portal to merge 311 Service Calls related to road condtions and accidents in the city.
## Project Overview
Our group aimed to find out if there were instances of road obstructions or problems in the same streets where an accident happened.
## Dataset
Chicago Open Data: 311-Calls and Crashes
## Key Findings
This analysis identified 1,739 instances in which a 311-service request was reported on a street where one or more traffic crashes occurred either shortly before or shortly after the call. This overlap highlights a meaningful relationship between public service complaints and roadway safety conditions.
By leveraging AWS tools—including S3, Glue Studio, and Athena—we were able to efficiently ingest, clean, transform, and organize large volumes of data from multiple sources. These steps enabled the development of a data-driven dashboard that demonstrates the value of the 311 service in identifying potential safety concerns and supporting proactive city operations.
## Technologies Used
- Python
- Spark
- Jupyter Notebook
## Files
- chicago_311_calls.json — Raw lastest 10,000 311 Calls
- chicago_crashes.json — Raw latest 10,000 crashes
- 311_sr_type_unique.json — Unique service request types (to allow for filtering)
- filtered_311_calls.json — Selected only calls related to road conditions
- clean_311_calls.json — Calls were checked for nulls, date and time was standardized, addresses were standardized
- clean_crashes.json — Crashes records were checked for nulls, date and time was standardized, addresses were standardized
- joined_final_calls_crashes.json — Calls and Crashes were joined in the address field
