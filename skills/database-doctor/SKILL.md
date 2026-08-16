---
name: index-advisor
description: Paste a slow query and schema, get ranked index candidates with reasoning and costs. Use when a specific query is slow and you suspect an index would help.
version: 1.0.0
---

# Index Advisor

*Free gateway skill from the Database Doctor bundle by Hankash.*

Paste a slow query and its schema; get ranked index candidates with the reasoning shown and the costs stated.

## Procedure

1. Take the query, the relevant table definitions with existing indexes, and if available approximate row counts and the execution plan. Name the engine; index behavior differs.
2. Extract the query's access pattern: equality predicates, range predicates, join keys, sort and group columns, and the selected column set.
3. Build candidates by the standard shape: equality columns first, then the range column, then sort columns; consider a covering index when the selected set is small and the query is hot.
4. Check each candidate against existing indexes (is it redundant? does it make an existing one redundant?) and against the table's write load, since every index taxes every write.
5. Rank candidates by expected benefit for this query against ongoing cost, and emit the advice below.

Advice format:

```
INDEX ADVICE: <query purpose> — engine: <name>
Access pattern: eq(<cols>) range(<col>) join(<cols>) sort(<cols>)
Candidates:
  1. <index definition> — why this column order — expected effect
  2. ...
Redundancy: <existing index affected | none>
Write cost note: <what this index taxes>
Verify with: <EXPLAIN command before/after>
```

## Rules

- Never recommend an index without explaining the column order; order is the difference between an index and a paperweight.
- Never present advice as confirmed without a before-and-after plan check; the verify step ships with every recommendation.
- If the honest answer is that no index fixes this query shape, say so and name the rewrite that would.

## Degradation

Without row counts or a plan, give the candidates with reasoning but label expected effects "unmeasured", and make the plan-collection command the first step of the advice.

---

*Like this? The full **Database Doctor** bundle adds the persona plus Schema Reviewer, Query Optimizer, Migration Guard — on Claw Mart.*
