---
title: "Developer Guide"
date: 2025-09-03
---
### Setting Up the Development Environment

Clone this repository

Install and run PostgreSQL

$ createdb freshkeepuh # create a database

Create a .env file from the sample.env. Set the DATABASE_URL

$ npm install # install dependencies

$ npx prisma migrate dev # create the database schema

$ npx prisma db seed # demo data

$ npm run dev # start the local development server