# Unity Logcat Debugging That Doesnt Suck

Original code from: http://ilkinulas.github.io/development/unity/2016/05/12/filter-unity-logs-logcat.html

If you've been wondering why the adb logcat output for Unity is so verbose and unusable, but have resigned to your fate, there may be hope yet. This is just a filter file for the output of adb logcat that cleans up and colorizes what you see so that its actually useful.

Script is simple enough, you should be able to modify it for your own needs. Currently I'm filtering out both warning and info messages as well.

# Prerequisites:
- Some form of python (as its a python script)

# Usage:
- Make sure you're adb device is connected and running a Unity application
- In command line, type adb logcat -v time | python logcat_unity.py
- Or adb logcat -v time | python <Path to logcat_unity.py file> if you're not in the current directory
