# Prebuilt Development Images

<p align="center">
  <img src="/assets/img/TCB128.png" alt="TorizonCore Builder Logo">
</p>

For each development cycle, [we provide development prebuilt images](https://github.com/commontorizon/meta-common-torizon/releases) for the following targets:

- Beagle Bone Black
- Beagle Play
- Raspberry Pi 3
- Raspberry Pi 4
- Intel x86-64

These images are available to accelerate the development and evaluation of the Torizon ecosystem, it's come with some packages and services for development and debugging already set:

- strace
- tcpdump
- gdb
- gdbserver
- perf
- kexec
- trace-cmd
- ssh server
- root user without password

## Feature Support

What are the differences between the features available for Torizon on Toradex modules and the images available for community boards?

| Feature                      | Toradex SoM | Rpi3 | Rpi4 | Nezha D1 | x86-64 | Beagle Bone Black | Rpi Zero W2 | BeaglePlay |
| ---------------------------- | ----------- | ---- | ---- | -------- | ------ | ----------------- | ----------- | ---------- |
| OTA Update OS Image          | ✅           | ✅    | ✅    |          | ⚠️**** |                   | ✅           |            |
| OTA Update Container App     | ✅           | ✅    | ✅    | ✅        | ✅      | ✅                 | ✅           | ✅          |
| OTA Update Bootloader        | ✅           |      |      |          |        |                   |             |            |
| Device Monitoring            | ✅           | ✅    | ✅    | ✅        | ✅      | ✅                 | ✅           | ✅          |
| LTS Hardware & BSP           | ✅           |      |      |          |        |                   |             |            |
| Free Toradex Technical Support       | ✅           |      |      |          |        |                   |             |            |
| Prebuilt Image   | ✅           | ✅    | ✅    | ✅        | ✅      | ✅                 | ✅           | ✅          |
| QA Pipeline         | ✅           |      |      |          |        |                   |             |            |
| TEZI*      | ✅           |      |      |          |        |                   |             |            |
| TCB** | ✅           |      |      |          |        |                   |             |            |
| VS Code Ext | ✅           | ✅    | ✅    | ⚠️***    | ⚠️***  | ✅                 | ✅           | ✅          |

> ⚠️* **TEZI**: Toradex Easy Installer;

> ⚠️** **TCB**: TorizonCore Builder;

> ⚠️*** **VS Code Extension**: are not all the templates that support RISC-V and x86-64 architectures;

> ⚠️**** **OTA Update:** Auto rollback is not implemented for x86-64;

## Telemetry

Only anonymous data is collected. Please consider that the data we collect is used to improve your development experience and better serve you. We use the data to know where put the efforts, for the most used machines.

The [service that collects the data is the `telemetry_0.1.bb`](https://github.com/commontorizon/meta-common-torizon/tree/kirkstone/recipes-support/telemetry/telemetry). You can check the data that is collect from the `telemetry` script, in summary:

- User Region;
- Board Model;
- Board Architecture;
- Common Torizon OS Version;
- dmesg logs;

> ⚠️ This data is sent to the server only once on the boot, and only if the user has an internet connection.

## Questions?

If you have any questions or feedback you can [join our discord channel](https://discord.gg/qKZgCq95df), you can use the github issues or post it on the [Torizon Community](https://community.toradex.com).
