# Reading Assignment Eight
*Sections Read:*
- [SQL Practice](https://sqlbolt.com/lesson/select_queries_introduction)

### Basic SQL Syntax

`SELECT * FROM myTable`

SELECT is denoting what columns to select; * is saying to select all columns from a table called myTable. 

Let's imagine we have a table called Books with columns named: Title, Author, Year_Published. If you wanted to SQL query the titles from this databse your query would look like this:
`SELECT Title FROM Books`

Now, if we wanted to select the Title AND Year Published our query would look like: `SELECT Title, Year_Published FROM Books`

If you are selecting multiple columns they are separated by a `,`.

Now, queries can also have conditional constraints. You identify these by using the keyword `WHERE`.

```
SELECT Title FROM Books
WHERE Year_Published > 2000
```

This query selects all the book Titles from our database Books where the year published is greater than 2000. 

You can have multiple conditionals too by utilizing the keywords `AND`/`OR`.

Strings can be used in conditionals too! They have their own specific keywords, but may also use `=` for strict comparison. Strings must be within "" to be parsed correctly as table information and not a table value. 

Let's say we want to **add** a new book to our table. How would we do that?

Like this!

```
INSERT INTO Books
(Title, Author, Year_Published)
VALUES("The Great Gatsby", "F. Scott Fitzgerald", 1995)
```

Here are are saying we want to insert a new row into our table Books, and fill the columns Title, Author, Year_Published with the corresponding values of The Great Gatsby, F Scott Fitzgerald and 1995.

Oops, the Great Gatsby wasn't published in 1995! To fix that we would query:
```
UPDATE Books
SET Year_Published = 1925
WHERE Title = "The Great Gatsby";
```

We can also delete rows from our table. Let's say we want to get rid of all the books written by JRR Tolkien. 

```
DELETE FROM Books
WHERE Author = "JRR Tolkien";
```
