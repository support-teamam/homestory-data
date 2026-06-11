# homestory-data

Public dataset for **Home Story** (Team AM): home-maintenance task templates
with intervals, seasonal anchors, and typical cost ranges.

- `data/home-tasks.json` — the dataset (schema 1). 8 systems, month-based
  intervals, DIY/pro cost ranges, applicability by home type
  (house / townhouse / condo / apartment).
- `data/manifest.json` — version + sha256, rebuilt by CI on every data change.
  Served via GitHub Pages so shipped apps can fetch updates without an App
  Store release.

## Honesty contract

Intervals are **standard home-maintenance recommendations, not manufacturer
data**. The app presents them as such. Equipment manuals and local climate
take precedence; corrections are welcome via issues.

## Consumers

- The Home Story iOS app (v1 ships this data bundled; over-the-air updates
  read `data/manifest.json` once enabled).
- teamam.org (planned: task pages, like the vehicle maintenance pages).

Sibling repo: [carstory-data](https://github.com/support-teamam/carstory-data).
