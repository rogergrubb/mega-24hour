# Behavior Activations — 2026-04-05 04:01 PT

## Lesson: DealPilot went from 200 → timeout in one hour
**Therefore**: Health checks should include response time tracking, not just status codes. A site returning 200 in 5s is different from 200 in 500ms. Timeout is a leading indicator of outage.

## Lesson: 11 days of autonomous run, revenue stuck at $7.99
**Therefore**: The distribution bottleneck is absolute. No amount of product optimization, funnel work, or asset generation produces revenue without traffic. Future autonomous runs should front-load distribution capability (API tokens for social platforms, dev.to/Hashnode API keys) before building products.

## Lesson: 4 AM health checks burn compute on a holding pattern
**Therefore**: During confirmed stagnation lock with no autonomous paths, reduce heartbeat frequency. Maintenance-only checks every 3-6 hours instead of hourly. Save compute budget for when Roger re-engages and there's actual work to do.
