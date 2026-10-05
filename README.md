# The Ledge

A small money transfer API I'm building in Go and PostgreSQL.

Status: early. Right now I have the schema and the local setup, no server yet. I'll keep
updating this as I go.

## Why I'm building this

Fintech is the space I want to work in, and money movement is the part of it I find most
interesting. I'm also aiming at backend roles that lean more toward cloud and
infrastructure, so getting hands on with Go, Postgres and Docker matters for that. Reading
about all three only gets you so far, so I wanted to build something small and actually
understand and familiarize myself with how it works.

A ledger seemed like a good place to start. The product idea is simple enough: people have
accounts with money in them and they send money to each other. The complexity shows up as
soon as more than one transfer is happening at the same time.

## Stack

Go, PostgreSQL, pgx, Docker Compose

## Running it

```bash
make up        # start postgres in docker
make migrate   # create the tables
make psql      # have a look around
```