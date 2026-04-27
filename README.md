# aibg-calendar

Static hosting for AI Builders Guild cohort `.ics` files via GitHub Pages.

Files are generated from `cohort-schedule-2026.xlsx` in the (private) `intelligenceapplied` repo by `scripts/generate-ics.py`. To update, regenerate there and copy the resulting files here.

## URL pattern

```
https://misterludden.github.io/aibg-calendar/<slug>.ics
```

Where `<slug>` is one of:

- `crystal-ball`
- `fundamentals-cohort-1`, `fundamentals-cohort-2`, `fundamentals-cohort-3`
- `advanced-cohort-1`, `advanced-cohort-2`, `advanced-cohort-3`

These slugs are the values used by GHL form fields, so the email merge URL is:

```
https://misterludden.github.io/aibg-calendar/{{contact.selected_cohort}}.ics
```
