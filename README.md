# GraphQL

# Node.js/Express CRUD backend using GraphQL and JSON-Server

1. Initialize project

```sh
npm init
```

2. install initial dependencies

```sh
npm install graphql cors express express-graphql nodemon --save
```

3. add below line in the Scripts tags in package.json to run program

```sh
"dev:server": "nodemon server.js"
```

4. To Run the dev server

```sh
npm run dev:server
```

5. Queries

```sh
#sample 1
{
  customer(id:"1"){
    name,
    email,
    age
  }
}


#sample2
{
  customer(id:"4"){
    name,
    email,
    age
  }
}
```