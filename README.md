# Starship Status Client

Starship Status Client is a small command-line tool used by deployment
operators to print the active environment and service state before a release.

## Status backends

The client loads a deployment-specific status backend from the
`starship.status_backend` Python entry-point group. Hosted, staging, and
on-premises environments may use different backends, so the core client does
not bundle one.

Set `STARSHIP_API_KEY` according to the selected backend's documentation, then
run:

```bash
python3 app.py
```

## Development

```bash
python3 -m unittest discover -s tests
```

## License

MIT
