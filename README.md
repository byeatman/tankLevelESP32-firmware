# TankLevelESP32 Firmware Releases

This public repository hosts signed OTA firmware assets for the private TankLevelESP32 source project. It contains release binaries and metadata only; do not publish source code or credentials here.

Each release includes:

- `firmware.bin`: ESP32-S3 application image.
- `manifest.json`: version and SHA-256 checksum.
- `manifest.sig`: base64-encoded RSA/SHA-256 signature of the manifest.

The device verifies the manifest signature with its embedded public key and checks the firmware checksum before installing an update. The private signing key is kept in the source repository's GitHub Actions secrets.
