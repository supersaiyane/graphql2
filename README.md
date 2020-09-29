# GraphQL

# Node.js/Express CRUD backend using GraphQL and JSON-Server

1. Initialize project

```sh
npm init
```

2. install initial dependencies

```sh
npm install graphql cors express express-graphql nodemon json-server axios --save
```

3. add below line in the Scripts tags in package.json to run program

```sh
"dev:server": "nodemon server.js"
"json:server": "json-server --watch data.json"
```

4. To Run the dev server

```sh
npm run dev:server
```

5. To Run the Json server

```sh
npm run json:server
```

6. To check if Json-server running good

```sh
localhost:3000/customers
```

7. Queries

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

#sample3
mutation{
  addCustomer(name:"Gurpreet",email:"gurpreet.singh@gmail.com",age:30){
    id,
    name,
    email
  }
  
  deleteCustomer(id:"3"){
    id
  }
  
  editCustomer(id:"2",age:60){
    id,
    age
  }
}