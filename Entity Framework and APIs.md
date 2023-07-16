## Entity Framework Core 
Entity Framework Core (EF Core) is a lightweight, extensible, open-source, and cross-platform version of the Entity Framework (EF) data access technology. It provides an object-relational mapper (ORM) that enables developers to work with databases using .NET objects and LINQ (Language Integrated Query).


## The model:


In Entity Framework Core (EF Core), the model represents the structure of the data that you want to persist in the database. It consists of entity classes and a context object that represents a session with the database.

Entity classes, also known as domain classes or POCO (Plain Old CLR Objects) classes, define the objects and their properties that will be mapped to database tables. Each entity class typically corresponds to a table in the database, and the properties of the class represent the columns of that table.
## Querying:
Instances of your entity classes are retrieved from the database using Language Integrated Query (LINQ) . 

## Saving data:

Data is created, deleted, and modified in the database using instances of your entity classes.  

## ASP.NET MVC:

ASP.NET MVC (Model-View-Controller) is a web application framework developed by Microsoft that follows the MVC architectural pattern. It provides a structured approach to building dynamic and scalable web applications.

## Overview of ASP.NET Core MVC:
ASP.NET Core MVC is designed to be cross-platform, modular, and high-performance. It allows you to build modern web applications that can run on Windows, macOS, or Linux. It also integrates seamlessly with other ASP.NET Core features, such as authentication, authorization, and caching, to provide a complete web development framework.

## Razor Pages 

The Razor Pages framework is lightweight and very flexible. It provides the developer with full control over rendered HTML. Razor Pages is the recommended framework for cross-platform server-side HTML generation.


## Data Seeding

Database seeding is populating a database with an initial set of data. It's common to load seed data such as initial user accounts or dummy data upon initial setup of an application.

There are several ways this can be accomplished in EF Core:

-Model seed data

-Manual migration customization

-Custom initialization logic -

-Building Web APIs with ASP.NET -

-Web API : Web API is an application programming interface (API) that is used to enable communication or interaction with software components with each other. ASP.NET Web API is a framework that makes it easy to build HTTP Service that reaches a broad range of clients, including browsers and mobile devices. Using ASP.NET, web API can enable communicating by different devices from the same database.


## Add User Secrets to .NET Core

### User secrets : is a secure way of storing private user information such as API keys, client secrets, and connection strings.

-Never store passwords or other sensitive data in source code.
-Production secrets shouldn't be used for development or test. Secrets shouldn't be deployed with the app  

### Environment variables : Environment variables are used to avoid storage of app secrets in code or in local configuration files. Environment variables override configuration values for all previously specified configuration sources.

### Secret Manager: The Secret Manager tool stores sensitive data during the development of an ASP.NET Core project. a piece of sensitive data is an app secret.
