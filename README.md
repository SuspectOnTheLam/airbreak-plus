# Probably compatible with all devices running SX567-0401
This firmware patcher has its fingerprinting disabled. Use at your own risk. Do not attempt to patch devices not running SW SX567-0401. You WILL brick your device.

# Stock look and feel
The "Hacked!" warnings have been removed and the custom palette has been taken out as well. Your machine will have many extra modes but it will not be noticeably different from a stock machine because the customizations are not applied. You can change the `patch-airsense` as you see fit.

# Jailbreaking CPAP machines to make temporary ventilators

This is the README for the internals of ResMed CPAP jailbreak works;
for a high-level overview, see [airbreak.dev](https://airbreak.dev).
The project is [MIT licnsed](LICENSE.txt) and has a [CoC](CODE_OF_CONDUCT.md).
Please review the [Contributor's Guidelines](CONTRIBUTORS.md) before
submitting issues or pull requests.

**This tree does not contain any files that are copyrighted by ResMed.**
You must have a device to extract the firmware from, which is then patched,
and the modified version is re-flashed.

You will need the tools described in [docs/disassembly](docs/disassembly.md).
The `stubs.S` file that has been committed is for SX567-0401. Flashing it on
a different version will likely cause problems.

Extensions can either replace existing functions at fixed addresses,
or can use some of the unused space in the image.
The `Makefile` has a short explanation of how to do this; the
`patch-airsense` file will also need to be updated to patch the
binary file into the firmware.

# How to install

Follow the instructions here but use this Airbreak Plus repository instead:
[https://airbreak.dev/firmware/](https://airbreak.dev/firmware/)


