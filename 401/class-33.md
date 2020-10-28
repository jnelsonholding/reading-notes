### Class 33 Reading Notes

## GraphQL Connections

GraphQL has built in syntax for creating connections between models. It can handle one-to-one, one-to-many, and many-to-one relationships. It actually doesn't have direct coverage for many-to-many, but that can of course be created with a join table. In all cases, the field needing the connection is annotated with `@connection`.

One-to-one relationships are fairly simple. The field type (usually String) is instead the name of the model to connect to (eg. Address if it's the Address model). And that's followed by `@connection`. GraphQL infers that the link should be to the `id` field of the table you are connecting to.

```
type Company @model {
  id: ID!
  name: String
  address: Address @connection
}

type Team @model {
  id: ID!
  street: String
  city: String
  state: String
  zip: String
}
```

One-to-many adds a bit more complexity. For one, the reference to the field type needs to be surrounded by square brackets, indicating a list. And the many relation needs a key for the one relation to relate to. Also the many relation will need a field to relate to the many relation's IDs.

```
type Design @model {
  id: ID!
  designer: String!
  colors: [Color] @connection(keyName: "byDesign", fields: ["id"])
}

type Color @model
  @key(name: "byDesign", fields: ["designID", "name"]) {
  id: ID!
  designID: ID!
  name: String!
}
```

The many-to-one relationship can now be added easily by adding a field to the many side. It just needs to reference the ID value of the one side again, but conveniently that's already in the many table from the previous connection.

```
type Design @model {
  id: ID!
  designer: String!
  colors: [Color] @connection(keyName: "byDesign", fields: ["id"])
}

type Color @model
  @key(name: "byDesign", fields: ["designID", "name"]) {
  id: ID!
  designID: ID!
  name: String!
  design: Design @connection(fields: ["designID"])
}
```

[Return to table of contents](../README.md)
