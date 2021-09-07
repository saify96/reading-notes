# Relationships between types

- The @connection directive enables you to specify relationships between @model types.
  - one-to-one
  - one-to-many
  - many-to-one
  - many-to-many

- Relationships between types are specified by annotating fields on an @model object type with the @connection directive.

- The fields argument can be provided and indicates which fields can be queried by to get connected objects.
- The keyName argument can optionally be used to specify the name of secondary index (an index that was set up using @key) that should be queried from the other type in the relationship.

- A Has One @connection can only reference the primary index of a model (ie. it cannot specify a "keyName" as described below in the Has Many section).

- A one-to-many connection needs an @key that allows comments to be queried by the postID and the connection uses this key to get all comments whose postID is the id of the post was called on. After it's transformed, you can create comments and query the connected Post as follows:

- You can make a connection bi-directional by adding a many-to-one connection to types that already have a one-to-many connection.

- The default number of nested objects is 100. You can override this behavior by setting the limit argument.
  
- In order to keep connection queries fast and efficient, the GraphQL transform manages global secondary indexes (GSIs) on the generated tables on your behalf when using @connection.
  