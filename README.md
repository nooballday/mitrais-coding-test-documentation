# Mitrais Coding Test Documentation

This documentation provides step by step process to running the **SIMPLE REGISTER APP** . 
It consist of 3 main entity :

 - Web App (Vue.js)
 - REST API (Express)
 - Database (Postgres)

**NOTE** that i am developing it with **Linux** based OS (Ubuntu 18.04). To run this app please make sure that these softwares are installed in your computer :

- Nodejs version 8+
- Postgresql
- npm / yarn

If requirements are met please continue to step 1 :

## Step 1. Database

**Source :** https://github.com/nooballday/mitrais-coding-test-db.git
Pull the source and run the query inside `structure.sql` into your current database or you can restore the whole database using `psql`with `dump.sql` make sure if you create your own database, the name of the database needs to be updated in **REST Api** server.

## Step 2. REST API

**Source :** https://github.com/nooballday/mitrais-coding-test-rest-api.git

- Pull the source with `git clone  https://github.com/nooballday/mitrais-coding-test-rest-api.git`
- Move inside the directory `cd mitrais-coding-test-rest-api`
- Install the required dependencies using `yarn install` or `npm install`
- Edit `server.config.json` inside `config` directory, and please fill your database config
- Run test with `yarn test` or `npm run test`
- Execute `yarn serve` to run development mode or `yarn build && yarn serve:production` to run in production

## Step 3. WebApp
**Source :** https://github.com/nooballday/mitrais-coding-test-webapp.git

- Pull the source with `git clone https://github.com/nooballday/mitrais-coding-test-webapp.git`
- move inside directory `cd mitrais-coding-test-webapp`
- Edit environment variables and provide your **REST Api** ip address or hostname inside `.env` file
- Install the required dependencies using `yarn install` or `npm install`
- start the server in development mode using `yarn serve` or `npm run serve` 
