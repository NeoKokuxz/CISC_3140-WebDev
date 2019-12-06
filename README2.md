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
1. Would you prepare differently in the future? How so?
I will try to speak clearly and slowly in the future, I believe that was a lot of information I was trying to fit into the small presentation, so that I was rushing through slides. 
2. Would you restructure the organization of content in your talk? How so?
I will restructure the organization of content by a bit, I will put up more codes rather than visual image of the presentation. This will help me to dive into the concept more for audiences to understand better. 
3. What are some enhancements to your presentation that would be relevant (if given more time to prepare or present) that you would include?
	I will prepare better slides, maybe some gif will be helpful in demonstrating some coding issues. 


4. Are you interested enough in your topic to continue honing it and possibly find another venue to present it again? Perhaps a conference or local programmers’ user group?
Yes, I am interested enough in my topic, I will try my best to present it again with enchanted slides and better talk. 
Analysis of the feedback
5. How does the open ended feedback differ between lower quantitative scores and higher scores, if applicable?
	I see the difference between lower score and higher score by looking at the data. It’s obvious that people know more about coding and more familiar with OPP will understand the concept and topics better in Swift. People with weaker coding background actually not understanding about what I did in the slides, that why they are confused with the ideas and concepts. I will try to balance these two and make the slides easier to understand and dive into harder coding part more smoothly.
