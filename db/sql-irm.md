# Immutable Relational Mapper

A simple relational database mapper for immutable objects.

## Concepts

- Less to learn.
- Less conventions: to avoid changing original code to conform to this library.
- Declarative and elegant representation: fluent, immutable, and `null`-eliminated.
- Simple features.
- Users can customize its various behaviors and it adapts to respective situations.

## Features

- Associates a name of an *immutable class* and a name of a *table*.
- Associates a property of an immutable class and a column of a table.
- Converts a record into an immutable instance automatically, and conversely.
- Provides some simple queries and commands without SQL.
- Takes SQL statemens from your resources automatically.

Additionally, users can specify how to realize these features if desired.

### Dao[T, K] class

Let `Dao[T, K]` is a DAO class where `T` is an *entity* type for this DAO, `K` is the type of the entity's *primary key*.

`Dao[T, K]` has following members (method and properties):

- `insert(entity: T): Long` or `insert(entity: T): T`
- `insertWithPrimaryKey(entity: T): Long`
- `find(key: K): T?`
- `delete(key: K): Int`
