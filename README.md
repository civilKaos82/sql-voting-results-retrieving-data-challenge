# SQL Queries: Voting Results 
 
## Summary 
In this challenge we'll be writing some SQL queries to investigate some voting data.  We'll work with a preexisting database.  We'll be presented with a number of requests for data.  For each of them, we'll need to think through how we can get the desired information out of the database and then write the SQL query to get it.
 

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

6. What are the ids and names of the politicians for which Lizzie Rath voted?

7. What are the current grades, names, locations, and vote counts for all politicians whose current grades are less than 9.00 ordered by current grade from high to low?

8. Which state had the largest number of voters (not votes) and how many unique voters voted in that state?

9. Voters should cast a maximum of two votes: one for the representative and one for the senator.  What are the first and last names of the voters who voted more than five times and how many times did each of them vote, ordered first by the number of votes cast and then alphabetically by first name?

10. Did anyone vote for the same politician twice? What was the name of the voter and the politician they voted for?  Pretty sneaky...

Paste the text from your `trace` file into the source file along with the schemas of the 3 tables. If you want to use this as a future reference, you might also include some on the output of the queries to help remember all this syntax!


<!-- ##Optimize Your Learning  -->

##Resources


[schema designer]: https://schemadesigner.devbootcamp.com/
