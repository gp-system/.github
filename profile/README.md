<p align="center">
  <strong>gp-system</strong><br>
  A service chassis and scaffolding CLI for modular Go backends
</p>

<p align="center">
  <a href="https://gpsystem.hu">Documentation</a> ·
  <a href="https://github.com/gp-system/gpsystem">gpsystem</a> ·
  <a href="https://github.com/gp-system/docs">docs source</a>
</p>

---

## gpsystem

A Go library and scaffolding CLI for building modular backends. It composes
the ecosystem's established libraries (pgx, bun, asynq, go-chi, Fiber,
OpenTelemetry, oapi-codegen) into one maintained foundation and generates
the wiring for you, so each service starts with the same solid baseline
instead of hand-rolled bootstrap code.

### Features

- Modular layout: one entry point per module (`cmd/<module>/main.go`).
- HTTP on Fiber v3 or chi, spec-first via TypeSpec, OpenAPI, oapi-codegen.
- RFC 9457 `problem+json` errors, request validation, pagination.
- JWT auth, RBAC, and fail-closed per-request policies.
- Postgres (pgx, bun), transactions, goose migrations, S3-compatible storage.
- Async: event dispatcher, transactional outbox, Redis queue, scheduler, workers.
- OpenTelemetry traces, metrics, and logs; slog logging; optional Sentry.
- Scaffolding CLI for projects, modules, handlers, events, and jobs.

### Coming from PHP?

Built with a path from Laravel or Symfony in mind. The docs have dedicated
getting-started guides for both.

## Documentation

Guides and full API reference: [gpsystem.hu](https://gpsystem.hu).

## Status

Pre-1.0. The API and CLI surface can still change between releases.
