# Historical-Data-Transformation
Brief

This Python script transforms current employee data from a columnar format into a historical, row-based versioning format suitable for database storage. The transformation process involves deriving effective and end dates for each historical record, ensuring consistency in data representation, and handling missing or incomplete data.
Key Features:

    Effective and End Dates: Derives effective and end dates for each historical record to avoid data overlap.
    Data Transformation: Transforms columnar data related to compensation, engagement, and performance reviews into a row-based format.
    Data Copying: Ensures unchanged values for fields without associated dates across different records and accurately reflects all relevant data from the input file in the output format.
    Output Format: Generates a CSV file formatted for historical data analysis, including employee identifiers, compensation details, dates, performance ratings, and engagement scores.

Methodology:

    Data Preparation: Reads the input CSV file containing employee data.
    Transformation: Applies transformation rules to convert columnar data into a row-based historical versioning system.
    Effective and End Dates Calculation: Derives effective and end dates for each historical record.
    Data Copying: Handles missing or incomplete data by inheriting values from the most recent past record for the same employee.
    Output Generation: Writes the transformed data into a CSV file for further analysis and database storage.
