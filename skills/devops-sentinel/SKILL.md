---
name: devops-sentinel
description: The ten checks that catch most bad deploys before they leave the driveway. Use as a fast gate before any production deploy when there's no custom checklist yet.
version: 1.0.0
---

# Deploy Checklist

*Free gateway skill from the DevOps Sentinel bundle by GarphenGate.*

The fixed ten-point gate that catches most bad deploys, runnable in five minutes with no setup.

## Procedure

1. Walk the ten checks in order against the deploy at hand; answer each yes, no, or not-applicable-because (the reason is mandatory):
   1. Is CI green on the exact commit being deployed?
   2. Does the diff contain only what you think it contains?
   3. Are migrations rehearsed and separately deployable?
   4. Are new config values and secrets present in production (not just locally)?
   5. Is there a written rollback, and does it cover data changes?
   6. Are feature flags defaulting to the safe state?
   7. Do you know the two metrics that show this deploy misbehaving?
   8. Is someone available to watch for 30 minutes after?
   9. Is this a sane time to deploy (not Friday 6pm, not during peak)?
   10. Is there a smoke test you will actually run, with expected output?
2. Any "no" on checks 1, 4, 5, or 6 means stop; fix before deploying. Other "no"s are stated risks the user may accept out loud.
3. Emit the gate result below.

Gate result:

```
DEPLOY GATE: <change> — result: GO | NO-GO (<blocking checks>)
Checks: 1 y/n ... 10 y/n (with reasons for n and n/a)
Accepted risks: <check — user's stated acceptance>
First post-deploy look: <metric/log + when>
```

## Rules

- Never let a "not applicable" pass without its reason; n/a without a why is a skipped check with better posture.
- Never soften a NO-GO into advice; blocking checks block, and the user overrides only explicitly and on the record.
- The gate takes five minutes; if it is taking twenty, the deploy needs the full custom checklist, and the result says so.

## Degradation

If the user cannot answer three or more checks, the result is NO-GO by ignorance, with the unanswered checks listed as the actual pre-deploy work.

---

*Like this? This is the free gateway skill for **DevOps Sentinel** by Moltline Studio. The paid listing: https://www.agensi.io/skills/devops-sentinel-persona*
