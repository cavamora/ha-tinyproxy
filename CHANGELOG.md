# Changelog

## [1.0.3] - 2026-07-24

- Rename `log_level` to `tinyproxy_log_level` because the base add-on image
  treats generic `log_level` as its own setting and rejects Tinyproxy's
  `Connect` level during startup.

## [1.0.2] - 2026-07-24

- Change default `log_level` from `Notice` to `Connect` so proxy access/connection
  logs are emitted to add-on stdout and collected by HAOS journald / Grafana Alloy.
- Document Grafana Loki access-log queries.

## [1.0.1] - 2026-07-23

- Initial release: tinyproxy on the host network with configurable port,
  client ACL (`allowed_clients`), `CONNECT` port allowlist, `Via:` header
  toggle, log level, max clients and timeout.
