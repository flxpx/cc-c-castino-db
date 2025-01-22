# Database for CC C Castino

This database is designed for use in a local environment and with the configurators WordPress database. It stores the data in the folder `db-data` (which is ignored by git).

## How to Start

Requires Docker CLI.

- Run `docker compose up -d` to start.
- Run `docker compose down` to stop.
- Alternatively, run `docker compose up` and stop with `CTRL+C`.

## Test Connection with MySQL Workbench

Connect to the database in MySQL Workbench by opening a connection to `localhost:3307` with the user `root` and the password `password`.

## Warning

Do not change the MySQL root password in `compose.yml` if you have persistent data in `db-data` already, as this will break the database.
