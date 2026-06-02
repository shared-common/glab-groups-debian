# glab-groups-debian

Thin GitHub Actions wrapper for the Debian and Salsa namespace mirror.

## Scope

- Loads `gh-actions-cfg/glab-groups-debian`
- Calls the reusable workflow in `glab-groups-shared`
- Publishes plan, report, CSV, JSON, and Parquet artifacts for each run

## Validation

```sh
python3 -m unittest discover -s tests
```
