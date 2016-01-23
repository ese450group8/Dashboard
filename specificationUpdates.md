# specifications for the patient section of web app

- Break the line in the graph where there are gaps of data (no data)
  - connecting the line where there is no data is misleading
- Use the same scale for every person (0 to 500 is reasonable)
- May be useful to mark any time periods where the patient's level is above his/her usual average
- Must figure out how to determine time of blood-glucose reading
  - time buckets for each patient?
  - test run for each patient and base pattern off of that?

# specifications for the population section of web app

- Make each row only one patient
  - right now, it's multiple rows for patient. We don't want that
- Outliers: delete ones greater than 700
