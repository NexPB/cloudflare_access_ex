# Changelog

All notable changes to this project will be documented in this file.

## [0.2.0] - 2026-04-16

### Changed

- Replaced `HTTPoison` with `Req` for JWKS fetching.
- Disabled duplicate HTTP retries during JWKS refreshes so retry timing stays under `JwksStrategy` control.
- Refreshed the test stack for Elixir 1.19 / OTP 28 compatibility by updating `test_server`, pinning `x509`, and running the test server on Bandit.
- Updated CI and release workflows to run on Elixir 1.19.4 / OTP 28.3.
- Moved preferred Mix task environments to `cli/0`.
- Raised the declared Elixir requirement to `~> 1.15`.
