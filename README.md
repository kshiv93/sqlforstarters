create a table to store information about weather observation stations:

-- No duplicate ID fields allowed
CREATE TABLE STATION 
(ID INTEGER PRIMARY KEY, 
CITY CHAR(20), 
STATE CHAR(2), 
LAT_N REAL, 
LONG_W REAL);

populate the table STATION with a few rows:

INSERT INTO STATION VALUES (13, 'Phoenix', 'AZ', 33, 112); 
INSERT INTO STATION VALUES (44, 'Denver', 'CO', 40, 105); 
INSERT INTO STATION VALUES (66, 'Caribou', 'ME', 47, 68);

query to look at table STATION in undefined order:

SELECT * FROM STATION;
ID	CITY	STATE	LAT_N	LONG_W
13	Phoenix	AZ	33	112
44	Denver 	CO	40	105
66	Caribou	ME	47	68
query to select Northern stations (Northern latitude > 39.7): 
-- selecting only certain rows is called a "restriction".
