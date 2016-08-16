# _still in progress ..._

# haskell-elm-todo-app

Todo app build with [Servant](http://haskell-servant.github.io/) ([Haskell](https://www.haskell.org/)) on server-side and [Elm](http://elm-lang.org/) on client-side

## Instructions

### Build and run server-side app


``` shell
stack build
stack exec haskell-elm-todo-app
```

### DB queries

by using [httpie](https://github.com/jkbrzt/httpie):

``` shell
# insert an user
http POST localhost:3000/user/add name=Alice age:=42 -j

# get an user
http localhost:3000/user/get/Alice

# get all users
http localhost:3000/users/

```

## Acknowledge

### Haskell / Servant stuff

- Haskell + Persistent: [http://www.yesodweb.com/book/persistent](http://www.yesodweb.com/book/persistent)

- "(Querying an existing database)[https://www.schoolofhaskell.com/school/advanced-haskell/persistent-in-detail/existing-database]"

- Example Servant + Persistent: [https://github.com/haskell-servant/example-servant-persistent/](https://github.com/haskell-servant/example-servant-persistent/)

- Example Servant + Persistent by Matt Parsons: [https://github.com/parsonsmatt/servant-persistent](https://github.com/parsonsmatt/servant-persistent)

- Example Servant + Elm: [https://github.com/haskell-servant/example-servant-elm](https://github.com/haskell-servant/example-servant-elm)

- "Todobackend" with Servant: [https://github.com/jhedev/todobackend-haskell/tree/master/todobackend-servant](https://github.com/jhedev/todobackend-haskell/tree/master/todobackend-servant)

- Album Haskell Elm app: [https://github.com/rundis/albums](https://github.com/rundis/albums)
