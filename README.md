# contenttelemetry.org

The website for the **Content Telemetry** standard: the landing page and the
version-pinned JSON Schemas that the standard's `$id` URLs resolve to.

## Schemas

Each published version of the standard is served at an immutable, version-pinned
path. The current version is **v0.1**:

- `https://contenttelemetry.org/schema/v0.1/telemetry-session.json`
- `https://contenttelemetry.org/schema/v0.1/telemetry-event.json`
- `https://contenttelemetry.org/schema/v0.1/manifest.json`

These are served with permissive CORS so they can be fetched by validators and
tooling from any origin:

```sh
curl -s https://contenttelemetry.org/schema/v0.1/telemetry-session.json
```

A `/schema/vX.Y/` path always returns that exact version. New versions are added
alongside existing ones; published versions are never mutated.

## Canonical specification

The normative specification and the canonical copies of these schemas live in
[SPUR-Coalition/telemetry](https://github.com/SPUR-Coalition/telemetry). The
files served here are version-pinned copies of the `v0.1` release; this repository
hosts them so the schema URLs resolve. The standard is licensed under Apache 2.0.
