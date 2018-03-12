# Graph QL Demo

## Set mongodb uri
1. Create .env file
2. Add following line
```
DB_URI=<mongodb uri>
```

## Install
```
$ npm install
```

## Start Server
```
$ npm start
```

## Run on Browser

- Go to `localhost:4000/graphiql`
- Run following queries / mutations

Get all authors
```
{
    authors {
        id
        name
        age
        books
    }
}
```

Filter authors by age
```
{
    authors(age) {
        id
        name
        age
        books
    }
}
```

Get Author by Id
```
{
    author(id) {
        id
        name
        age
        books
    }
}
```

Add author
```
mutation {
    addAuthor(name, age, books) {
        id
        name
        age
        books
    }
}
```

Delete Author
```
mutation {
  deleteAuthor(id) {
    id
    name
    age
    books
  }
}
```

Update Author
```
mutation {
    updateAuthor(id, name) {
        id
        name
        age
        books
    }
}
```