## Predictive Maintenance: Machine Learning to Prevent Equipment Breakdowns
This repository contains a comprehensive analysis and implementation of a Predictive Maintenance project using Python. The goal is to predict equipment failures by analyzing historical sensor data and machine characteristics.

# Data Source:
https://www.kaggle.com/code/arnabbiswas1/predictive-maintenance-exploratory-data-analysis

# Data Description: 

There are 5 CSV files consisting of:

Telemetry Time Series Data (PdM_telemetry.csv): It consists of hourly average of voltage, rotation, pressure, vibration collected from 100 machines for the year 2015.

Error (PdM_errors.csv): These are errors encountered by the machines while in operating condition. Since, these errors don't shut down the machines, these are not considered as failures. The error date and times are rounded to the closest hour since the telemetry data is collected at an hourly rate.

Maintenance (PdM_maint.csv): If a component of a machine is replaced, that is captured as a record in this table. Components are replaced under two situations:

During the regular scheduled visit, the technician replaced it (Proactive Maintenance) A component breaks down and then the technician does an unscheduled maintenance to replace the component (Reactive Maintenance). This is considered as a failure and corresponding data is captured under Failures. Maintenance data has both 2014 and 2015 records. This data is rounded to the closest hour since the telemetry data is collected at an hourly rate. Failures (PdM_failures.csv): Each record represents replacement of a component due to failure. This data is a subset of Maintenance data. This data is rounded to the closest hour since the telemetry data is collected at an hourly rate.

Metadata of Machines (PdM_Machines.csv): Model type & age of the Machines.

Data preprocessing and feature engineering is done here: 'https://github.com/smkandel/DS_project/blob/main/Predictivemaintenance_FeatureEngineering.ipynb'

