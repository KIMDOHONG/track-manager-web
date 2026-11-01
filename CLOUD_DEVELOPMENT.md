# Cloud development routing

This repository contains the compiled Flutter web distribution. Development takes place in the access-controlled [Track Manager source repository](https://github.com/KIMDOHONG/track-manager).

## Start development

1. In Codex Cloud, select `KIMDOHONG/track-manager`.
2. Use source branch `chore/cloud-web-first`, based on the existing web implementation. The older source main branch does not contain the latest web entrypoint.
3. Read the source repository's `AGENTS.md`, `docs/CODEX_CLOUD.md` and `docs/WEB_FIRST_PLAN.md`.
4. Develop and verify Flutter web first, then extend the existing Android adapters and test on devices.

The source repository requires its existing access permissions. This public repository does not provide a standalone Dart build environment.

## Distribution updates

Build from the private source with entrypoint `apps/mobile/lib/web_main.dart` and base href `/track-manager-web/`. Copy only reviewed static output from `apps/mobile/build/web`. Preserve this repository's README, AGENTS.md and CLOUD_DEVELOPMENT.md when updating generated assets.

Do not edit generated `main.dart.js`, Flutter loaders or CanvasKit binaries to implement features. Do not copy the private repository, personal location/vehicle records, credentials, source maps, or captured telemetry into the public distribution.

The existing public site remains [Track Manager Web](https://kimdohong.github.io/track-manager-web/). Documentation preparation does not redeploy it or change its supported features.
