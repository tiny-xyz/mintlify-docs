# Tiny Exchange internal docs

This repository is the standalone Mintlify source for Tiny Exchange's internal
integration documentation. It contains only documentation pages, Mintlify
configuration, and the OpenAPI schemas used to generate the API reference.

The exchange implementation and canonical protocol behavior live in the
private `tiny-xyz/tiny-exchange` repository. Update these docs alongside any
implementation change that affects authentication, wire formats, endpoints,
WebSocket events, recovery, or fees.

## Preview and validate

```sh
npx --yes mintlify@latest validate
npx --yes mintlify@latest broken-links
npx --yes mintlify@latest dev
```

The local preview is available at `http://localhost:3000`.

## Publishing

Mintlify deploys the `main` branch. Merge documentation changes into `main` to
publish them.
