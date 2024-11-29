Kea's options
====================

Kea provides the following options. please consult ``kea -h`` for a full list.

``-f``: The test files that contain the properties.

``-a --apk``: The apk file of the app under test.

``-d --device_serial``: The serial number of the device used in the test. (use 'adb devices' to find)

``-o --output``: The output directory of the execution results.

``-p --policy``: The policy name of the exploration. ("random" or "guided")

``-t --timeout``: The maximum testing time(seconds).

``-n``: Every n events, then restart the app.

``-debug``: Run in debug mode (dump debug messages).

``-keep_app``: Keep the app on the device after testing.

``-grant_perm``: Grant all permissions while installing. Useful for Android 6.0+.

``-is_emulator``: Declare the target device to be an emulator, which would be treated specially.

``-is_harmonyos``: use harmonyos devices

``-load_config``: load config from config.yml. The setting in config.yml will cover the commandline args.