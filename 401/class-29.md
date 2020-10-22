### Class 29 Reading Notes

## Android Data Persistence Using Room

If you need database storage on an Android app, then there is a SQLite database waiting for you. The layer that allows you to access it is called Room. You can think of it as your app's "room" on the shared Android database.

Room is made of 3 components: Database, Entity, and DAO. Database is the main access point to the data. Entity is a table in the database. And DAO is the data access object that contains your access methods.

Each Entity needs to have a primary key, which is defined by annotating the chosen field with `@PrimaryKey`. The table created for the Entity will match the class name by default. But it's possible to change it by passing a `tableName` parameter to the `@Entity` annotation.

An Entity can also have embedded subclasses. This is a handy tool for database normalization, which conveniently also helps keep to object oriented tenants.

Joining tables can also be done in One to One, One to Many, and Many to Many relationships. Each of these is actually handled through a similar format. No matter which type of relation, you'll need to create a class representing a join table.

Querying the database is handled through the DAO. various CRUD operations can be defined by creating interfaces. In the interface, each operation is labelled with an annotation indicating its type: `@Insert`, `@Update`, `@Delete`, and `@Query`.

[Return to table of contents](../README.md)
