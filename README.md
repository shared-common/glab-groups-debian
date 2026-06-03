# glab-groups-debian

Thin GitHub Actions wrapper for the Debian and Salsa namespace mirror.

## Scope

- Loads `gh-actions-cfg/glab-groups-debian`
- Calls the reusable workflow in `glab-groups-shared@main`
- Uses the BWS target PAT secret `GL_PAT_GROUP_DEBIAN_SVC`
- Runs one 25-repository batch per mirror job with five jobs max in parallel
- Schedules at minute 5 of hours 3, 9, 15, and 21 UTC
- Publishes plan, report, CSV, JSON, and Parquet artifacts for each run

## Validation

```sh
python3 -m unittest discover -s tests
```
