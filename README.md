# File Schema Detector
Analyzes a CSV file and generates database table schema, all within the browser

This application uses [PapaParse](http://papaparse.com/) to parse CSV files (including huge ones)
within the browser. It analyzes each field to suggest the best database field type, max length,
and whether or not there are any `null` values. From there, you can rename fields, ignore them,
override field types/lengths, etc. and generate database table creation sql for MySQL, MariaDB,
Postres, Oracle, or SQLite3.

## Development
Install dependencies using `npm install`, then run a development server using `npm start`.
To deploy the application use `npm run deploy`.

This application uses [PapaParse](http://papaparse.com/) for CSV parsing and
[Knex.js](http://knexjs.org/) for SQL query building.
