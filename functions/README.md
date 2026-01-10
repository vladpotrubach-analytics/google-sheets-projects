# Google Sheets — Functions Practice

This folder contains my notes and practice examples for common Google Sheets functions (Google Data Analytics Certificate).

## What I practiced

### Text functions
- `LEN(text)` — count characters
- `LEFT(text, n)` / `RIGHT(text, n)` — extract first/last characters
- `FIND(search_for, text, [start_at])` — find position of a substring (case-sensitive)

#### Examples
- `=LEN(A2)`
- `=LEFT(A2, 3)`
- `=RIGHT(A2, 4)`
- `=FIND("@", A2)`

### Lookup functions
- `VLOOKUP(search_key, range, index, [is_sorted])` — lookup a value by key and return data from another column

#### Example
- `=VLOOKUP(A2, $E$2:$G$100, 3, FALSE)`

## When I use these in analytics
- Cleaning messy text fields (IDs, names, emails)
- Extracting parts of strings for grouping / categorization
- Joining data using lookup keys (basic enrichment)

## Notes / common mistakes
- `FIND` is case-sensitive (use `SEARCH` if you need case-insensitive search)
- In `VLOOKUP`, use `FALSE` for exact match (most analytics tasks need exact match)
- Lock ranges with `$` when copying formulas

