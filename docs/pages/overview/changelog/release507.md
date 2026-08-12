## Version 5.0.7 ##

Release Date : 2026-08-12

The 5.0.7 release is a small release and is mainly focused on dependency upgrades.

### Key Highlights

- **Dual Retry Store support for Jetty-based failed message retrier** — Introduces `RetryFromJettyDualStore`, allowing requests to be routed to one of two `RetryStore` instances based on a configurable routing expression and store identifiers. A new `RetryFromJettyBase` class provides shared infrastructure (endpoints, routing, listeners, lifecycle) used by both the existing `RetryFromJetty` and the new dual-store variant. See [Dual Retry Store](/pages/advanced/advanced-dual-retry-store) for more details.
