# DataEase
The program is being created to minimize data entry errors for laboratory measurements.

## Functionality Required
The program must:

- allow all relevant, valid data to be entered, as per the field chart
- append entered data to a CSV file
  - The CSV file must have a filename
    of abq_data_record_CURRENTDATE.csv, where 
    CURRENTDATE is the date of the checks in 
    ISO format (Year-month-day)
  - The CSV file must have all the fields as per the chart
- enforce correct datatypes per field

The program should try, whenever possible, to:

- enforce reasonable limits on data entered 
- Auto-fill data
- Suggest likely correct values
- Provide a smooth and efficient workflow

## Functionality not Required
The program does not need to:

- Allow editing of data. This can be done in LibreOffice if necessary.
- Allow deletion of data.

## Limitations

The program must:
- Be efficiently operable by keyboard-only users.
- Be accessible to color blind users.
- Run on debian LINUX.
- Run acceptably on a low-end PC.


| Field       | Datatype   | Units  | Range          | Descripton            |
|-------------|------------|--------|----------------|-----------------------|
| Date        | Date       |        |                | Date of record        |
| Time        | Time       |        | 8, 12, 16, 20  | Time period           |
| Lab         | String     |        | A - E          | Lab ID                |
| Technician  | String     |        |                | Technician name       |
| Plot        | Int        |        | 1 - 20         | Plot ID               |
| Seed sample | String     |        |                | Seed sample ID        |
| Fault       | Bool       |        |                | Fault on sensor       |
| Light       | Decimal    | klx    | 0 - 100        | Light at plot         |
| Humidity    | Decimal    | g/m³   | 0.5 - 52.0     | Abs humidity at plot  |
| Temperature | Decimal    | °C     | 4 - 40         | Temperature at plot   |
| Blossoms    | Int        |        | 0 - 1000       | # blossoms in plot    |
| Fruit       | Int        |        | 0 - 1000       | # fruits in plot      |
| Plants      | Int        |        | 0 - 20         | # plants in plot      |
| Max height  | Decimal    | cm     | 0 - 1000       | Ht of tallest plant   |
| Min height  | Decimal    | cm     | 0 - 1000       | Ht of shortest plant  |
| Median      | Decimal    | cm     | 0 - 1000       | Median ht of plants   |
| Notes       | String     |        |                | Miscellaneous notes   |
|Min height  |Decimal   |cm    | 0 - 1000     |Ht of shortest plant |\
+------------+----------+------+--------------+---------------------+\
|Median      |Decimal   |cm    | 0 - 1000     |Median ht of plants  |\
|height      |          |      |              |                     |\
+------------+----------+------+--------------+---------------------+\
|Notes       |String    |      |              |Miscellaneous notes  |\
+------------+----------+------+--------------+---------------------+\
