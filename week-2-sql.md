# Week 2 - SQL
## Concepts
- [SQL](https://en.wikipedia.org/wiki/SQL): [ANSI SQL](https://blog.ansi.org/2018/10/sql-standard-iso-iec-9075-2016-ansi-x3-135/), SQL Sublanguages, SELECT clauses
- RDBMS: Relational DataBase Management System, SQL Dialects
- [Relational Databases](https://en.wikipedia.org/wiki/Relational_database): Relations, Records, Keys, Constraints
- [Normalization](https://en.wikipedia.org/wiki/Database_normalization): 1-3 Normal Forms, Candidate/Composite/Foreign/Primary Keys
- Multiplicity & Joins
- Database Transactions: [ACID Properties](https://en.wikipedia.org/wiki/ACID), [Isolation Levels](https://en.wikipedia.org/wiki/Isolation_(database_systems)#Isolation_levels)

## Tools 
- AWS RDS: RDBMS hosted and managed by Amazon, on their servers
- PostgreSQL: Open Source RDBMS
- DBeaver: Utility for working with databases

## SQL Language
- Sublanguages:
  - [DQL](https://en.wikipedia.org/wiki/Data_query_language): SELECT
  - [DML](https://en.wikipedia.org/wiki/Data_manipulation_language): INSERT, UPDATE, DELETE
  - [DDL](https://en.wikipedia.org/wiki/Data_definition_language): CREATE, ALTER, DROP
  - [DCL](https://en.wikipedia.org/wiki/Data_control_language): GRANT, REVOKE
  - TCL: SAVEPOINT, COMMIT, ROLLBACK
- SELECT clauses: (The best way to learn these is to use them.  I recommend SQL Bolt -- ADK)
  - FROM: specify table
  - WHERE: filter records
  - GROUP BY: group records
  - HAVING: filter groups
  - ORDER BY: order results
  - LIMIT: limit to N results
  - OFFSET: skip first N results
- [Data Types](https://www.postgresql.org/docs/current/datatype.html)
  - boolean
  - integer
  - numeric
  - varchar
  - text
  - serial
  - timestamp
  - interval
  - json

## PostgreSQL Features
- [ACID Transactions](https://www.postgresql.org/docs/12/tutorial-transactions.html)
- [Indexes](https://www.postgresql.org/docs/12/indexes-intro.html)
- Sequences:
  - [CREATE SEQUENCE](https://www.postgresql.org/docs/12/sql-createsequence.html)
  - [SERIAL Datatype](https://www.postgresql.org/docs/12/datatype-numeric.html#DATATYPE-SERIAL)
- [Triggers](https://www.postgresql.org/docs/12/trigger-definition.html)
- [Views](https://www.postgresql.org/docs/12/tutorial-views.html) & [Materialized Views](https://www.postgresql.org/docs/12/rules-materializedviews.html)
- [Built-in Functions and Operators](https://www.postgresql.org/docs/12/functions.html):
  - [Strings](https://www.postgresql.org/docs/12/functions-string.html)
  - [Date/Time](https://www.postgresql.org/docs/12/functions-datetime.html)
  - [Pattern Matching](https://www.postgresql.org/docs/12/functions-matching.html)
- [Functions](https://www.postgresql.org/docs/12/xfunc.html): 
  - [CREATE FUNCTION](https://www.postgresql.org/docs/12/sql-createfunction.html)
  - [SQL Language Functions](https://www.postgresql.org/docs/12/xfunc-sql.html)
  - [PL/pgSQL](https://www.postgresql.org/docs/12/plpgsql-overview.html)
- [Stored Procedures](https://www.postgresql.org/docs/12/xproc.html), note these are very different in other SQL dialects
- [Query Planner](https://www.postgresql.org/docs/12/using-explain.html)

# Articles
- [Why We Still Use SQL](https://blog.sqlizer.io/posts/sql-43/)
- [Why Postgres](http://www.craigkerstiens.com/2012/04/30/why-postgres/)
- [Why Use Postgres, 5 Years Later](http://www.craigkerstiens.com/2017/04/30/why-postgres-five-years-later/)
- [Postgres as Pub/Sub & Job Server](https://layerci.com/blog/postgres-is-the-answer/)
- [PostgreSQL Features You May Not Have Tried But Should](https://pgdash.io/blog/postgres-features.html)
- [A Simple Guide to Five Normal Forms](http://www.bkent.net/Doc/simple5.htm) (I didn't find this simple, but it is a nice resource -- ADK)
- [Normalization](https://medium.com/develbyte/normalization-c128a28aae00)

# Books
- [Wikibooks - SQL](https://en.wikibooks.org/wiki/Structured_Query_Language)
- [Wikibooks - PostgreSQL](https://en.wikibooks.org/wiki/PostgreSQL)
- [Wikibooks - Relational Database Design](https://en.wikibooks.org/wiki/Relational_Database_Design)
- [Use The Index, Luke!](https://use-the-index-luke.com/) : E-Book on Practical Indexes for Multiple SQL Dialects

# Documentation

## Postgres
- [PostgreSQL 12 Documentation](https://www.postgresql.org/docs/12/index.html)
- [PostgreSQL SQL Command Reference](https://www.postgresql.org/docs/12/sql-commands.html)

## AWS
- [AWS Documentation](https://docs.aws.amazon.com/)
- [AWS RDS User Guide](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html)
- [PostgreSQL on Amazon RDS](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_PostgreSQL.html)
- [AWS CLI Reference for RDS](https://docs.aws.amazon.com/cli/latest/reference/rds/)
  - This is useful if you want to use the command line to interact with AWS

# Tools
- [DBeaver](https://dbeaver.io/) (pick this or pgAdmin)
- [pgAdmin](https://www.pgadmin.org/)
- [AWS Tools for PowerShell](https://www.powershellgallery.com/packages/AWSPowerShell.NetCore/4.0.5.0):
  - We can interact with AWS using the command line instead of the web GUI.  Not required, but worth exploring!

# Tutorials

## Normalization
- [Example of a Step by Step Normalization](https://en.wikipedia.org/wiki/Database_normalization#Example_of_a_step_by_step_normalization)
- [Description of the Database Normalization Basics](https://docs.microsoft.com/en-us/office/troubleshoot/access/database-normalization-description)

## ANSI SQL
- [SQL Bolt](https://sqlbolt.com/)
- [SQL Teaching](https://www.sqlteaching.com/)
- [Learn SQL Coming From Excel](https://blog.treasuredata.com/blog/2014/12/05/learn-sql-by-calculating-customer-lifetime-value-part-1/)
- [Khan Academy](https://www.khanacademy.org/computing/computer-programming/sql) (uses SQLite, beware differing syntax!)

## PostgreSQL
- [postgresql.org Tutorial](https://www.postgresql.org/docs/12/tutorial-sql-intro.html)
- [Postgres Guide](http://www.postgresguide.com/) (check the sidebar to see if this contains the topic you want)
- [Working With Time in Postgres](http://www.craigkerstiens.com/2017/06/08/working-with-time-in-postgres/)

## AWS RDS
- Be careful to only select free tier options when using AWS!
- [Setting Up for Amazon RDS](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_SettingUp.html)
- [Creating Postgres RDS and Connecting Using pgAdmin](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_GettingStarted.CreatingConnecting.PostgreSQL.html)
