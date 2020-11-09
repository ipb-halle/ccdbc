[![](https://img.shields.io/docker/cloud/build/ipbhalle/ccdbc.svg)](https://hub.docker.com/r/ipbhalle/ccdbc/builds/)

# ccdbc
_Combined Chemistry DataBase Cartridges_

This project combines the database extensions [pgchem](https://github.com/ergo70/pgchem_tigress) and [RDKit](https://github.com/rdkit/rdkit) in a single [PostgreSQL 11](https://www.postgresql.org/) Docker image.

This project is a spin-off of [CRIMSy](https://github.com/ipb-halle/CRIMSy) and our NatBase project (yet unpublished).

When setting up your database, please activate the extensions with the following SQL commands:

    CREATE EXTENSION IF NOT EXISTS "pgchem_tigress";
    CREATE EXTENSION IF NOT EXISTS "rdkit";
    
# More docs

The container is based on the official PostgreSQL container, so all info from https://hub.docker.com/_/postgres and in particular https://github.com/docker-library/docs/blob/master/postgres/README.md applies.

The `pgchem_tigress` extension was developed by Ernst-Georg Schmid
and can be found at https://github.com/ergo70/pgchem_tigress/.
