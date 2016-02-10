# Files for HealthKit Dashboard

These are the html/css/js files used to create the web application for ESE Senior Design. They must be run with Python

# Running files with Python

Must have access to the test csv files in the same folder
1. Open up command prompt
2. Go to the folder with all the files
3. Type: python -m SimpleHTTPServer 1111
4. Open up a browser and type in directory: localhost:1111


# specifications for the patient section of web app

- (solved) Break the line in the graph where there are gaps of data (no data)
  - connecting the line where there is no data is misleading
- (solved) Use the same scale for every person (0 to 500 is reasonable)
- May be useful to mark any time periods where the patient's level is above his/her usual average
- Must figure out how to determine time of blood-glucose reading
  - time buckets for each patient?
  - test run for each patient and base pattern off of that?

# specifications for the population section of web app

- (solved) Make each row only one patient
  - right now, it's multiple rows for patient. We don't want that
- Outliers: delete ones greater than 700
- Columns helpful in Population Data
  - Information from patient-entered flowsheet
    - Avg fasting over past 30 days
    - Avg breakfast postprandial (1-3 hrs after break)
    - Avg lunch preprandial
    - Avg lunch postprandial
    - Avg dinner preprandial
    - Avg dinner postprandial
    - Arrow with trends up or down
  - Information from Epic
    - A1C value
    - A1C date
    - Last BP
    - Last Optho
    - Last podiatry

# notes
breakfast: 5 - 11
lunch: 11 - 16
dinner: 16 - 24
