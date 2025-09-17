---
title: "Developer Guide"
date: 2025-09-06
---
## Quick Start
* Install [PostgreSQL](https://www.postgresql.org/download/)
  * Make your password simple - no special characters, otherwise you will need to [Percent Encode](https://developer.mozilla.org/en-US/docs/Glossary/Percent-encoding) (otherwise known as URL Encode) the password.
* Install [Node.js and NPM](https://nodejs.org/en/download/)
* Install [git](https://git-scm.com/downloads)
* Install your favorite Integrated Development Environment
  * [VS Code](https://code.visualstudio.com/download)
  * [IntelliJ IDEA](https://www.jetbrains.com/idea/download)
* Clone the FreshKeep Repository
  * `git clone https://github.com/freshkeepuh/freshkeep.git`
* Install the dependencies
  * `npm install`
  * Update npm if necessary
* Create the Database
  * `createdb freshkeepuh`
  * On Windows, you should use pgAdmin to create the database.
* Create .env file using sample.env as template
  * Set DATABASE_URL to "postgresql://postgres:{password}@localhost:5432/freshkeepuh"
    * Replace '{password}' with the postgres root password
  * Set NEXTAUTH_SECRET to Long (64 characters or more) Random String
    * For example, you can generate one using: `openssl rand -base64 64`
* Create the Database Schema
  * `npx prisma migrate dev` or `npm run migrate`
* Seed the Database Schema
  * `npx prisma db seed` or `npm run seed`
* Start the Node.js Server in Development mode
  * `npm run dev`
* Open your web browser to the [Home Page](http://localhost:3000)

### Testing
* Install Playwright with Dependencies (only once)
  * `npx playwright install --with-deps`
* Run Playwright
  * `npx playwright test` or `npm run test`

## Draft Entity Relationship Diagram

![ERD Diagram](images/devGuide/prisma-uml.png)

## Draft Tech Stack Flowchart

![Tech Stack Flowchart](images/devGuide/draft-tech-stack-flow-chart.png)

## Draft Page Flowchart
![Page Flow Chart](images/devGuide/draft-page-flow-chart.png)

