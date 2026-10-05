# interactor-study-data-vsk

A parquet datalake of the V-Sekai organizations' repositories, issues and decision records, with the studies that rank them.

## What it is for

It answers which open task can be finished today. It ingests public repositories, their open
issues and the manuals' decision records, normalizes them into parquet tables in Essential Tuple
Normal Form, and scores each open issue for how finishable it is and each repository for how
close it is to shipping as a single binary. The rankings go to `reports/`, and `SCHEMA.md`
describes the tables.

## Build and run

```sh
pixi run all
```

It reads a token from `GITHUB_TOKEN`, or from the signed-in `gh` session when that is unset.

## Licence

MIT; see `LICENSE`.
