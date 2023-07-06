For this project, a csv file with up-to-date covid data was downloaded then split into two csv files called 'CovidDeaths' and 'CovidVaccinations'.
It was easier to examine the csv files after reducing the number of columns viewed at a time, and the data was briefly scanned for consistency and data type. 
I turned on filters to see what options were available for columns "continent" and "location", and found that empty cells in "continent" existed for rows in "location" that weren't always locations. 
All rows with a specified continent had a country in the "location" column, however, when "continent" was blank the "location" was for various income levels or a grouping of countries.

The two csv files were then imported to an MSQL database and stored in a project portfolio schema.
The import was completed carefully, ensuring the proper data types were chosen. For example, varchar for "Continent" and "location", and longint for "total_tests".

See SQL_Queries_Covid for details on what information was queried.

See link below for Tableau dashboard created from some of the queries.
https://public.tableau.com/views/Covid2019-2022/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link
