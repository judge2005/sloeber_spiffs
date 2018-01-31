# sloeber_spiffs
An ant file that adds some useful functions for ESP8266 developers to the Sloeber Eclipse plugin:

1. mkspiffs
1. upload spiffs either by wire or OTA
1. clear flash (aka factory reset)
1. decode ESP8266 stack traces

It uses the project settings to figure out where the tools are and what arguments should be passed, with a few exceptions that need to be defined in the launch config (although these are standard Eclipse variables, so nothing that is project-specific).

You will need to define an external tool to run it and pass the eclipse_home, project_loc and project_name variables in to it. An example launch config is included.

You will also need to install an [Oracle Java JRE] (http://www.oracle.com/technetwork/java/javase/downloads/index.html) and then select it as the default JRE in eclipse preferences (windows/preferences/java/installed JREs).
