# Instructions + Notes
You have been asked to work on a system for tracking directors, movies and actors.

Complete the project using the PHP scripting language.  You may choose to use any framework you like, or none at all.  Demonstrate your understanding of OOP and MVC, where possible.

The design/UI of the project is not important, although any CSS or HTML included should be valid and well-structured. 

You may choose to use any JS framework or none at all. You may choose to use any CSS preprocessor and/or framework or none at all. 

## Submitting
Fork this repository and submit a link to the repo with the completed exercise.

# Database Schema
Design a MySQL or PostgresSQL schema that allows tracking the following information and relationships:

## Entities
### Movies
* Title
* Rating
* URL for ‘cover art'
* Date of release

###Directors
* Name 
* Country of birth
* URL for photo
* Birthday
* email address
* password

### Actors
* Name
* Country of birth
* URL for photo
* Birthday
* Phone Number
* Home Address

### Relationships
* Each movie will have exactly one director.  
* Each movie may have one or more actors.

# Web Interface
## Anonymous User
Develop a web interface that allows an anonymous visitor to browse a list movies, directors or actors (pagination is not necessary).

A user should be able to click any entity and view a page with that entity’s details, including links to all related entities.

Provide a text input that allows users to search movies, directors, or actors by name/title.
 
## Authorized User (Director)
Provide a login form that directors can use to log in to the site using their email and password.  If a director is currently logged in, when they are viewing the page of any actor that they have worked with on a movie, they can see the phone number and home address of that actor.

# REST API
## Authentication
Access to the REST API should be restricted to Directors with a valid email and password. The type of authentication required is at your discretion.

## Querying Records
Provide a REST API that allows querying of any entity and returning the results as JSON. Any group of entities should be searchable by name/title or by relationship (for example, allow filtering Actors by Movie ID or Movies by Director ID). 

## Editing Records
Allow creating or editing of Movies via the API. Only allow editing movies if their release date is null or in the future 

Contacts and Actors can not be created nor edited via the REST API.
