---
name: benchmark-template
description: A fair benchmark setup in five steps, ready to fill in and run. Use when the user wants to measure something quickly without designing a methodology from scratch.
version: 1.0.0
---

# Benchmark Template

*Free gateway skill from the Perf Profiler bundle by Hankash.*

The minimum honest benchmark, as a fill-in template. It will not survive a conference review, but it will stop you from fooling yourself, which is the actual job.

## Procedure

1. **Name the thing being measured** as a user-felt operation with a unit, not as a function name. 'Search returns results (ms, p95)' beats 'query() speed'.
2. **Fix the workload:** write down the exact input data or the seed that generates it. If you cannot re-create the input, you cannot re-run the benchmark.
3. **Run warm, then measure:** at least 3 warmup runs discarded, at least 10 measured runs kept. Record all ten numbers, not just the favorite.
4. **Report median and spread** (fastest and slowest kept run). If the spread exceeds 20% of the median, the environment is too noisy to conclude anything; fix that first.
5. **Write the one-line conclusion** scoped to what was measured: this operation, this workload, this machine.

```
QUICK BENCHMARK - <date>
Measuring: <operation> (<unit>, <percentile or median>)
Workload: <data description or seed> | Machine: <one line>
Warmup: 3 discarded | Runs kept: <all numbers>
Median: <x> | Spread: <min>-<max> (<spread as % of median>)
Conclusion (scoped): <one sentence>
```

## Rules

- Never keep only the best run; all measured runs go in the record.
- Never compare against a number measured on a different day or machine; re-run both sides together or do not compare.
- If spread exceeds 20% of the median, the only valid conclusion is 'too noisy'; must not interpret the direction anyway.

## Degradation

With no timing tooling at hand, fall back to the coarsest honest clock available (even a stopwatch on a batch run), widen the noise threshold accordingly, and say so in the conclusion.


---

*Like this? The full **Perf Profiler** bundle adds the persona plus Bottleneck Hypothesizer, Benchmark Designer, Optimization Log — on Claw Mart.*
