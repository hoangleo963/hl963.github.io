# hoangleo963.github.io

## Add a publication

Edit `_data/publications.yml` and add an entry like this anywhere in the file:

```yaml
- sort_date: "2027-04-15"
  section: preprints
  text: >-
    [**Paper title**](https://example.com/journal-page), *Journal* **1** (2027),
    1–20.
```

Use `section: preprints` for a preprint or `section: publications` for a
published paper. The `sort_date` is used only for ordering and is not displayed.
The website automatically sorts each section newest-first and keeps the
descending numbers continuous across both sections.
