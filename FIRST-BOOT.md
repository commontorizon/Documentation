# First Boot

The default login is:

- login: `torizon`
- password: `torizon`

> ⚠️ Pay attention that on the first login, the system will force the change of the password.

## How to Access Device Console

### SSH

Common Torizon comes with an SSH server enabled by default. You can use any SSH client to access the device console, using the hostname or IP address of the device.

Common Torizon generate the device hostname based on the machine target and the serial number of the device. For example, if you are using a Raspberry Pi 4B and the serial number of your hardware is `100000008c7e0024`, then the hostname will be `raspberrypi4-64-100000008c7e0024`.

> ⚠️ There are know issues for some hardware that does not provide acces to serial number. In this case, the hostname will be only the machine target.

### Serial UART

If your target hardware has accessible pins to the UART, you can use an USB-to-serial cable to access the device's console.

Check the [Serial UART Configuration](./UART-PINS.md) for more information about the pins configured as UART on devices tested by the community.
