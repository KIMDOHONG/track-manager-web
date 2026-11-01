# Track Manager — public Flutter web

[Open Track Manager](https://kimdohong.github.io/track-manager-web/)

Compiled Flutter distribution. Driver mode reuses the app's track/profile editor, lap workspace and history. Browser location and browser-local storage replace native interfaces. Share your current location only after explicitly starting sharing; spectator links expire after two hours. Stopping sharing removes server coordinates when the final request arrives.

The separate example experience replays synthetic Closed/Open routes through the same lap engine. It does not represent physical driving evidence.

Foreground only. Browser lap accuracy is still under validation. Native OBD/IMU and background recording are not available here. The web route view has no road-map background. No account or cross-device permanent record synchronization. Clearing browser site data removes local records.

Third-party notices: assets/NOTICES. Private source, personal driving logs and credentials are not published in this repository.

## Develop with Codex Cloud

Use the existing Flutter source in the access-controlled Track Manager repository, branch `chore/cloud-web-first`, to develop web features first and extend the native app later. This repository remains the public build output. See [Cloud development routing](CLOUD_DEVELOPMENT.md) for the workflow.
