# roswaal-spec

Publishes [spec.roswaal.app](https://spec.roswaal.app/), Roswaal's technical
specification. The pages and the build live in
[Roswaal](https://github.com/neopolitans/Roswaal): its tables are generated
from Roswaal's source, so the current draft is built from it each time, by
Roswaal's `spec.yml`, as [roswaal-site](https://github.com/neopolitans/roswaal-site)
does for roswaal.app.

```sh
gh workflow run spec.yml --repo neopolitans/roswaal-spec
```

## Drafts

The latest draft is served at the root, and also at `/<draft>/`, the address
to cite. When a newer draft replaces it, the old one's published pages are
copied into `drafts/<draft>/` here, unchanged, and are served from then on as
they are rather than rebuilt from a source that has moved on.
