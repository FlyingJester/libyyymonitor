import os
import sys

Import("environment")

yyymonitor_files = ["monitor.cpp"]

if sys.platform.startswith('win'):
  yyymonitor_files += ["monitor_win32.c"]
else:
  yyymonitor_files += ["monitor_pthread.c"]

libyyymonitor = environment.StaticLibrary("yyymonitor", yyymonitor_files)

Return("libyyymonitor")
