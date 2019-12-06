Part 1:
//Start 3140.db
~/desktop/cisc_3140/sqlite $sqlite3 3140.db
SQLite version 3.24.0 2018-06-04 14:10:15
Enter ".help" for usage hints.
//Create table EvaSheet for data
sqlite> create table EvaSheet (one varchar(10), well smallint, clear smallint, enthustic smallint, learnNew smallint, f1 text, f2 text, f3 text, f4 text);
//Change mode to csv for import and file location
sqlite> .mode csv
sqlite> .import /Users/Naokikokubyakuin/Downloads/5518.csv EvaSheet
//Calculate the average of each column
sqlite> SELECT avg(well) From EvaSheet;
4.24
sqlite> SELECT avg(clear) From EvaSheet;
4.08
sqlite> SELECT avg(enthustic) From EvaSheet;
4.44
sqlite> SELECT av(learnNew) From EvaSheet;
Error: no such function: av
sqlite> SELECT avg(learnNew) From EvaSheet;
4.44
//Change output format for better view 
sqlite> .mode line
sqlite> select one, well, clear, enthustic, learnNew from EvaSheet;
      one = Timestamp
     well = Presentation was well organized
    clear = Speaker spoke clearly and was easy to understand.
enthustic = Presenter was enthusiastic about the topic.
 learnNew = I learned something new today

      one = 11/6/2019 14:50:06
     well = 5
    clear = 5
enthustic = 5
 learnNew = 5

      one = 11/6/2019 14:50:12
     well = 3
    clear = 4
enthustic = 5
 learnNew = 4

      one = 11/6/2019 14:50:22
     well = 4
    clear = 4
enthustic = 5
 learnNew = 5

      one = 11/6/2019 14:50:26
     well = 5
    clear = 3
enthustic = 5
 learnNew = 5

      one = 11/6/2019 14:50:29
     well = 4
    clear = 4
enthustic = 4
 learnNew = 4

      one = 11/6/2019 14:51:13
     well = 5
    clear = 4
enthustic = 4
 learnNew = 5

      one = 11/6/2019 14:51:48
     well = 5
    clear = 4
enthustic = 4
 learnNew = 5

      one = 11/6/2019 14:52:38
     well = 4
    clear = 5
enthustic = 3
 learnNew = 4

      one = 11/6/2019 14:53:55
     well = 4
    clear = 4
enthustic = 4
 learnNew = 4

      one = 11/6/2019 14:55:30
     well = 4
    clear = 3
enthustic = 5
 learnNew = 4

      one = 11/6/2019 15:03:21
     well = 5
    clear = 5
enthustic = 5
 learnNew = 5

      one = 11/6/2019 15:06:52
     well = 5
    clear = 5
enthustic = 5
 learnNew = 5

      one = 11/6/2019 15:08:41
     well = 4
    clear = 3
enthustic = 4
 learnNew = 4

      one = 11/6/2019 15:27:32
     well = 4
    clear = 4
enthustic = 4
 learnNew = 5

      one = 11/6/2019 16:38:47
     well = 5
    clear = 5
enthustic = 5
 learnNew = 5

      one = 11/7/2019 18:38:58
     well = 5
    clear = 5
enthustic = 5
 learnNew = 5

      one = 11/7/2019 19:07:36
     well = 5
    clear = 5
enthustic = 5
 learnNew = 5

      one = 11/8/2019 15:34:05
     well = 5
    clear = 5
enthustic = 5
 learnNew = 5

      one = 11/9/2019 22:16:51
     well = 5
    clear = 5
enthustic = 5
 learnNew = 5

      one = 11/11/2019 0:44:00
     well = 4
    clear = 4
enthustic = 5
 learnNew = 4

      one = 11/11/2019 19:23:39
     well = 3
    clear = 2
enthustic = 4
 learnNew = 3

      one = 11/12/2019 14:32:47
     well = 4
    clear = 4
enthustic = 5
 learnNew = 5

      one = 11/12/2019 18:16:35
     well = 5
    clear = 5
enthustic = 5
 learnNew = 5

      one = 11/21/2019 18:42:31
     well = 4
    clear = 5
enthustic = 5
 learnNew = 5
sqlite> .exit   
.exit
~/desktop/cisc_3140/sqlite $


Part 2: 
Would you prepare differently in the future? How so?
I will try to speak clearly and slowly in the future, I believe that was a lot of information I was trying to fit into the small presentation, so that I was rushing through slides. 
Would you restructure the organization of content in your talk? How so?
I will restructure the organization of content by a bit, I will put up more codes rather than visual image of the presentation. This will help me to dive into the concept more for audiences to understand better. 
What are some enhancements to your presentation that would be relevant (if given more time to prepare or present) that you would include?
	I will prepare better slides, maybe some gif will be helpful in demonstrating some coding issues. 


Are you interested enough in your topic to continue honing it and possibly find another venue to present it again? Perhaps a conference or local programmers’ user group?
Yes, I am interested enough in my topic, I will try my best to present it again with enchanted slides and better talk. 
Analysis of the feedback
How does the open ended feedback differ between lower quantitative scores and higher scores, if applicable?
	I see the difference between lower score and higher score by looking at the data. It’s obvious that people know more about coding and more familiar with OPP will understand the concept and topics better in Swift. People with weaker coding background actually not understanding about what I did in the slides, that why they are confused with the ideas and concepts. I will try to balance these two and make the slides easier to understand and dive into harder coding part more smoothly.
