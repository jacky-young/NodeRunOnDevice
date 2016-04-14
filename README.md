# NodeRunOnDevice

An shell script for nodejs tests running on python-unsupported target devices

## Running steps

1. Modify your device node tests path on script parameter BIG_TESTS_BASE_DIR likes "/data/nodejs/node-5.6.0/test/"

2. Modify node tests name list on script parameter BIG_TESTS_NAME likes "(message sequential parallel pummel internet gc debugger addons/async-hello-world ...)", you can find node BUILT_IN_TESTS names on tools/test.py

3. Modify your device executive node command path on script parameter CMD_CONFIG or else "which node" path will be default

4. Adb push this script to device & `adb shell` `chmod 755 noderun.sh`, then `./noderun.sh`

5. The node running result will directly show on device command line
