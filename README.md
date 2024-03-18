Run npm i to initialise the project.
You will need to create a db.js file to connect to postgres database. In the db.js file, copy and paste the following code:

import pg from "pg";

const db = new pg.Client({
  user: 'your_username',
  password: 'your_password',
  host: 'localhost',
  port: 5432, // default Postgres port
  database: 'your_database_name'
});

db.connect();

export default db;

Take a look at the databaseSetup.sql file and create the required database tables. Change anything that does not match your database settings and you are goog to go, enjoy~
