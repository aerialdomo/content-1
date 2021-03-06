# Add Default Value
author: SebaRaba

levels:

  - beginner

  - basic

  - medium

  - advanced

type: normal

category: must-know

inAlgoPool: false

links:

  - '[More on ADD DEFAULT](https://www.w3schools.com/sql/sql_default.asp)'

tags:
  - workout

---
## Content

In *MS Acccess* and *SQL Servers* we can use the `ALTER TABLE` statement to set default values for desired columns:
```
ALTER TABLE table_name
ALTER COLUMN column_name
SET DEFAULT value;
```

In *MySQL* the syntax is a little bit different:
```
ALTER TABLE table_name
ALTER column_name
SET DEFAULT value;
```

And if we are using *Oracle*:
```
ALTER TABLE table_name
MODIFY column_name
DEFAULT value;
```

---
## Practice

Consider the "region" table. We want to set default value 1 to all entries under "region_id" column:
```
id | region_id |      name      
===+===========+===============
 1 |         1 | generation-i
 2 |         2 | generation-ii
 3 |         3 | generation-iii
 4 |         4 | generation-iv
 5 |         5 | generation-v
 6 |         6 | generation-vi
(6 rows)

??? region
ALTER ??? ???
??? 1;
```

* ALTER TABLE
* COLUMN
* region_id
* SET DEFAULT
* region
* UPDATE
* ALTER COLUMN

---
## Revision

We would like to set the default value "ruby" to all entries under column "name" in the "version" table:
```
id | version_group_id |      name      
===+==================+===============
 1 |                1 | red
 2 |                1 | blue
 3 |                2 | yellow
 4 |                3 | gold
 5 |                3 | silver
 6 |                4 | crystal
 7 |                5 | ruby
 8 |                5 | sapphire
...

    ???
```

* ALTER TABLE version ALTER COLUMN name SET DEFAULT 'ruby';
* ALTER TABLE region ALTER COLUMN name SET DEFAULT 'ruby';
* ALTER TABLE version ALTER name SET DEFAULT 'ruby';
