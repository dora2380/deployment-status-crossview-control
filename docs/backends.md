# Status backend contract

A status backend registers one callable in the `starship.status_backend`
entry-point group. The callable receives the application name and returns a
mapping with `deployment`, `control_plane`, and `release_channel` fields.

Backend packages are installed separately so the same client can be used with
hosted and private deployments.
