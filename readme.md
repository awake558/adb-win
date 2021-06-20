

## [platform-tools](https://developer.android.com/studio/releases/platform-tools)

[CN](https://developer.android.google.cn/studio/releases/platform-tools?hl=en)

- 31.0.2 (April 2021)
	- adb
		- Support forwarding to vsock on linux.
		- Fix bug in adb track-devices where devices over wireless debugging wouldn't immediately receive updates.
		- Implement preliminary support for mDNS device discovery without a separately installed mDNS service. This is currently disabled by default, and can be enabled by setting the environment variable ADB_MDNS_OPENSCREEN to 1 when starting the adb server.
	- fastboot
		- Don't fail when unable to get boot partition size.
		- Derive device locked state from property instead of parsing the kernel command line.

	- [platform-tools_r31.0.2-windows](https://dl.google.com/android/repository/platform-tools_r31.0.2-windows.zip)
	- [platform-tools_r31.0.2-linux](https://dl.google.com/android/repository/platform-tools_r31.0.2-linux.zip)
	- [platform-tools_r31.0.2-darwin](https://dl.google.com/android/repository/platform-tools_r31.0.2-darwin.zip)

- 31.0.1 (March 2021)

	- adb
		- Reduce TCP keepalive interval.
		- Improve incremental installation performance.
	- fastboot
		- Add support for compressed snapshot merges.
		- Restore legacy A/B support.

	- [platform-tools_r31.0.1-windows](https://dl.google.com/android/repository/platform-tools_r31.0.1-windows.zip)
	- [platform-tools_r31.0.1-linux](https://dl.google.com/android/repository/platform-tools_r31.0.1-linux.zip)
	- [platform-tools_r31.0.1-darwin](https://dl.google.com/android/repository/platform-tools_r31.0.1-darwin.zip)

- 31.0.0 (February 2021)

	- adb
		- Disable compression on pull by default.

	- [platform-tools_r31.0.0-windows](https://dl.google.com/android/repository/platform-tools_r31.0.0-windows.zip)
	- [platform-tools_r31.0.0-linux](https://dl.google.com/android/repository/platform-tools_r31.0.0-linux.zip)
	- [platform-tools_r31.0.0-darwin](https://dl.google.com/android/repository/platform-tools_r31.0.0-darwin.zip)

- 30.0.5 (November 2020)

	- adb
		- Improve performance of adb push when pushing many files over a high-latency connection.
		- Improve adb push/pull performance on Windows.
		- Fix adb push --sync with multiple inputs.
		- Improve performance of incremental apk installation.
		- Improve error handling for incremental apk installation.

	- [platform-tools_r30.0.5-windows](https://dl.google.com/android/repository/platform-tools_r30.0.5-windows.zip)
	- [platform-tools_r30.0.5-linux](https://dl.google.com/android/repository/platform-tools_r30.0.5-linux.zip)
	- [platform-tools_r30.0.5-darwin](https://dl.google.com/android/repository/platform-tools_r30.0.5-darwin.zip)

- 30.0.4 (July 2020)
	- adb
		- Fix fallback to non-incremental apk installation on pre-Android 11 devices.
		- Fix adb install-multi-package.
		- Fix some more crashes related to adb wireless pairing.
		- Improve some error messages.
	- fastboot
		- Improve console output on fastboot oem commands.
		- Fix fastboot flashall on older devices such as Nexus 7.

	- [platform-tools_r30.0.4-windows](https://dl.google.com/android/repository/platform-tools_r30.0.4-windows.zip)
	- [platform-tools_r30.0.4-linux](https://dl.google.com/android/repository/platform-tools_r30.0.4-linux.zip)
	- [platform-tools_r30.0.4-darwin](https://dl.google.com/android/repository/platform-tools_r30.0.4-darwin.zip)

- 30.0.3 (June 2020)
	- adb
		- Fix installation of APKs signed with v4 signature scheme on pre-Android 11 devices.
		- Fix crash when authenticating without ADB_VENDOR_KEYS.
		- Fix crash when using adb -H.

	- [platform-tools_r30.0.3-windows](https://dl.google.com/android/repository/platform-tools_r30.0.3-windows.zip)
	- [platform-tools_r30.0.3-linux](https://dl.google.com/android/repository/platform-tools_r30.0.3-linux.zip)
	- [platform-tools_r30.0.3-darwin](https://dl.google.com/android/repository/platform-tools_r30.0.3-darwin.zip)

- 30.0.2 (June 2020)
	- adb
		- Improve adb wireless pairing.
		- Fix hang in adb logcat when run before a device is connected.
		- Add adb transport-id to allow scripts to safely wait for a device to go away after root/unroot/reboot.

	- [platform-tools_r30.0.2-windows](https://dl.google.com/android/repository/platform-tools_r30.0.2-windows.zip)
	- [platform-tools_r30.0.2-linux](https://dl.google.com/android/repository/platform-tools_r30.0.2-linux.zip)
	- [platform-tools_r30.0.2-darwin](https://dl.google.com/android/repository/platform-tools_r30.0.2-darwin.zip)

- 30.0.1 (May 2020)
	- adb
		- Disable adb mdns auto-connection by default. This can be reenabled with the ADB_MDNS_AUTO_CONNECT environment variable.
		- Improve performance of adb install-multi on Android 10 or newer devices.
		- Fix timeout when using adb root/unroot on a device connected over TCP.
		- Update support for wireless pairing.

	- [platform-tools_r30.0.1-windows](https://dl.google.com/android/repository/platform-tools_r30.0.1-windows.zip)
	- [platform-tools_r30.0.1-linux](https://dl.google.com/android/repository/platform-tools_r30.0.1-linux.zip)
	- [platform-tools_r30.0.1-darwin](https://dl.google.com/android/repository/platform-tools_r30.0.1-darwin.zip)

- 30.0.0 (April 2020)
	- adb
		- Add initial support for wireless pairing.
		- Add support for incremental APK installation.
		- Implement client-side support for compression of adb {push, pull, sync} when used with an Android 11 device.
		- Improve performance of adb push on high-latency connections.
		- Improve push/pull performance on Windows.

	- [platform-tools_r30.0.0-windows](https://dl.google.com/android/repository/platform-tools_r30.0.0-windows.zip)
	- [platform-tools_r30.0.0-linux](https://dl.google.com/android/repository/platform-tools_r30.0.0-linux.zip)
	- [platform-tools_r30.0.0-darwin](https://dl.google.com/android/repository/platform-tools_r30.0.0-darwin.zip)

- 29.0.6 (February 2020)
	- adb
		- 64-bit size/time support for adb ls when used with an Android 11 device.
		- Support listening on ::1 on POSIX.
		- Client support for WinUSB devices that publish a WinUSB descriptor (required for Android 11) should no longer require a USB driver to be installed.
		- Fix hang when using adb install on something that isn't actually a file.

	- [platform-tools_r29.0.6-windows](https://dl.google.com/android/repository/platform-tools_r29.0.6-windows.zip)
	- [platform-tools_r29.0.6-linux](https://dl.google.com/android/repository/platform-tools_r29.0.6-linux.zip)
	- [platform-tools_r29.0.6-darwin](https://dl.google.com/android/repository/platform-tools_r29.0.6-darwin.zip)

- 29.0.5 (October 2019)
	- adb
		- Slight performance improvement on Linux when using many simultaneous connections.
		- Add --fastdeploy option to adb install, for incremental updates to APKs while developing.

	- [platform-tools_r29.0.5-windows](https://dl.google.com/android/repository/platform-tools_r29.0.5-windows.zip)
	- [platform-tools_r29.0.5-linux](https://dl.google.com/android/repository/platform-tools_r29.0.5-linux.zip)
	- [platform-tools_r29.0.5-darwin](https://dl.google.com/android/repository/platform-tools_r29.0.5-darwin.zip)

- 29.0.4 (September 2019)
	- adb
		- Hotfix for native debugging timeout with LLDB (see issue #134613180). This also fixes a related bug in the Android Studio Profilers that causes an AdbCommandRejectedException, which you can see in the idea.log file.

	- [platform-tools_r29.0.4-windows](https://dl.google.com/android/repository/platform-tools_r29.0.4-windows.zip)
	- [platform-tools_r29.0.4-linux](https://dl.google.com/android/repository/platform-tools_r29.0.4-linux.zip)
	- [platform-tools_r29.0.4-darwin](https://dl.google.com/android/repository/platform-tools_r29.0.4-darwin.zip)

- 29.0.3 (September 2019)
	- adb
		- adb forward --list works with multiple devices connected.
		- Fix devices going offline on Windows.
		- Improve adb install output and help text.
		- Restore previous behavior of adb connect <host> without specifying port.

	- [platform-tools_r29.0.3-windows](https://dl.google.com/android/repository/platform-tools_r29.0.3-windows.zip)
	- [platform-tools_r29.0.3-linux](https://dl.google.com/android/repository/platform-tools_r29.0.3-linux.zip)
	- [platform-tools_r29.0.3-darwin](https://dl.google.com/android/repository/platform-tools_r29.0.3-darwin.zip)

- 29.0.2 (July 2019)
	- adb
		- Fixes a Windows heap integrity crash.
		- fastboot
		- Adds support for partition layout of upcoming devices.

	- [platform-tools_r29.0.2-windows](https://dl.google.com/android/repository/platform-tools_r29.0.2-windows.zip)
	- [platform-tools_r29.0.2-linux](https://dl.google.com/android/repository/platform-tools_r29.0.2-linux.zip)
	- [platform-tools_r29.0.2-darwin](https://dl.google.com/android/repository/platform-tools_r29.0.2-darwin.zip)

- 29.0.1 (June 2019)
	- adb
		- Hotfix for Windows crashes (https://issuetracker.google.com/134613180)

	- [platform-tools_r29.0.1-windows](https://dl.google.com/android/repository/platform-tools_r29.0.1-windows.zip)
	- [platform-tools_r29.0.1-linux](https://dl.google.com/android/repository/platform-tools_r29.0.1-linux.zip)
	- [platform-tools_r29.0.1-darwin](https://dl.google.com/android/repository/platform-tools_r29.0.1-darwin.zip)

- 29.0.0 (June 2019)
	- adb
		- adb reconnect performs a USB reset on Linux.
		- On Linux, when connecting to a newer adb server, instead of killing the server and starting an older one, adb attempts to launch the newer version transparently.
		- adb root waits for the device to reconnect after disconnecting. Previously, adb root; adb wait-for-device could mistakenly return immediately if adb wait-for-device started before adb noticed that the device had disconnected.
	- fastboot
		- Disables an error message that occurred when fastboot attempted to open the touch bar or keyboard on macOS.

	- [platform-tools_r29.0.0-windows](https://dl.google.com/android/repository/platform-tools_r29.0.0-windows.zip)
	- [platform-tools_r29.0.0-linux](https://dl.google.com/android/repository/platform-tools_r29.0.0-linux.zip)
	- [platform-tools_r29.0.0-darwin](https://dl.google.com/android/repository/platform-tools_r29.0.0-darwin.zip)

- 28.0.3
	- [platform-tools_r28.0.3-windows](https://dl.google.com/android/repository/platform-tools_r28.0.3-windows.zip)
	- [platform-tools_r28.0.3-linux](https://dl.google.com/android/repository/platform-tools_r28.0.3-linux.zip)
	- [platform-tools_r28.0.3-darwin](https://dl.google.com/android/repository/platform-tools_r28.0.3-darwin.zip)
- 28.0.2 (March 2019)
	- adb
		- Fixes flakiness of adb shell port forwarding that leads to "Connection reset by peer" error message.
		- Fixes authentication via ADB_VENDOR_KEYS when reconnecting devices.
		- Fixes authentication—when the private key used for authentication does not match the public key—by calculating the public key from the private key, instead of assuming that they match.
	- fastboot
		- Adds support for dynamic partitions.
		- Updated Windows requirements
		- The platform tools now depend on the Windows Universal C Runtime, which is usually installed by default via Windows Update. If you see errors mentioning missing DLLs, you may need to manually fetch and install the runtime package.

	- [platform-tools_r28.0.2-windows](https://dl.google.com/android/repository/platform-tools_r28.0.2-windows.zip)
	- [platform-tools_r28.0.2-linux](https://dl.google.com/android/repository/platform-tools_r28.0.2-linux.zip)
	- [platform-tools_r28.0.2-darwin](https://dl.google.com/android/repository/platform-tools_r28.0.2-darwin.zip)
- 28.0.1 (September 2018)
	- adb
		- Add support for reconnection of TCP connections. Upon disconnection, adb will attempt to reconnect for up to 60 seconds before abandoning a connection.
		- Fix Unicode console output on Windows. (Thanks to external contributor Spencer Low!)
		- Fix a file descriptor double-close that can occur, resulting in connections being closed when an adb connect happens simultaneously.
		- Fix adb forward --list when used with more than one device connected.
	- Fastboot
		- Increase command timeout to 30 seconds, to better support some slow bootloader commands.

	- [platform-tools_r28.0.1-windows](https://dl.google.com/android/repository/platform-tools_r28.0.1-windows.zip)
	- [platform-tools_r28.0.1-linux](https://dl.google.com/android/repository/platform-tools_r28.0.1-linux.zip)
	- [platform-tools_r28.0.1-darwin](https://dl.google.com/android/repository/platform-tools_r28.0.1-darwin.zip)
- 28.0.0 (June 2018)
	- adb:
		- Add support for checksum-less operation with devices running Android P, which improves throughput by up to 40%.
		- Sort output of adb devices by connection type and device serial.
		- Increase the socket listen backlog to allow for more simulataneous adb commands.
		- Improve error output for adb connect.
	- fastboot:
		- Improve output format, add a verbose output mode (-v).
		- Clean up help output.
		- Add product.img and odm.img to the list of partitions flashed by fastboot flashall.
		- Avoid bricking new devices when using a too-old version of fastboot by allowing factory image packages to require support for specific partitions.

	- [platform-tools_r28.0.0-windows](https://dl.google.com/android/repository/platform-tools_r28.0.0-windows.zip)
	- [platform-tools_r28.0.0-linux](https://dl.google.com/android/repository/platform-tools_r28.0.0-linux.zip)
	- [platform-tools_r28.0.0-darwin](https://dl.google.com/android/repository/platform-tools_r28.0.0-darwin.zip)
- 27.0.1 (December 2017)
	- adb: fixes an assertion failure on MacOS that occurred when connecting devices using USB 3.0.
	- Fastboot: On Windows, adds support for wiping devices that use F2FS (Flash-Friendly File System).

	- [platform-tools_r27.0.1-windows](https://dl.google.com/android/repository/platform-tools_r27.0.1-windows.zip)
	- [platform-tools_r27.0.1-linux](https://dl.google.com/android/repository/platform-tools_r27.0.1-linux.zip)
	- [platform-tools_r27.0.1-darwin](https://dl.google.com/android/repository/platform-tools_r27.0.1-darwin.zip)
- 27.0.0 (December 2017)
	- [platform-tools_r27.0.0-windows](https://dl.google.com/android/repository/platform-tools_r27.0.0-windows.zip)
	- [platform-tools_r27.0.0-linux](https://dl.google.com/android/repository/platform-tools_r27.0.0-linux.zip)
	- [platform-tools_r27.0.0-darwin](https://dl.google.com/android/repository/platform-tools_r27.0.0-darwin.zip)
- 26.0.2 (October 2017)
	- [platform-tools_r26.0.2-windows](https://dl.google.com/android/repository/platform-tools_r26.0.2-windows.zip)
	- [platform-tools_r26.0.2-linux](https://dl.google.com/android/repository/platform-tools_r26.0.2-linux.zip)
	- [platform-tools_r26.0.2-darwin](https://dl.google.com/android/repository/platform-tools_r26.0.2-darwin.zip)
- 26.0.1 (September 2017)
	- [platform-tools_r26.0.1-windows](https://dl.google.com/android/repository/platform-tools_r26.0.1-windows.zip)
	- [platform-tools_r26.0.1-linux](https://dl.google.com/android/repository/platform-tools_r26.0.1-linux.zip)
	- [platform-tools_r26.0.1-darwin](https://dl.google.com/android/repository/platform-tools_r26.0.1-darwin.zip)
- 26.0.0 (June 2017)
	- [platform-tools_r26.0.0-windows](https://dl.google.com/android/repository/platform-tools_r26.0.0-windows.zip)
	- [platform-tools_r26.0.0-linux](https://dl.google.com/android/repository/platform-tools_r26.0.0-linux.zip)
	- [platform-tools_r26.0.0-darwin](https://dl.google.com/android/repository/platform-tools_r26.0.0-darwin.zip)
- 25.0.6
	- [platform-tools_r25.0.6-windows](http://dl.google.com/android/repository/platform-tools_r25.0.6-windows.zip)
	- [platform-tools_r25.0.6-linux](http://dl.google.com/android/repository/platform-tools_r25.0.6-linux.zip)
	- [platform-tools_r25.0.6-darwin](http://dl.google.com/android/repository/platform-tools_r25.0.6-darwin.zip)
- 25.0.5 (April 24, 2017)
	- Fixed adb sideload of large updates on Windows, manifesting as "std::bad_alloc" (bug 37139736).
	- Fixed adb problems with some Windows firewalls, manifesting as "cannot open transport registration socketpair" (bug 37139725).
	- Both adb --version and fastboot --version now include the install path.
	- Changed adb to not resolve localhost to work around misconfigured VPN.
	- Changed adb to no longer reset USB devices on Linux, which could affect other attached USB devices.

	- [platform-tools_r25.0.5-windows](http://dl.google.com/android/repository/platform-tools_r25.0.5-windows.zip)
	- [platform-tools_r25.0.5-linux](http://dl.google.com/android/repository/platform-tools_r25.0.5-linux.zip)
	- [platform-tools_r25.0.5-darwin](http://dl.google.com/android/repository/platform-tools_r25.0.5-darwin.zip)
- 25.0.4 (March 16, 2017)
	- Added experimental libusb support to Linux and Mac adb
	To use the libusb backend, set the environment variable ADB_LIBUSB=true before launching a new adb server. The new adb host-features command will tell you whether or not you're using libusb.

	To restart adb with libusb and check that it worked, use adb kill-server; ADB_LIBUSB=1 adb start-server; adb host-features. The output should include "libusb".

	In this release, the old non-libusb implementation remains the default.

	- fastboot doesn't hang 2016 MacBook Pros anymore (bug 231129)

	- Fixed Systrace command line capture on Mac

	- [platform-tools_r25.0.4-windows](http://dl.google.com/android/repository/platform-tools_r25.0.4-windows.zip)
	- [platform-tools_r25.0.4-linux](http://dl.google.com/android/repository/platform-tools_r25.0.4-linux.zip)
	- [platform-tools_r25.0.4-darwin](http://dl.google.com/android/repository/platform-tools_r25.0.4-darwin.zip)
- 25.0.3 (December 16, 2016)
	- Fixed fastboot bug causing Android Things devices to fail to flash

	- [platform-tools_r25.0.3-windows](http://dl.google.com/android/repository/platform-tools_r25.0.3-windows.zip)
	- [platform-tools_r25.0.3-linux](http://dl.google.com/android/repository/platform-tools_r25.0.3-linux.zip)
	- [platform-tools_r25.0.3-darwin](http://dl.google.com/android/repository/platform-tools_r25.0.3-darwin.zip)
- 25.0.2 (December 12, 2016)
	- Updated with the Android N MR1 Stable release (API 25)

	- [platform-tools_r25.0.2-windows](http://dl.google.com/android/repository/platform-tools_r25.0.2-windows.zip)
	- [platform-tools_r25.0.2-linux](http://dl.google.com/android/repository/platform-tools_r25.0.2-linux.zip)
	- [platform-tools_r25.0.2-darwin](http://dl.google.com/android/repository/platform-tools_r25.0.2-darwin.zip)
- 25.0.1 (November 22, 2016)
	- Updated with the release of Android N MR1 Developer Preview 2 release (API 25)

	- [platform-tools_r25.0.1-windows](http://dl.google.com/android/repository/platform-tools_r25.0.1-windows.zip)
	- [platform-tools_r25.0.1-linux](http://dl.google.com/android/repository/platform-tools_r25.0.1-linux.zip)
	- [platform-tools_r25.0.1-darwin](http://dl.google.com/android/repository/platform-tools_r25.0.1-darwin.zip)
- 25.0.0 (October 19, 2016)
	- Updated with the release of Android N MR1 Developer Preview 1 release (API 25)

	- [platform-tools_r25-windows](http://dl.google.com/android/repository/platform-tools_r25-windows.zip)
	- [platform-tools_r25-linux](http://dl.google.com/android/repository/platform-tools_r25-linux.zip)
	- [platform-tools_r25-darwin](http://dl.google.com/android/repository/platform-tools_r25-darwin.zip)
- 24.0.4 (October 14, 2016)
	- Updated to address issues in ADB and Mac OS Sierra

	- [platform-tools_r24.0.4-windows](http://dl.google.com/android/repository/platform-tools_r24.0.4-windows.zip)
	- [platform-tools_r24.0.4-linux](http://dl.google.com/android/repository/platform-tools_r24.0.4-linux.zip)
	- [platform-tools_r24.0.4-darwin](http://dl.google.com/android/repository/platform-tools_r24.0.4-darwin.zip)
- 24.0.3
	- [platform-tools_r24.0.3-windows](http://dl.google.com/android/repository/platform-tools_r24.0.3-windows.zip)
	- [platform-tools_r24.0.3-linux](http://dl.google.com/android/repository/platform-tools_r24.0.3-linux.zip)
	- [platform-tools_r24.0.3-darwin](http://dl.google.com/android/repository/platform-tools_r24.0.3-darwin.zip)
- 24.0.2
	- [platform-tools_r24.0.2-windows](http://dl.google.com/android/repository/platform-tools_r24.0.2-windows.zip)
	- [platform-tools_r24.0.2-linux](http://dl.google.com/android/repository/platform-tools_r24.0.2-linux.zip)
	- [platform-tools_r24.0.2-darwin](http://dl.google.com/android/repository/platform-tools_r24.0.2-darwin.zip)
- 24
	- [platform-tools_r24-windows](http://dl.google.com/android/repository/platform-tools_r24-windows.zip)
	- [platform-tools_r24-linux](http://dl.google.com/android/repository/platform-tools_r24-linux.zip)
	- [platform-tools_r24-darwin](http://dl.google.com/android/repository/platform-tools_r24-darwin.zip)
- 23.1.0
	- [platform-tools_r23.1.0-windows](http://dl.google.com/android/repository/platform-tools_r23.1.0-windows.zip)
	- [platform-tools_r23.1.0-linux](http://dl.google.com/android/repository/platform-tools_r23.1.0-linux.zip)
	- [platform-tools_r23.1.0-darwin](http://dl.google.com/android/repository/platform-tools_r23.1.0-darwin.zip)
- 22
	- [platform-tools_r22-windows](http://dl.google.com/android/repository/platform-tools_r22-windows.zip)
	- [platform-tools_r22-linux](http://dl.google.com/android/repository/platform-tools_r22-linux.zip)
	- [platform-tools_r22-darwin](http://dl.google.com/android/repository/platform-tools_r22-darwin.zip)
- 21
	- [platform-tools_r21-windows](http://dl.google.com/android/repository/platform-tools_r21-windows.zip)
	- [platform-tools_r21-linux](http://dl.google.com/android/repository/platform-tools_r21-linux.zip)
	- [platform-tools_r21-darwin](http://dl.google.com/android/repository/platform-tools_r21-darwin.zip)
- 20
	- [platform-tools_r20-windows](http://dl.google.com/android/repository/platform-tools_r20-windows.zip)
	- [platform-tools_r20-linux](http://dl.google.com/android/repository/platform-tools_r20-linux.zip)
	- [platform-tools_r20-darwin](http://dl.google.com/android/repository/platform-tools_r20-darwin.zip)
- 19.0.2
	- [platform-tools_r19.0.2-windows](http://dl.google.com/android/repository/platform-tools_r19.0.2-windows.zip)
	- [platform-tools_r19.0.2-linux](http://dl.google.com/android/repository/platform-tools_r19.0.2-linux.zip)
	- [platform-tools_r19.0.2-darwin](http://dl.google.com/android/repository/platform-tools_r19.0.2-darwin.zip)
- 19.0.1
	- [platform-tools_r19.0.1-windows](http://dl.google.com/android/repository/platform-tools_r19.0.1-windows.zip)
	- [platform-tools_r19.0.1-linux](http://dl.google.com/android/repository/platform-tools_r19.0.1-linux.zip)
	- [platform-tools_r19.0.1-darwin](http://dl.google.com/android/repository/platform-tools_r19.0.1-darwin.zip)
- 19
	- [platform-tools_r19-windows](http://dl.google.com/android/repository/platform-tools_r19-windows.zip)
	- [platform-tools_r19-linux](http://dl.google.com/android/repository/platform-tools_r19-linux.zip)
	- [platform-tools_r19-darwin](http://dl.google.com/android/repository/platform-tools_r19-darwin.zip)
- 18.0.1
	- [platform-tools_r18.0.1-windows](http://dl.google.com/android/repository/platform-tools_r18.0.1-windows.zip)
	- [platform-tools_r18.0.1-linux](http://dl.google.com/android/repository/platform-tools_r18.0.1-linux.zip)
	- [platform-tools_r18.0.1-darwin](http://dl.google.com/android/repository/platform-tools_r18.0.1-darwin.zip)
- 18
	- [platform-tools_r18-windows](http://dl.google.com/android/repository/platform-tools_r18-windows.zip)
	- [platform-tools_r18-linux](http://dl.google.com/android/repository/platform-tools_r18-linux.zip)
	- [platform-tools_r18-darwin](http://dl.google.com/android/repository/platform-tools_r18-darwin.zip)
- 17
	- [platform-tools_r17-windows](http://dl.google.com/android/repository/platform-tools_r17-windows.zip)
	- [platform-tools_r17-linux](http://dl.google.com/android/repository/platform-tools_r17-linux.zip)
	- [platform-tools_r17-darwin](http://dl.google.com/android/repository/platform-tools_r17-darwin.zip)
- 16.0.2
	- [platform-tools_r16.0.2-windows](http://dl.google.com/android/repository/platform-tools_r16.0.2-windows.zip)
	- [platform-tools_r16.0.2-linux](http://dl.google.com/android/repository/platform-tools_r16.0.2-linux.zip)
	- [platform-tools_r16.0.2-darwin](http://dl.google.com/android/repository/platform-tools_r16.0.2-darwin.zip)
- 16.0.1
	- [platform-tools_r16.0.1-windows](http://dl.google.com/android/repository/platform-tools_r16.0.1-windows.zip)
	- [platform-tools_r16.0.1-linux](http://dl.google.com/android/repository/platform-tools_r16.0.1-linux.zip)
	- [platform-tools_r16.0.1-darwin](http://dl.google.com/android/repository/platform-tools_r16.0.1-darwin.zip)
- 16
	- [platform-tools_r16-windows](http://dl.google.com/android/repository/platform-tools_r16-windows.zip)
	- [platform-tools_r16-linux](http://dl.google.com/android/repository/platform-tools_r16-linux.zip)
	- [platform-tools_r16-darwin](http://dl.google.com/android/repository/platform-tools_r16-darwin.zip)
- 14
	- [platform-tools_r14-windows](http://dl.google.com/android/repository/platform-tools_r14-windows.zip)
	- [platform-tools_r14-linux](http://dl.google.com/android/repository/platform-tools_r14-linux.zip)
	- [platform-tools_r14-darwin](http://dl.google.com/android/repository/platform-tools_r14-darwin.zip)
- 13
	- [platform-tools_r13-windows](http://dl.google.com/android/repository/platform-tools_r13-windows.zip)
	- [platform-tools_r13-linux](http://dl.google.com/android/repository/platform-tools_r13-linux.zip)
	- [platform-tools_r13-darwin](http://dl.google.com/android/repository/platform-tools_r13-darwin.zip)
- 12
	- [platform-tools_r12-windows](http://dl.google.com/android/repository/platform-tools_r12-windows.zip)
	- [platform-tools_r12-linux](http://dl.google.com/android/repository/platform-tools_r12-linux.zip)
	- [platform-tools_r12-darwin](http://dl.google.com/android/repository/platform-tools_r12-darwin.zip)
- 11
	- [platform-tools_r11-windows](http://dl.google.com/android/repository/platform-tools_r11-windows.zip)
	- [platform-tools_r11-linux](http://dl.google.com/android/repository/platform-tools_r11-linux.zip)
	- [platform-tools_r11-darwin](http://dl.google.com/android/repository/platform-tools_r11-darwin.zip)
- 10
	- [platform-tools_r10-windows](http://dl.google.com/android/repository/platform-tools_r10-windows.zip)
	- [platform-tools_r10-linux](http://dl.google.com/android/repository/platform-tools_r10-linux.zip)
	- [platform-tools_r10-darwin](http://dl.google.com/android/repository/platform-tools_r10-darwin.zip)


