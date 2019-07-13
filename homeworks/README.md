## Instructions

I was unable to find **hw0-setup** or access to Barkley docker image so I
created my own. This should be enough to finish the homework. I automated most
of the process, so its matter of just calling few scripts.

## Important stuff

- Database `lahman.pgdump.gz` is preloaded and its name is `postgres` with all
  data to start HW1.
- DB username is `postgres`.
- Each time you do `docker-compose down` everything you changed will be lost.
  Next time you `docker-compose up` db will be preloaded from `lahman.pgdump.gz`

1. Make sure `dockerd` is running
2. from location where is `docker-compose.yml` do `docker-compose up`
    - `docker-compose up -d` to detach
3. `docker-compose exec db psql -Upostgres` - interact with database


## Homework 2019 - RDBMS
- **HW1:** SQL queries and scalable algorithms
- **HW2:** B+ Trees
- **HW3:** Iterators and Join Algorithms
- **HW4:** Cost Estimation and Query Optimization
- **HW5:** Locking

[official cs186 site 2019](https://www.cs186berkeley.net/)


