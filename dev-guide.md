---
title: "Developer Guide"
date: 2025-09-03
---
### Quick Start
* Install [PostreSQL](https://www.postgresql.org/download/)
* Install [Node.js and NPM](https://nodejs.org/en/download/)
* Clone the FreshKeep Repository
  * `git clone https://github.com/freshkeepuh/freshkeep.git`
* Install the dependencies
  * `npm install`
* Create the Database
  * `createdb freshkeepuh`
* Create .env file using sample.env as template
  * Set DATABASEURL to "postgresql://postgre:{password}@localhost:5432/mydb?schema=freshkeepuh"
    * Replace '{password}' with the postgre root password
  * Set NEXTAUTH_SECRET to Random String
* Create the Database Schema and Seed the demo data
  * `npx prisma migrate dev`
* Build the FreshKeep application
  * `npm run build`
* Start the Node.js Server in Development mode
  * `npm run dev`
* Open your web browser to the [Home Page](http://localhost:3000)

## Draft Tech Stack Flowchart

<img src="images/draft-tech-stack-flow-chart.png" alt="Tech Stack Flowchart">

## Draft Page Flowchart
<img src="images/draft-page-flow-chart.png" alt="Page Flow Chart">

