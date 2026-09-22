# Integration Bridge

A portfolio project demonstrating reliable API and webhook integration patterns.

## What it demonstrates

- REST API integration concepts
- webhook ingestion
- JSON/schema validation
- normalization
- idempotency and duplicate protection
- retry/backoff strategy
- structured error logging
- dead-letter/replay thinking
- downstream acknowledgement
- troubleshooting and recovery

## Architecture

Source → Webhook → Validation/Normalization → API Bridge → Destination

The interactive demo includes malformed payloads, duplicate events, HTTP 429 rate limiting, and downstream HTTP 503 failures.

## Why this project exists

Business automations often work in a happy-path demo but fail when APIs time out, providers resend events, payloads change, or downstream systems become unavailable. Integration Bridge demonstrates the reliability patterns I use when designing and troubleshooting connected workflows.

## Demo note

The incidents and status codes shown in the UI are simulated engineering scenarios for portfolio demonstration, not claimed production metrics.

## Roadmap

V2: executable local webhook endpoint, configurable schema, event store, retry queue, automated tests, and JSON logs.
