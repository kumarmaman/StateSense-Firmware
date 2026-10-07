# StateSense firmware releases

Signed over-the-air firmware packages for the StateSense nRF52832 device.

The StateSense mobile app reads the connected device's firmware revision,
checks the latest stable GitHub release, and offers a direct download and
Bluetooth update when a newer version is available. No manual file transfer
to the phone is required.

Download a package from [Releases](https://github.com/kumarmaman/StateSense-Firmware/releases).
For manual installation, use the `StateSense-x.y.z-ota.zip` file in the app.
Keep the device powered and nearby until the app confirms completion.

Release tags use `vMAJOR.MINOR.PATCH`, for example `v1.0.3`. Each stable release
contains exactly one signed `StateSense-MAJOR.MINOR.PATCH-ota.zip` asset.
The app verifies the asset's SHA-256 digest before sending it to the device;
MCUboot verifies the firmware signature before booting it.

This repository contains release artifacts and documentation. Production
signing keys and private source code are not stored here.
