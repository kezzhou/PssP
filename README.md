# Patient Self Service Portal - Admin View
HHA 504 // Week 9 // Assignment 7

## Description:

In this repository, our patient self service portal becomes more fleshed out with its addition of tangible tables, dummy data, and adding/editing/updating/deleting features. With our given source code as a base, we can ensure that our own data is connected to the app properly by adjusting table connections and endpoint parameters in the app.py. To ensure that our information is displayed correctly, we focus mainly on patient_all.html and patient_details.html. Specifically, from the source code, we have adapted three new fields for patients: Sex, Birthdate, and Zip Code, based on gender, dob, and zip_code fields from our original patient_portal.patients table. These fields are added uniformly across the patient master list, the individual patient info views, as well as where relevant when adding and updating patient information.

## The four components found in this repository are:

1. app.py (python script) - through sqlalchemy and pymysql, we can foster a connection to Azure Database for MySQL Server and pull table queries into classes for respective htmls, as well as create the necessary endpoints for proper launching and access of the site.

2. templates (folder) - this folder houses our html files:
- about.html
- base.html
- header.html
- landing.html
- patient_all.html
- patient_details.html
- signin.html


3. static (folder) - this folder houses our css files:
- bootstrap.css
- dashboard.css
- landing.css
- signin.css

4. images (folder) - this folder houses image files picturing the following:
- The /patients list page with dummy data and the three newly added fields
- The /view page of a single patient with the three newly added fields
- The modal window for editing a patient's details with the three newly added fields available for editing and updating
- The modal window for adding a new patient with the three newly added fields available for editing and updating

## Resources:

[Source Code for Project](https://github.com/hantswilliams/HHA-504-2022/tree/main/Part6_CRUD)

## Requirements:

- VS Code/Python Program of Choice
- MySqlWorkbench/popSQL/Equivalent
- Azure Database for MySQL Servers/GCP/Amazon/Equivalent
- Chrome/Safari/Browser of Choice

For package requirements and dependencies, please refer to requirements.txt and the notes section below.

## Notes:

We are using Python 3.9.12 Conda, which is important to note since Python has had a recent update, and users' local machines' updated Pythons can bring about dependency issues.

For Macs with M1 processors, pymysql will be the way to go for creating a connection rather than mysqldb.