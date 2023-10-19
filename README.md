# Accidents Database

The Accidents Database project aims to collect, clean, and build a comprehensive database of accidents. This database includes various intrinsic and contextual attributes such as severity, location, time, weather conditions, and more, which help us understand how different factors contribute to accidents. The data has been extracted from various sources, audited for accuracy, and loaded into a structured database for analysis.

## Objective

The primary objective of this project is to provide a valuable resource for studying accidents and their contributing factors. This includes detailed information about crash events, vehicles involved, laws violated, and environmental factors.

## Data Sources

We have collected most of our data from reputable sources, including:

- [San Jose Crashes Data](https://data.sanjoseca.gov/dataset/crashes-data)
- [San Jose Crash Data 2011-2020](https://data.sanjoseca.gov/dataset/918fb7f0-60c0-484e-b31c-334d1ec74e92/resource/c19a01f2-33e1-4c66-9498-85d489f90da4/download/crashdata2011-2020.csv)
- [San Jose Vehicle Crash Data 2021-Present](https://data.sanjoseca.gov/dataset/918fb7f0-60c0-484e-b31c-334d1ec74e92/resource/a92d2d50-f8c5-46a3-a0a8-5eaf8b3a865f/download/vehiclecrashdata2021-present.csv)

## Architecture

<img width="874" alt="Screen Shot 2023-10-19 at 4 26 52 PM" src="https://github.com/RuthwikBg/Accident-database-project/assets/113303754/1c92a0be-2c39-4c48-b719-fb2a9dbf97d3">


## Data Cleaning Process

The collected data was audited, cleaned, and validated to ensure its accuracy and completeness. Data cleaning involved:

- Removing rows with NULL or unknown values.
- Filling empty rows in the "Age" column with the mean value.
- Adjusting blank rows in the "Sex" column with the nearest row's string value.

## Database Structure

The data has been organized into a structured database using MySQL. The database schema includes four tables:

1. **Crashes Table:** Contains detailed information about crash events, including location, severity, and involved parties.

2. **Vehicles Table:** Provides vehicle-level details of the crash, including vehicle types, driver information, and injury severity.

3. **Factors Table:** Includes information about environmental factors such as weather, road conditions, and time of day.

4. **Laws Table:** Contains information related to violation codes and their descriptions.

## Data Normalization

To ensure data integrity and eliminate redundancies, the data has been normalized into the following forms:

### First Normal Form (1NF)

- All tables have single-valued attributes.
- Attribute domains remain consistent.
- Each attribute/column has a unique name.

### Second Normal Form (2NF)

- All requirements for 1NF are met.
- No partial dependencies exist.
- All columns are dependent on the primary key.

### Third Normal Form (3NF)

- All requirements for 2NF are met.
- No transitive dependencies exist.

## Database Structure

The normalized database includes four tables, each serving a specific purpose:

- **Crashes Table:** Contains crash event-level details, including location, severity, and involved parties.

- **Vehicles Table:** Provides vehicle-level details, including vehicle types, driver information, and injury severity.

- **Factors Table:** Includes environmental factors, such as weather, road conditions, and time of day.

- **Laws Table:** Contains information related to violation codes and their descriptions.

## Usage

The data and database structure are available in the associated CSV files and database loaders in this GitHub repository. Feel free to use this resource for research, analysis, or any other purpose that may benefit from a comprehensive accidents database.


Thank you for your interest in the Accidents Database project! If you have any questions or would like to contribute, please don't hesitate to get in touch.


