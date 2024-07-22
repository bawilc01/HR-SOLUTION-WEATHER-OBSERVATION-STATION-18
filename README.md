# HR-Solution-Weather-Observation-Station-18
Solutions for MySQL and SQL Server

## PROBLEM
![image](https://github.com/user-attachments/assets/0c27b23d-2137-47b2-a057-81c2c4e8dbb3)

Query the [Manhattan Distance](https://xlinux.nist.gov/dads/HTML/manhattanDistance.html) between points
and and round it to a scale of decimal places.

## SQL SERVER:
SELECT CONVERT(DECIMAL(16, 4), ABS(MAX(LAT_N) - MIN(LAT_N)) + ABS(MAX(LONG_W) - MIN(LONG_W))) 
FROM STATION;

## MySQL:
SELECT ROUND(ABS(MAX(LAT_N) - MIN(LAT_N)) + ABS(MAX(LONG_W) - MIN(LONG_W)), 4) 
FROM STATION;



