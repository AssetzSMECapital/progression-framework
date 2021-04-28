---
path: "/zBadge/databases"
title: "💾 Databases Engineering Framework"
sidebarTitle: "💾 Databases"
sidebarGroup: "Engineering Badges"
yaml: true 
levels: 4 
homepage: true 
topics:
- name: "Writing SQL"
  title: "✏️ Writing SQL"
  content:
    - level: 1 
      criteria:
        - "Can perform simple SELECT statements"
        - "Can describe the different types of JOIN"
      exampleCriteria:
        - criteria: "Writes queries containing simple aggregate functions"
          examples:
            - "SELECT SUM(...) FROM ..."
            - "SELECT COUNT(*) FROM ..."
    - level: 2
      criteria:
        - "Utilises database transactions to atomically execute multiple statements"
      exampleCriteria:
        - criteria: "Implements Common Table Expressions to break-down complex queries"
          examples:
            - "WITH something AS (...) SELECT * FROM something;"
        - criteria: "Writes queries containing complex aggregate functions"
          examples:
          - "SELECT SUM(...) FILTER (WHERE ...) FROM ..."
          - "SELECT COUNT(*) FILTER (WHERE ...) FROM ..."
    - level: 3
      criteria:
        - "Utilises indexes to increase the performance of a query"
        - "Interprets the output from EXPLAIN ANALYSE to make actionable gains"
        - "Understands how SECURITY DEFINER promotes additional privileges where appropriate"
        - "A good boy-scout and optimises slow queries"
    - level: 4
      criteria:
        - "TODO: Feels like something should go here?"
- name: "Designing data models"
  title: "🗂️ Designing data models"
  content:
    - level: 1
      criteria:
        - "Can create a simple, standalone database table"
        - "Ensures any database fields containing personal information are registered with the InfoSec team"
        - "Usage of enum types where value can only be of limited choices"
      exampleCriteria:
        - criteria: "Follows Assetz conventions and best practices"
          examples:
          - "Timestamp columns are suffixed with `_at` and contain timezone"
          - "Boolean columns are prefixed with `is_`"
          - "Table names are non-plural"
        - criteria: "Understands and uses the correct data types"
          examples:
          - "numeric(38,20) for monetary amounts"
          - "text for all string types"
          - "bigint primary keys for large volumes of data"
    - level: 2
      criteria:
        - "Creates tables containing multiple relationships"
        - "Applies unique constraints where necessary"
      exampleCriteria:
        - criteria: "Implements constraints to ensure data integrity"
          examples:
            - "`CONSTRAINT prevent_negative CHECK (amount >= 0)`"
    - level: 3
      exampleCriteria:
        - criteria: "Usage of table triggers where appropriate"
          examples:
            - "BEFORE DELETE ON ... EXECUTE ..."
    - level: 4
      criteria:
        - "Can implement data partitioning to increase efficiency"
        - "Applies strategic thinking for designing tables to handle big data"
- name: "mastery"
  title: "🛠️ Mastery"
  content:
  - level: 1
    exampleCriteria:
      - criteria: "Applies the minimum required privileges for an application"
        examples:
          - "GRANT SELECT, UPDATE ON ..."
          - "REVOKE DELETE ON ..."
  - level: 2
    criteria:
      - "A good boy-scout and safely removes un-used database fields without a negative impact"
  - level: 3
    criteria:
      - "Safely applies usage of advisory locks"
    exampleCriteria:
      - criteria: "Identifies running queries that are causing a negative impact"
        examples:
          - "Are queries waiting for a lock to be released?"
          - "Is the query paging to disc and causing high I/O usage?"
      - criteria: "Uses appropriate database connection management"
        examples:
          - "Connection pooling for APIs"
          - "Minimum required connections for a service or application"
  - level: 4
    criteria:
      - "Safely applies table and row level locks"
- name: "TODO / Questions"
  title: "TODO / Questions"
  content:
  - level: 1
    criteria:
    - "Aimed at using databases, not administrating databases. Is this the right approach? Or could lvl 4 be for more admin'y things engineers still need to consider like table bloat"
    - "Database functions? Want to discourage - but occasionally they are acceptable?"
    - "What about views, and materialized views?"
    - "Connection management"
---

Become a master of the database!

### Technologies 

- PostgreSQL

### The aim of these frameworks are to

- Help people understand how to progress in their work
- Help us evaluate and pay people fairly and consistently
- Help people understand the skills and behaviours we value

The framework is a compass, not a GPS.

It's meant to be helpful. It's not meant to be a rating system for humans, free from edge cases.

### How does it work?

The framework covers all the things we’re looking for from engineers at Assetz. We’re interested in these five elements:

- Mastery - Your Assetz knowledge and technical capability
- Impact - The size, scope and value of what you deliver
- Influence - How you change the world around you for the better
- Comms & Feedback - How you interact with others
- Leadership - How people around you become better and more impactful

We sort them into four levels, and we try to give specific examples of behaviours we expect for each. Each of those levels has a fairly wide salary range associated with it, and within each level you can progress in sub-levels, labelled A–D. So even if you’re at level 3 for a couple of years, you’ll still be able to see that you’re moving forward. Basically, the more behaviours you show from your level, the more you’ll progress.

Your manager will work with you on this. None of it will happen mysteriously behind closed doors. You’ll agree what level of progression you’re going for and what you need to improve on with your manager. It should be clear how you’re doing relative to that at all times.

### Things to keep in mind

- There are many different ways to progress and be valuable to Assetz as you grow, including deep technical knowledge and ability, technical leadership and people management. All are equally valuable paths in Assetz’s engineering team.
- The framework represents a career’s worth of progression, people shouldn’t expect to fly up it in 18 months!
- Engineering progression isn’t an exact science and there will always be some ambiguity.
- This isn’t a checklist – it’s possible to progress up a level without showing all the behaviours in that level.
- You can find some more information in these links. If that doesn't answer most of your questions, please ask your manager.

### Give us your feedback!

This is only the first version of our framework and we really want your feedback.

We're particularly keen to add as many examples to the behaviours as possible, to further clarify them.

