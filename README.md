# graphql-with-mongodb
API of graphql with mongodb

## Introduction 
This is a server for CRUD operations using GraphQL and MongoDB.

## Getting started
 1. Copy or clone the project from https://github.com/dev-expert/graphql-with-mongodb.git
 2. Goto the folder graphql-with-mongodb
 3. Run npm install for dependencies
 4. Create database into the mongodb: 
        a. Database name: test
        b. collection name : users
        c. fields : id : string
                    name : string
                    email : string
 5. Run npm start to see the example on port : http://localhost:4000/graphql


 # Parameters for CURD operations:

 ## Create User mutation like:

 mutation {
  addUser(id: "1", name: "Sam", email: "sam@sam.com") {
    id
    name
    email
  }
}

 ## Edit User mutation like:

 mutation {
  editUser(id: "1", name: "Sam", email: "sam@ymail.com") {
    id
    name
    email
  }
}

 ## Delete User mutation like:

 mutation {
  deleteUser(id: "1", name: "Sam", email: "sam@sam.com") {
    id
    name
    email
  }
}

 ## Get all users query like:

 query {
  users {
    id
    name
    email
  }
}

 ## Get a specific user query like:

 query {
  user(id: "1"){
    id
    name
    email
  }
}


## Happy coding......