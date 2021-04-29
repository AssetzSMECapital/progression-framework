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
        - "Can perform simple SELECT statements and apply ORDER BY"
        - "Can describe the different types of JOIN and when to use them"
      exampleCriteria:
        - criteria: "Writes queries containing simple aggregate functions and GROUP BY"
          examples:
            - "SELECT SUM(...) FROM ..."
            - "SELECT COUNT(*) FROM ..."
        - criteria: "Applies simple pagination techniques"
          examples:
            - "LIMIT x OFFSET y"
    - level: 2
      criteria:
        - "Utilises database transactions to atomically execute multiple statements"
      exampleCriteria:
        - criteria: "Implements Common Table Expressions or temporary tables to break-down complex queries"
          examples:
            - "WITH something AS (...) SELECT * FROM something;"
        - criteria: "Writes queries containing complex aggregate functions"
          examples:
          - "SELECT SUM(...) FILTER (WHERE ...) FROM ..."
          - "SELECT COUNT(*) FILTER (WHERE ...) FROM ..."
        - criteria: "Applies appropriate pagination techniques"
          examples:
            - "LIMIT x OFFSET y"
            - "Keyset pagination e.g. WHERE id > x"
    - level: 3
      criteria:
        - "Utilises indexes to increase the performance of a query"
        - "Interprets the output from EXPLAIN ANALYSE to make actionable gains"
        - "Create database functions in appropriate circumstances"
        - "Understands how SECURITY DEFINER promotes additional privileges where appropriate"
        - "A good boy-scout and optimises slow queries"
        - "Optimises for CPU vs network bandwidth when accessing data"
    - level: 4
      criteria:
        - "Writes functions containing embedded transactions"
        - "Utilises WINDOW functions and RECURSIVE queries where appropriate"
      exampleCriteria: 
        - criteria: "Applies advanced pagination techniques"
          examples:
            - "Cursors"
            - "Clustered TID scan"
- name: "Designing data models"
  title: "🗂️ Designing data models"
  content:
    - level: 1
      criteria:
        - "Can create a simple, standalone database table with a primary key"
        - "Ensures any database fields containing personal information are registered with the InfoSec team"
        - "Usage of enum types where value can only be of limited choices"
      exampleCriteria:
        - criteria: "Follows Assetz conventions and best practices"
          examples:
          - "Timestamp columns are suffixed with `_at` and contain timezone"
          - "Boolean columns are prefixed with `is_`"
          - "Table names are non-plural"
        - criteria: "Understands and uses basic data types"
          examples:
          - "numeric(38,20) for monetary amounts"
          - "text for all string types"
          - "bigint primary keys for large volumes of data"
    - level: 2
      criteria:
        - "Creates tables containing multiple relationships"
        - "Applies unique constraints where necessary - INDEXES?"
        - "Utilises simple indexes to optimise data access"
        - "Create a database view in appropriate circumstances"
      exampleCriteria:
        - criteria: "Understands and uses advanced data types"
          examples:
            - "`JSONB`"
            - "Network address types"
            - "`ARRAY`"
            - "`UUID`"
        - criteria: "Implements constraints to ensure data integrity"
          examples:
            - "`CONSTRAINT prevent_negative CHECK (amount >= 0)`"
    - level: 3
      criteria:
        - "Create a materialized view in appropriate circumstances and understands the drawbacks of refreshing an entire dataset"
      exampleCriteria:
        - criteria: "Usage of table triggers where appropriate"
          examples:
            - "BEFORE DELETE ON ... EXECUTE ..."
    - level: 4
      criteria:
        - "Understands and creates custom data types"
        - "Monitor table and index sizes pro-actively"
        - "Can implement data partitioning to increase efficiency"
        - "Applies strategic thinking for designing tables to handle big data"
        - "Reduce data duplication by taking advantage of table inheritance"
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
      - "Utilises cascading role permissions"
  - level: 3
    criteria:
      - "Safely applies table and row level locks and understands impact"
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
      - "Safely applies usage of advisory locks"
      - "Implements strategies to minimise table bloat"
      - "Understands transaction XID wraparound"
    exampleCriteria:
      - criteria: "Implements different types of replication"
        examples:
          - "Streaming replication"
          - "Logical replication"
- name: "redis"
  title: "⚡Redis"
  content:
  - level: 1
    criteria:
      - "TODO: something here?"
  - level: 2
    criteria:
      - "Connect to a Redis instance"
      - "Fetch key(s) from a Redis datastore"
      - "Set or update keys in a Redis datastore"
      - "Uses appropriate TTLs when setting keys"
  - level: 3
    criteria:
      - "TODO: something here?"
      
- name: "TODO / Questions"
  title: "TODO / Questions"
  content:
  - level: 1
    criteria:
    - "Aimed at using databases, not administrating databases. Level 4 includes some more admin'y things engineers still need to consider like table bloat"
    - "Leaving out foreign data wrappers - doesn't feel aligned with separation of concerns?"
    - "Tried to align with our architecture principles - avoid logic in database etc"
---

Become a master of databases!

### Technologies 

- PostgreSQL
- Redis
- Amazon RDS
- Amazon Elasticache


