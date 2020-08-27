### Class 14 Reading Notes

## Database Normalization

Database normalization is the practice of separating tables of data by their purpose. This has multiple benefits. For one it helps to avoid duplicating data since it will be stored in one table and referenced by others. It also can make finding data easier since it should limit data to single sources of truth. And it allows tables to all connect through identifiers. It puts the 'relational' in relational databases.

There are three steps to database normalization called the first, second, and third normal forms. Each is dependent on the previous being completed.

The first normal form is for each column in a table to have atomic values. Meaning that the table should not have repeating columns to store similar data. Instead those should be moved to enother table and related through IDs.

The second normal form assumes the first is true already. Additionally, it requires that all non-key columns are dependent on the table's primary key. If they are not, then they should be moved into another table. One technique to transfer data like this is to create an intersection table, a table with only keys used to relate data from separate sources.

The third form then specifies to make sure all columns rely directly on the primary key and are not transitive through other columns. At some point this becomes more about best practice than actual efficiency. But if there are going to be duplicate references, just move those to another table and relate them through keys.

[Return to table of contents](../README.md)
