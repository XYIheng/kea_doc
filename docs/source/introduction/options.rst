Optional arguments
====================

Kea provides the following options. please consult ``kea -h`` for a full list.

``-f``: The test files that contain the properties.

``-a --apk``: The apk file of the app under test.

``-d --device_serial``: The serial number of the device used in the test. (use 'adb devices' to find)

``-o --output``: The output directory of the execution results.

``-p --policy``: The policy name of the exploration. ("random" or "guided")

``-t --timeout``: The maximum testing time(seconds).

``-n``: Every n events, then restart the app.
