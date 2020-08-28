# go-gqlgen-Server

Go Server using graphQL to querie mocked database. 

![serverRunning1](https://i.imgur.com/JTAcG7f.gif)

![serverRunning2](https://i.imgur.com/wRihO6Z.gif)

## Schema

```
type Mutation {
  createTodo(input: NewTodo!): Todo!
}

input NewTodo {
  text: String!
  userId: String!
}

type Query {
  todos: [Todo!]!
}

type Todo {
  id: ID!
  text: String!
  done: Boolean!
  user: User!
}

type User {
  id: ID!
  name: String!
}
```

### Reference:
https://gqlgen.com/getting-started/
