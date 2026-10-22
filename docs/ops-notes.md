# Ops meeting notes - week of 2026-04-06

Attendees: Hezi, Mia, Jonas
Note-taker: Hezi

## v2 release status
Code freeze: 2026-04-24. Everything on the open-items list must land before the freeze.

## Open items for v2
1. Migrate the billing export job off the legacy cron host. Owner: Mia.
2. Publish the updated failover drill runbook. Owner: Jonas. Current draft: drafts/runbook-v2.md.
3. Rotate the staging database credentials before the freeze. Owner: Hezi.

## Decisions
- The failover drill must never run during business hours.
- This cycle the handoff repo lives under the release lead's own GitHub account.