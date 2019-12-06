# Part 1
- //Start 3140.db
- ~/desktop/cisc_3140/sqlite $sqlite3 3140.db
- SQLite version 3.24.0 2018-06-04 14:10:15
- Enter ".help" for usage hints.
- //Create table EvaSheet for data
- sqlite> create table EvaSheet (one varchar(10), well smallint, clear smallint, enthustic smallint, learnNew smallint, f1 text, f2 text, f3 text, f4 text);
- //Change mode to csv for import and file location
- sqlite> .mode csv
- sqlite> .import /Users/Naokikokubyakuin/Downloads/5518.csv EvaSheet
- //Calculate the average of each column
- sqlite> SELECT avg(well) From EvaSheet;
- 4.24
- sqlite> SELECT avg(clear) From EvaSheet;
- 4.08
- sqlite> SELECT avg(enthustic) From EvaSheet;
- 4.44
- sqlite> SELECT av(learnNew) From EvaSheet;
- Error: no such function: av
- sqlite> SELECT avg(learnNew) From EvaSheet;
- 4.44

  
  # Part 2
