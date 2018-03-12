# Graph QL Demo

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


