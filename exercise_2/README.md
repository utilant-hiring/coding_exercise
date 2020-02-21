# Visualizing Solar Data

The National Renewable Energy Laboratory has published two decades worth of data related to Solar Radiation collected in the US. Summary data is made available online at `ftp://ftp.ncdc.noaa.gov/pub/data/nsrdb-solar/summary-stats-2010/dailystats/`.

This exercise requires no background knowledge about the NREL, solar radiation data, or how this dataset was collected. You are only being asked to write code that can produce a visualization based off data stored in their format.

## Daily Stats Data for 20 Years

For each of the 850+ data collection stations, the NREL has published a text file on their FTP site (`ftp://ftp.ncdc.noaa.gov/pub/data/nsrdb-solar/summary-stats-2010/dailystats/`). Each of these files includes:
* A first line that includes the location of the station,
* A table giving average, month-by-month statistics for the full 20 year time span (1991-2010), and
* Twenty more tables, each giving month-by-month statistics for a single year in that time span.

(Note: each of the 21 tables includes 13 rows. Rows 1-12 are data on a month-by-month basis. The 13th row includes column-by-column summary statistics for the full table.)

There are many columns in each of these tables. For this exercise, we only care about values from 3 columns: `AVGLO`, `AVDIR`, `AVDIF`. (You do not need to know what these represent. For the curious, these values represent **AV**erage daily total solar radiation for the **GLO**bal horizontal, **DIR**ect normal, and **DIF**fuse horizontal elements. The unit of measure is energy per unit area, measured in Watt-hour per meter-squared. More information is available through [their website](https://www.ncdc.noaa.gov/data-access/land-based-station-data/land-based-datasets/solar-radiation).)

## Exercise:

In a separate file, we'd like you to write code that can open a single file in the format described, parse the data, and output 3 line charts (overlayed or as separate figures in one file) for that station's data on `AVGLO`, `AVDIR`, and `AVDIF` **for the year 2002**. The X-axis here will represent the months of 2002, while the Y-axis will be average daily total solar radiation for the three columns.

Beyond just having the data points represented in the line chart, consider including any other elements in your figures that may make your result easier to interpret -- e.g., a legend, a title, labeled axes, etc.

Usage of your code might look like:
```python
>>> input_file_name = "NSRDB_DailyStatistics_19910101_20101231_700260.txt"
>>> plot_2002_solar_radiation(input_file_name)
Figure saved to Output.png
```

Add an example output plot to the repo along with your code.
