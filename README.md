# SQL Queries: Voting Results 
 
## Summary 
In this challenge we'll be writing some SQL queries to investigate some voting data.  We'll work with a preexisting database.  The queries we write we start simpler and build in complexity as we move through the challenge.  

We'll be presented with a number of requests for data.  For each of them, we'll need to think through how we can get the desired information out of the database and then write the SQL query to get it.
 

## Releases
### Release 0:  Model the Database with Schema Designer
The database we'll be working with is `voting_results.db`.  Open the database using `SQLite3`.  Take a look at the database schema (use the `.schema` command).  There should be three tables: `congress_members`, `voters`, and `votes`.

Model the database schema using the [schema designer].  Be sure to connect primary and foreign keys.  When our schema is complete, take a screenshot of the design and commit it.


### Release 1: Query the Datbase
For each of the data requests below, write a SQL query that will retrieve the appropriate data.  Record our query for each request in the file `queries.md`.

If we want to double-check the results of our queries, each desired result set is recorded as a CSV file in the `query_results` directory—viewing the CSV files on GitHub will present them as nicely formatted tables.


1. How many votes were cast for the politician with id 524?

2. How many votes were cast for Rep. Erik Paulsen?

3. What were the names of the eight congress members who received the most votes and how many votes did each receive?

4. What were the names of the congress members who received less than ten votes and how many votes did each receive?

5. What are the first and last names of the female voters who voted for Rep. Marcia Fudge?

6. Which Congress member received the most votes? List their name and a count of their votes.  Who were the people that voted for that politician?  List their names, gender and party.

7. How many votes were received by Congress members whose communication grade average was less than 9 (this number can be found in the `grade_current` field)? List their name, location, grade since 1996, and the vote count.

8. What 10 states had the most voters turnout? (Does this correspond to the population of those states?) List the people that voted in the top state's elections.  (It will be a big list, and you can use the results from your first query to help simplify this next query.)

9. List the people that voted more than 2 times? (It should only be once for their Senator and once for their representative!)  Ay Caramba!  We have some serious ballot stuffing! Report this to the Election Board!

10. Did anyone vote for the same politician twice? What was the name of the voter and the politician they voted for?  Pretty sneaky...

Paste the text from your `trace` file into the source file along with the schemas of the 3 tables. If you want to use this as a future reference, you might also include some on the output of the queries to help remember all this syntax!


<!-- ##Optimize Your Learning  -->

##Resources


[schema designer]: https://schemadesigner.devbootcamp.com/
