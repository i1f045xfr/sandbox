# Scratchpad

Random notes from today.

## Go microservices

- Use `context` with timeouts for all outbound HTTP calls.
- Prefer `errgroup` with `golang.org/x/sync/errgroup` for fan-out.
- Graceful shutdown: `signal.NotifyContext` + `http.Server.Shutdown`.

## Docker

- Pin base images by digest in production.
- Keep `CMD` as the binary, not `entrypoint.sh` unless needed.

## TODO

- Try `goa` vs `connect-go` for a small internal API.
- Look into `openTelemetry` logs/metrics/traces correlation.
