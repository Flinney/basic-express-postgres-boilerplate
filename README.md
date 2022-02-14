# basic-express-postgres-boilerplate

Quick boiler plate setup for an express server using knex and a cloud-based postgres db.

## Prerequisites

* A cloud based postgres db (i.e. [ElephantSQL](https://www.elephantsql.com/))

## Setup

1. `npm install`

1. Run `cp .env.sample .env` and insert your db's full url in the `DATABASE_URL` variable within the newly created `.env` file.

1. `npm run dev` will now start the server in development mode (<http://localhost:5000/> by default) and a simple `GET` request should return a `Hello World!` message in JSON.

1. Create migration and seed files as needed to populate db (see <https://knexjs.org/#Migrations> for more info).

1. `IMPORTANT:` CORS is enabled for the entire server by default. If you do not want every request accessible from cross-origins, see <https://www.npmjs.com/package/cors> for instruction on limiting CORS to single routes or methods.

1. Enjoy!
