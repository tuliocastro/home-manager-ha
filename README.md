# Home Manager — Home Assistant Apps

> [!WARNING]
> **Personal / experimental repository — not ready for community use.**
>
> This repository currently exists only to support my own local Home Assistant installation while I develop and test Home Manager.
>
> **Please do not install or rely on this repository yet.** It has not been packaged, documented, security-reviewed, tested, or supported for general-purpose community deployment. Configuration, APIs, data models, images, and update behavior may change without notice.

## Current status

Home Manager is being developed and validated against my own private, local Home Assistant environment first.

At this stage:

- this is **not** a Home Assistant Community Store or community-supported project;
- there is **no compatibility guarantee** outside my own installation;
- there is **no support commitment** for third-party installations;
- releases may include breaking changes without migration instructions;
- security assumptions currently depend on my local Home Assistant setup and Home Assistant Ingress;
- the application expects private backend services and credentials that are **not** provided by this repository.

The public repository is intentionally small. It contains only the Home Assistant app metadata needed for my local update mechanism. The application source, family data, database migrations, automation workflows, credentials, and operational configuration remain private.

## Family Documents

The current app is **Family Documents**, a private dashboard for my Home Manager family-document system.

The app image is published to GitHub Container Registry as:

`ghcr.io/tuliocastro/family-documents`

The image contains only the application runtime needed by Home Assistant. Runtime credentials are configured separately inside Home Assistant and are not stored in this repository or baked into the image.

## Why is this repository public?

Home Assistant can consume a public third-party app repository and a public GHCR image without requiring GitHub credentials. This repository exists primarily to provide that update path for my own Home Assistant instance.

I may make Home Manager suitable for wider use later. Until that happens, **treat everything here as development infrastructure for a personal installation, not as a distributable product.**

## Reuse and support

No community support, compatibility commitment, or installation guidance is currently offered. This repository does not currently include an open-source license granting reuse or redistribution rights.
