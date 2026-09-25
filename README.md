### Project Setup

## Creating database 

CREATE DATABASE LibraryDB 

## Creating Books table

CREATE TABLE books(

id SERIAL PRIMARY KEY,

title VARCHAR(50),

author_id INTEGER REFERENCE authors(id)

genres TEXT[],

published_year INTEGER,

available BOOLEAN

)

## Creating authors table

CREATE TABLE patrons(

id SERIAL PRIMARY KEY,

name VARCHAR(50),

email VARCHAR(50),

borrowed_books INTEGER[]

)

## Creating patrons table

CREATE TABLE patrons(

id SERIAL PRIMARY KEY,

name VARCHAR(50),

email VARCHAR(50),

borrowed_books INTEGER[]

)




