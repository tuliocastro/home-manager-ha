# Family Documents

> [!WARNING]
> This Home Assistant app is currently for **my personal local installation only**. It is under active development and is **not ready for community installation or support**.

Family Documents is the Home Assistant dashboard for my private Home Manager document system.

The app runs behind Home Assistant Ingress and pulls a pre-built multi-architecture image from:

`ghcr.io/tuliocastro/family-documents`

## Current assumptions

The current build assumes infrastructure from my private Home Manager deployment, including a compatible Supabase schema and private runtime credentials.

Those backend services, credentials, migration history, n8n workflows, and family data are **not** part of this public repository.

Do not treat the current configuration or API surface as stable. Breaking changes may occur while local testing continues.

## Security

The app intentionally exposes no host port and is designed to be accessed through Home Assistant Ingress.

Supabase credentials are supplied at runtime through Home Assistant app configuration. They must never be committed to this repository or embedded in the container image.

## Supported architectures

- amd64
- aarch64
