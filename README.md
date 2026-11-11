# ping-monitor

A tiny, dependency-free HTTP ping / uptime checker.

## What it does

Sends a periodic HTTP request to a configurable endpoint and reports the
result. Intended for lightweight "is it still up?" style checks.

## Usage

The endpoint to probe is configured through the repository secret
`PING_TARGET` (set in repository Settings → Secrets and variables).

- Run the check manually from the **Actions** tab, or
- let the scheduled workflow run it on a fixed interval.

## Notes

- No external dependencies; uses the built-in `curl`.
- The scheduled run uses GitHub's standard `ubuntu-latest` runner.

## License

MIT
