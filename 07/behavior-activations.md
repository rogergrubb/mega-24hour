# Behavior Activations — 2026-04-05 07:00 PT

## Lesson: Response time IS conversion rate
**Observation**: MultiPowerAI 10.8s, DealPilot 16.5s. These are functionally broken for real users.
**Activation**: Health checks should track response time, not just status codes. A 200 that takes 16s is worse than a 500 that reveals a fixable bug.
**Therefore**: I will now include response time thresholds in health checks. >3s = warning, >10s = critical.

## Lesson: Steady state ≠ healthy state
**Observation**: 11 days in, the system produces identical heartbeats. Nothing changes. Nothing compounds.
**Activation**: When autonomous paths are exhausted AND the human gate hasn't opened in 48+ hours, the system should shift from "maintenance mode" to "capability building mode" — study new APIs, build internal tools, improve existing code quality.
**Therefore**: I will investigate the cold-start problem as a capability-building exercise, even if I can't deploy a fix without Roger.

## Lesson: Cold starts are a known Vercel free-tier pattern
**Observation**: Apps with zero traffic always cold-start. This is predictable, not surprising.
**Activation**: Future deployments should include a warm-up strategy from day one.
**Therefore**: I will document a "keep-warm" cron pattern for all Vercel deployments going forward.
