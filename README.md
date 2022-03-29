# PSQL Playground

This repository is meant to be an easy-to-setup, dockerized PostgreSQL database playground that you can easily run locally.

It works by converting your CSV files into Schemas and Tables automatically, and then importing the CSV data into PostgreSQL.

The data included here is baseball data from Sean Lahman's <a href="https://www.seanlahman.com/baseball-archive/statistics/"site</a>.

# Requirements

1. docker and docker compose
2. csvkit
3. pgcli

# Instructions

1. Drop your CSV files into the data folder. Ensure that the file names do not contain any special characters. These will be used as the names of the PostgreSQL tables.
2. Run `./setup` file. This will create a file that PostgreSQL will use to copy the data.
3. Run `docker-compose up` to start up the database.
4. Run `bin/connect` to connect your shell to the database.
