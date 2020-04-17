# Week 2 - SQL
## Concepts
- SQL: ANSI SQL, SQL Sublanguages, SELECT clauses
- RDBMS: Relational DataBase Management System, SQL Dialects
- Relational Databases: Relations, Records, Keys, Constraints
- Normalization: 1-3 Normal Forms, Candidate/Composite/Foreign/Primary Keys
- Multiplicity & Joins
- Database Transactions: [ACID Properties](https://en.wikipedia.org/wiki/ACID), [Isolation Levels](https://en.wikipedia.org/wiki/Isolation_(database_systems)#Isolation_levels)

## Tools 
- AWS RDS: RDBMS hosted and managed by Amazon, on their servers
- PostgreSQL: Open Source RDBMS
- DBeaver: Utility for working with databases

## SQL Language
- Sublanguages:
  - DQL: SELECT
  - DML: INSERT, UPDATE, DELETE
  - DDL: CREATE, ALTER, DROP
  - DCL: GRANT, REVOKE
  - TCL: SAVEPOINT, COMMIT, ROLLBACK
- SELECT clauses:
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
  - json (optional)

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

# Books

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
  - We can interact with AWS using the command line instead of the web GUI.  Not required, but worth looking into!

# Tutorials

## ANSI SQL
- [SQL Bolt](https://sqlbolt.com/)

## PostgreSQL
- [postgresql.org Tutorial](https://www.postgresql.org/docs/12/tutorial-sql-intro.html)

## AWS RDS
- Be careful to only select free tier options when using AWS!
- [Setting Up for Amazon RDS](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_SettingUp.html)
- [Creating Postgres RDS and Connecting Using pgAdmin](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_GettingStarted.CreatingConnecting.PostgreSQL.html)
