# SQL Queries: Voting Results 
 
## Summary 
In this challenge we'll be writing some SQL queries to investigate some voting data.  We'll work with a preexisting database.  The queries we write we start simpler and build in complexity as we move through the challenge.  

We'll be presented with a number of requests for data.  For each of them, we'll need to think through how we can get the desired information out of the database and then write the SQL query to get it.
 

##Releases

###Release 0 :  Download and set up the Poll DB

Download the database [here](https://github.com/downloads/dbc-challenges/binary_store/congress_poll_results.db), and open it up with `sqlite3 congress_poll_results.db`.

Take a look at the schemas included.  Type `.schema`.  There should be 3 tables, `congress_members`, `voters`, and `votes`.  We're going to be doing some queries to get some insights into the data set.

We suggest copying the schemas and putting them into a text file that's easy to reference.  You'll need it as we try to access multiple columns across multiple tables.

Type `.trace sql_history.txt` to create a file to save all the commands you do for reference and for submitting this challenge  (NOTE: '.trace' only works with the latest version of sqlite3.  If you are having problems running it on a DBC machine, quit out of the sqlite3 console and type `brew link sqlite3` from the command line.)  


###Release 1 : Query to extract voting data

Let's get going with some simple queries.

1. Count the votes for Sen. Olympia Snowe, whose id is 524.

2. Now do that query with a `JOIN` statement without hard-coding the id `524` explicitly, querying both the votes and congress_members table.

3. How about Rep. Erik Paulsen?  How many votes did he get?

4. Make a list of Congress members that got the most votes, in descending order.  Exclude the create_at and updated_at columns.

5. Now make a list of all the Congress members that got the least number of votes, in ascending order. Again, skip the date columns.


###Release 2 : Advanced queries to expose voter fraud

The Election Board suspects there's some cheating going on!  Help them figure out what is going on and if anyone is to blame.

1. Which Congress member received the most votes? List their name and a count of their votes.  Who were the people that voted for that politician?  List their names, gender and party.

2. How many votes were received by Congress members whose communication grade average was less than 9 (this number can be found in the `grade_current` field)? List their name, location, grade since 1996, and the vote count.

3. What 10 states had the most voters turnout? (Does this correspond to the population of those states?) List the people that voted in the top state's elections.  (It will be a big list, and you can use the results from your first query to help simplify this next query.)

4. List the people that voted more than 2 times? (It should only be once for their Senator and once for their representative!)  Ay Caramba!  We have some serious ballot stuffing! Report this to the Election Board!

5. Did anyone vote for the same politician twice? What was the name of the voter and the politician they voted for?  Pretty sneaky...

Paste the text from your `trace` file into the source file along with the schemas of the 3 tables. If you want to use this as a future reference, you might also include some on the output of the queries to help remember all this syntax!


<!-- ##Optimize Your Learning  -->

##Resources