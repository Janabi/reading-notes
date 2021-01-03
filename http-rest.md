# HTTP and REST

## Review, Research, and Discussion

### Define three related pieces of data in a possible application. An example of a store application might be Product, Category and Department. Describe the constraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department.

We can say a social media app where you can register, post any type of data, and add friends as much as you can.

### What is the advantage of an ORM, like Mongoose?
- It is much easier to update the document of the data rather than any other database language.
- It has a lot of built-in validation methods which make it easy to read with a little bunch of codes.
- Mongoose provides optional pre and post in order to save operations for data models.


### How does the repository pattern compare with an ORM?
For many reasons, you must go for _repository pattern_, including:
- Repository pattern mainly handling business/domain objects.
- It is abstract the persistent access, whatever how the storage looks like.

### When making a repository/facade, what flexibility do you gain?
It uses a facade methodology to reduces the communication between the complex subsystem and its clients.

### Name 3 cloud based NoSQL Databases
- MongoDB.
- Amazon Web Services.
- Google Firebase.

## Document the following Vocabulary Terms

- **lifecycle -** which might say as a "Program Development Life Cycle", a process that contains five stages where every computer prgram undergoes. These satges are analyzing, designing, coding, debugging, and testing to implement and maintain the quality of this software.

- **Collection -** which what exactly the MongoDB has, a set of collections as documents, graphs and pair of ky-value representing a bunch of records as an inserting data.

- **the “Repository” design pattern -** a representation where you can keep all of the operations of your database in one local business entity.

- **mongoose middleware -** a function that could be passed to control the execution of asynchronous functions.

- **Object Relation Mapping (ORM) -** is a programming idea of converting data between incompatible type systems using OOP.