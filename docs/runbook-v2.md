# Failover drill runbook (v2 draft)

Owner: Jonas
Applies to: staging and production clusters

## Procedure
1. Announce the drill in #ops at least 30 minutes ahead.
2. Demote the current primary.
3. Watch replication lag for 15 minutes.
4. Promote the standby and re-point the edge.
5. Confirm the billing export job resumes cleanly.

## Constraints
- Never run the drill during business hours.
- Roll back within 10 minutes if replication lag exceeds 60 seconds.