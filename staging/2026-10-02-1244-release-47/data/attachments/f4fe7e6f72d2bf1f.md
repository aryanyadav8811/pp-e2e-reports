# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: navigation/top-nav-desktop.spec.ts >> Desktop top nav - routing and wallet pill >> Feed link routes to the feed and takes the underline
- Location: tests/navigation/top-nav-desktop.spec.ts:83:5

# Error details

```
Error: browser.newContext: Target page, context or browser has been closed
Browser logs:

[pid=3177][err] [1002/124912.041197:INFO:CONSOLE:4] "[ThemeProvider] System theme detected: light", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124912.041215:INFO:CONSOLE:4] "[ThemeProvider] Setting up system theme listener", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124912.055289:INFO:CONSOLE:4] "Browser language detected: en-US", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124912.059528:INFO:CONSOLE:4] "[ThemeProvider] Initialized with theme: light isSystem: true", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124912.061180:INFO:CONSOLE:4] "[ThemeProvider] Applying theme: light", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124912.130808:INFO:CONSOLE:4] "Radar SDK: initialized with publishableKey.", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124912.130976:INFO:CONSOLE:4] "Radar SDK (debug): using options [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124912.132537:INFO:CONSOLE:4] "Radar SDK: Using geolocation options: {"maximumAge":0,"timeout":10000,"enableHighAccuracy":true}", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124912.579617:INFO:CONSOLE:4] "[AppLifecycle] authReq data received [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124912.628989:INFO:CONSOLE:4] "Browser language detected: en-US", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124913.634298:INFO:CONSOLE:4] "[AppLifecycle] bootstrap start undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124913.644324:INFO:CONSOLE:4] "[AppLifecycle] initializeUpdater done undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124913.644369:INFO:CONSOLE:4] "[Auth] initStorageCookies [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124913.644378:INFO:CONSOLE:4] "[AppLifecycle] initStorageCookies done undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124913.644385:INFO:CONSOLE:4] "[AppLifecycle] initAppsFlyer done undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124913.644394:INFO:CONSOLE:4] "[AppLifecycle] bootstrap complete undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124913.809158:INFO:CONSOLE:4] "[ThemeProvider] Initializing theme...", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124913.809427:INFO:CONSOLE:4] "[ThemeProvider] Loaded preference from localStorage: null", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124913.810121:INFO:CONSOLE:4] "[ThemeProvider] System theme detected: light", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124913.810137:INFO:CONSOLE:4] "[ThemeProvider] Setting up system theme listener", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124913.825624:INFO:CONSOLE:4] "Browser language detected: en-US", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124913.833313:INFO:CONSOLE:4] "[ThemeProvider] Initialized with theme: light isSystem: true", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124913.833381:INFO:CONSOLE:4] "[ThemeProvider] Applying theme: light", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124914.308802:INFO:CONSOLE:4] "Radar SDK: initialized with publishableKey.", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124914.308989:INFO:CONSOLE:4] "Radar SDK (debug): using options [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124914.310120:INFO:CONSOLE:4] "Radar SDK: Using geolocation options: {"maximumAge":0,"timeout":10000,"enableHighAccuracy":true}", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124914.372196:INFO:CONSOLE:4] "[AppLifecycle] authReq data received [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124914.432001:INFO:CONSOLE:4] "Browser language detected: en-US", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124915.237403:INFO:CONSOLE:1] "[Intercom] Launcher is disabled in settings or current page does not match display conditions", source: https://js.intercomcdn.com/frame-modern.41377646.js (1)
[pid=3177][err] [1002/124915.444154:ERROR:dbus/bus.cc:405] Failed to connect to the bus: Failed to connect to socket /run/dbus/system_bus_socket: No such file or directory
[pid=3177][err] [1002/124915.444180:WARNING:dbus/property.cc:94] Failed to connect to PropertiesChangedsignal.
[pid=3177][err] [1002/124915.444210:ERROR:dbus/bus.cc:405] Failed to connect to the bus: Failed to connect to socket /run/dbus/system_bus_socket: No such file or directory
[pid=3177][err] [1002/124915.444224:ERROR:dbus/object_proxy.cc:572] Failed to call method: org.freedesktop.DBus.Properties.GetAll: object_path= /org/freedesktop/UPower/devices/DisplayDevice: unknown error type: 
[pid=3177][err] [1002/124915.444228:WARNING:dbus/property.cc:174] GetAll request failed for: org.freedesktop.UPower.Device
[pid=3177][err] [1002/124915.866270:INFO:CONSOLE:4] "[AppLifecycle] bootstrap start undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124915.869944:INFO:CONSOLE:4] "[AppLifecycle] initializeUpdater done undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124915.870206:INFO:CONSOLE:4] "[Auth] initStorageCookies [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124915.870493:INFO:CONSOLE:4] "[AppLifecycle] initStorageCookies done undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124915.870707:INFO:CONSOLE:4] "[AppLifecycle] initAppsFlyer done undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124915.870836:INFO:CONSOLE:4] "[AppLifecycle] bootstrap complete undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124916.039228:INFO:CONSOLE:4] "[ThemeProvider] Initializing theme...", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124916.039465:INFO:CONSOLE:4] "[ThemeProvider] Loaded preference from localStorage: null", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124916.039571:INFO:CONSOLE:4] "[ThemeProvider] System theme detected: light", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124916.040272:INFO:CONSOLE:4] "[ThemeProvider] Setting up system theme listener", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124916.051794:INFO:CONSOLE:4] "Browser language detected: en-US", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124916.059431:INFO:CONSOLE:4] "[ThemeProvider] Initialized with theme: light isSystem: true", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124916.059498:INFO:CONSOLE:4] "[ThemeProvider] Applying theme: light", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124916.118908:INFO:CONSOLE:4] "Radar SDK: initialized with publishableKey.", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124916.118934:INFO:CONSOLE:4] "Radar SDK (debug): using options [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124916.120355:INFO:CONSOLE:4] "Radar SDK: Using geolocation options: {"maximumAge":0,"timeout":10000,"enableHighAccuracy":true}", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124916.537465:INFO:CONSOLE:4] "[AppLifecycle] authReq data received [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124916.590883:INFO:CONSOLE:4] "Browser language detected: en-US", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124919.387020:INFO:CONSOLE:1] "[Intercom] Launcher is disabled in settings or current page does not match display conditions", source: https://js.intercomcdn.com/frame-modern.41377646.js (1)
[pid=3177][err] [1002/124919.565234:ERROR:dbus/bus.cc:405] Failed to connect to the bus: Failed to connect to socket /run/dbus/system_bus_socket: No such file or directory
[pid=3177][err] [1002/124919.565267:WARNING:dbus/property.cc:94] Failed to connect to PropertiesChangedsignal.
[pid=3177][err] [1002/124919.565274:ERROR:dbus/bus.cc:405] Failed to connect to the bus: Failed to connect to socket /run/dbus/system_bus_socket: No such file or directory
[pid=3177][err] [1002/124919.565292:ERROR:dbus/object_proxy.cc:572] Failed to call method: org.freedesktop.DBus.Properties.GetAll: object_path= /org/freedesktop/UPower/devices/DisplayDevice: unknown error type: 
[pid=3177][err] [1002/124919.565297:WARNING:dbus/property.cc:174] GetAll request failed for: org.freedesktop.UPower.Device
[pid=3177][err] [1002/124920.487926:INFO:CONSOLE:4] "[AppLifecycle] bootstrap start undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124920.490596:INFO:CONSOLE:4] "[AppLifecycle] initializeUpdater done undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124920.490798:INFO:CONSOLE:4] "[Auth] initStorageCookies [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124920.491002:INFO:CONSOLE:4] "[AppLifecycle] initStorageCookies done undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124920.491145:INFO:CONSOLE:4] "[AppLifecycle] initAppsFlyer done undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124920.491256:INFO:CONSOLE:4] "[AppLifecycle] bootstrap complete undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124920.600359:INFO:CONSOLE:4] "[ThemeProvider] Initializing theme...", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124920.600914:INFO:CONSOLE:4] "[ThemeProvider] Loaded preference from localStorage: null", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124920.601248:INFO:CONSOLE:4] "[ThemeProvider] System theme detected: light", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124920.601419:INFO:CONSOLE:4] "[ThemeProvider] Setting up system theme listener", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124920.608641:INFO:CONSOLE:4] "Browser language detected: en-US", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124920.615227:INFO:CONSOLE:4] "[ThemeProvider] Initialized with theme: light isSystem: true", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124920.615543:INFO:CONSOLE:4] "[ThemeProvider] Applying theme: light", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124920.674460:INFO:CONSOLE:4] "Radar SDK: initialized with publishableKey.", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124920.674610:INFO:CONSOLE:4] "Radar SDK (debug): using options [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124920.675372:INFO:CONSOLE:4] "Radar SDK: Using geolocation options: {"maximumAge":0,"timeout":10000,"enableHighAccuracy":true}", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124920.729701:INFO:CONSOLE:4] "[AppLifecycle] authReq data received [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124920.741142:INFO:CONSOLE:4] "Browser language detected: en-US", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.217385:INFO:CONSOLE:4] "[AppLifecycle] bootstrap start undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.220149:INFO:CONSOLE:4] "[AppLifecycle] initializeUpdater done undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.220330:INFO:CONSOLE:4] "[Auth] initStorageCookies [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.220562:INFO:CONSOLE:4] "[AppLifecycle] initStorageCookies done undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.220716:INFO:CONSOLE:4] "[AppLifecycle] initAppsFlyer done undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.220787:INFO:CONSOLE:4] "[AppLifecycle] bootstrap complete undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.313487:INFO:CONSOLE:4] "[ThemeProvider] Initializing theme...", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.314693:INFO:CONSOLE:4] "[ThemeProvider] Loaded preference from localStorage: null", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.315080:INFO:CONSOLE:4] "[ThemeProvider] System theme detected: light", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.315098:INFO:CONSOLE:4] "[ThemeProvider] Setting up system theme listener", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.324742:INFO:CONSOLE:4] "Browser language detected: en-US", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.328792:INFO:CONSOLE:4] "[ThemeProvider] Initialized with theme: light isSystem: true", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.328838:INFO:CONSOLE:4] "[ThemeProvider] Applying theme: light", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.402258:INFO:CONSOLE:4] "Radar SDK: initialized with publishableKey.", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.402422:INFO:CONSOLE:4] "Radar SDK (debug): using options [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.403094:INFO:CONSOLE:4] "Radar SDK: Using geolocation options: {"maximumAge":0,"timeout":10000,"enableHighAccuracy":true}", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.425380:INFO:CONSOLE:4] "[AppLifecycle] authReq data received [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.429845:INFO:CONSOLE:4] "Browser language detected: en-US", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.778844:INFO:CONSOLE:4] "[AppLifecycle] bootstrap start undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.779998:INFO:CONSOLE:4] "[AppLifecycle] initializeUpdater done undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.780143:INFO:CONSOLE:4] "[Auth] initStorageCookies [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.780297:INFO:CONSOLE:4] "[AppLifecycle] initStorageCookies done undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.780330:INFO:CONSOLE:4] "[AppLifecycle] initAppsFlyer done undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.780390:INFO:CONSOLE:4] "[AppLifecycle] bootstrap complete undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.863368:INFO:CONSOLE:4] "[ThemeProvider] Initializing theme...", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.863429:INFO:CONSOLE:4] "[ThemeProvider] Loaded preference from localStorage: null", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.863516:INFO:CONSOLE:4] "[ThemeProvider] System theme detected: light", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.863536:INFO:CONSOLE:4] "[ThemeProvider] Setting up system theme listener", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.867002:INFO:CONSOLE:4] "Browser language detected: en-US", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.868763:INFO:CONSOLE:4] "[ThemeProvider] Initialized with theme: light isSystem: true", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.868856:INFO:CONSOLE:4] "[ThemeProvider] Applying theme: light", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.909204:INFO:CONSOLE:4] "Radar SDK: initialized with publishableKey.", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.909318:INFO:CONSOLE:4] "Radar SDK (debug): using options [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.910536:INFO:CONSOLE:4] "Radar SDK: Using geolocation options: {"maximumAge":0,"timeout":10000,"enableHighAccuracy":true}", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.947226:INFO:CONSOLE:4] "[AppLifecycle] authReq data received [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124921.951579:INFO:CONSOLE:4] "Browser language detected: en-US", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124922.378305:INFO:CONSOLE:4] "[AppLifecycle] bootstrap start undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124922.381333:INFO:CONSOLE:4] "[AppLifecycle] initializeUpdater done undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124922.381542:INFO:CONSOLE:4] "[Auth] initStorageCookies [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124922.381839:INFO:CONSOLE:4] "[AppLifecycle] initStorageCookies done undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124922.382041:INFO:CONSOLE:4] "[AppLifecycle] initAppsFlyer done undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124922.382210:INFO:CONSOLE:4] "[AppLifecycle] bootstrap complete undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124922.521789:INFO:CONSOLE:4] "[ThemeProvider] Initializing theme...", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124922.522034:INFO:CONSOLE:4] "[ThemeProvider] Loaded preference from localStorage: null", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124922.522259:INFO:CONSOLE:4] "[ThemeProvider] System theme detected: light", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124922.522457:INFO:CONSOLE:4] "[ThemeProvider] Setting up system theme listener", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124922.529758:INFO:CONSOLE:4] "Browser language detected: en-US", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124922.534090:INFO:CONSOLE:4] "[ThemeProvider] Initialized with theme: light isSystem: true", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124922.534322:INFO:CONSOLE:4] "[ThemeProvider] Applying theme: light", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124922.578550:INFO:CONSOLE:4] "Radar SDK: initialized with publishableKey.", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124922.578592:INFO:CONSOLE:4] "Radar SDK (debug): using options [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124922.579387:INFO:CONSOLE:4] "Radar SDK: Using geolocation options: {"maximumAge":0,"timeout":10000,"enableHighAccuracy":true}", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124922.975117:INFO:CONSOLE:4] "[AppLifecycle] authReq data received [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124923.028442:INFO:CONSOLE:4] "Browser language detected: en-US", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124923.881596:INFO:CONSOLE:4] "[AppLifecycle] bootstrap start undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124923.884837:INFO:CONSOLE:4] "[AppLifecycle] initializeUpdater done undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124923.885080:INFO:CONSOLE:4] "[Auth] initStorageCookies [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124923.885411:INFO:CONSOLE:4] "[AppLifecycle] initStorageCookies done undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124923.885626:INFO:CONSOLE:4] "[AppLifecycle] initAppsFlyer done undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124923.885774:INFO:CONSOLE:4] "[AppLifecycle] bootstrap complete undefined", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124924.014255:INFO:CONSOLE:4] "[ThemeProvider] Initializing theme...", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124924.014626:INFO:CONSOLE:4] "[ThemeProvider] Loaded preference from localStorage: null", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124924.014739:INFO:CONSOLE:4] "[ThemeProvider] System theme detected: light", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124924.014956:INFO:CONSOLE:4] "[ThemeProvider] Setting up system theme listener", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124924.023376:INFO:CONSOLE:4] "Browser language detected: en-US", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124924.028606:INFO:CONSOLE:4] "[ThemeProvider] Initialized with theme: light isSystem: true", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124924.028829:INFO:CONSOLE:4] "[ThemeProvider] Applying theme: light", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124924.076731:INFO:CONSOLE:4] "Radar SDK: initialized with publishableKey.", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124924.076898:INFO:CONSOLE:4] "Radar SDK (debug): using options [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124924.077617:INFO:CONSOLE:4] "Radar SDK: Using geolocation options: {"maximumAge":0,"timeout":10000,"enableHighAccuracy":true}", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124924.431684:INFO:CONSOLE:4] "[AppLifecycle] authReq data received [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124924.494172:INFO:CONSOLE:4] "Browser language detected: en-US", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124924.649080:INFO:CONSOLE:4] "[AppLifecycle] authReq data received [object Object]", source: https://staging.parlayplay.io/_next/static/chunks/pages/_app-182069e7938d0955.js (4)
[pid=3177][err] [1002/124925.290332:INFO:CONSOLE:1] "[Intercom] Launcher is disabled in settings or current page does not match display conditions", source: https://js.intercomcdn.com/frame-modern.41377646.js (1)
```

# Test source

```ts
  371 |             } catch (err) {
  372 |               log.error(`auth[${role}]: leader login failed`, {
  373 |                 durationMs: Date.now() - t0,
  374 |                 error: (err as Error).message,
  375 |               });
  376 |               throw err;
  377 |             } finally {
  378 |               try {
  379 |                 fs.rmSync(lockPath);
  380 |               } catch {
  381 |                 /* noop */
  382 |               }
  383 |             }
  384 |             break;
  385 |           } catch (err) {
  386 |             const code = (err as NodeJS.ErrnoException).code;
  387 |             if (code !== 'EEXIST') throw err;
  388 |             // Another worker is logging in. If its lock has outlived any
  389 |             // plausible login (leader process died without running finally),
  390 |             // take it over; otherwise back off and check again.
  391 |             try {
  392 |               const age = Date.now() - fs.statSync(lockPath).mtimeMs;
  393 |               if (age > STALE_LOCK_MS) {
  394 |                 log.warn(`auth[${role}]: login lock is stale — taking it over`, {
  395 |                   lockAgeMs: Math.round(age),
  396 |                 });
  397 |                 fs.rmSync(lockPath, { force: true });
  398 |                 continue;
  399 |               }
  400 |             } catch {
  401 |               continue; // lock vanished between EEXIST and stat — retry now
  402 |             }
  403 |             if (Date.now() >= nextWaitLog) {
  404 |               log.debug(`auth[${role}]: another worker holds the login lock — waiting`, {
  405 |                 waitedMs: Date.now() - waitStart,
  406 |               });
  407 |               nextWaitLog = Date.now() + WAIT_LOG_EVERY_MS;
  408 |             }
  409 |             await new Promise((r) => setTimeout(r, 500));
  410 |           }
  411 |         }
  412 |         cache.set(username, statePath);
  413 |         return statePath;
  414 |       };
  415 |       await use(factory);
  416 |     },
  417 |     { scope: 'worker' },
  418 |   ],
  419 | 
  420 |   primaryStorageStatePath: [
  421 |     async ({ storageStateFor }, use) => {
  422 |       const { username, password } = loginMatrix[0];
  423 |       const statePath = await storageStateFor(username, password);
  424 |       await use(statePath);
  425 |     },
  426 |     { scope: 'worker' },
  427 |   ],
  428 | 
  429 |   // Profile (username / email / phone / referral code) of the primary account,
  430 |   // for specs that need an identity the backend already knows — e.g. the
  431 |   // signup "already taken" checks. Read once per worker.
  432 |   existingUser: [
  433 |     async ({ browser, primaryStorageStatePath }, use, workerInfo) => {
  434 |       const projectUse = workerInfo.project.use as {
  435 |         baseURL?: string;
  436 |         httpCredentials?: { username: string; password: string };
  437 |         userAgent?: string;
  438 |       };
  439 |       const profile = await fetchUserProfile(browser, primaryStorageStatePath, {
  440 |         baseURL: projectUse.baseURL,
  441 |         httpCredentials: projectUse.httpCredentials,
  442 |         userAgent: projectUse.userAgent,
  443 |       });
  444 |       await use(profile);
  445 |     },
  446 |     { scope: 'worker' },
  447 |   ],
  448 | 
  449 |   // Test-scoped page that boots already authenticated as the primary user
  450 |   // (loginMatrix[0]). Uses the worker-cached storageState so no login API
  451 |   // call is made per test — but verifies the session is still alive first and
  452 |   // re-logs-in once if the server invalidated it mid-run (the failure mode
  453 |   // that cascaded a whole run into logged-out timeouts).
  454 |   loggedInPage: async (
  455 |     { browser, contextOptions, baseURL, storageStateFor, primaryStorageStatePath, diag },
  456 |     use,
  457 |   ) => {
  458 |     let statePath = primaryStorageStatePath;
  459 |     if (!(await sessionAlive(statePath, baseURL, contextOptions.httpCredentials, 'primary'))) {
  460 |       log.warn('session[primary]: dead before the test — forcing a fresh login');
  461 |       const { username, password } = loginMatrix[0];
  462 |       statePath = await storageStateFor(username, password, true);
  463 |       if (!(await sessionAlive(statePath, baseURL, contextOptions.httpCredentials, 'primary'))) {
  464 |         log.error('session[primary]: still unauthenticated after a fresh login');
  465 |         throw new Error(
  466 |           '[e2e:infra] loggedInPage: session still unauthenticated after a fresh login — ' +
  467 |             'check the test user credentials and staging auth (Cloudflare rate limit / bot challenge).',
  468 |         );
  469 |       }
  470 |     }
> 471 |     const ctx = await browser.newContext({
      |                 ^ Error: browser.newContext: Target page, context or browser has been closed
  472 |       ...contextOptions,
  473 |       storageState: statePath,
  474 |     });
  475 |     diag.watch(ctx);
  476 |     const page = await ctx.newPage();
  477 |     await suppressIosBanner(page, baseURL);
  478 |     await suppressNextDevOverlay(page);
  479 |     await installCloudflareGuard(page);
  480 |     await installHud(page);
  481 |     await use(page);
  482 |     await ctx.close();
  483 |   },
  484 | 
  485 |   // A freshly registered account for flows that must end in a state no shared
  486 |   // user may be left in (frozen, stale terms). Registered through the fixed-OTP
  487 |   // signup API (@creates-user @mock-otp) and hard-deleted in teardown — which,
  488 |   // unlike a `finally` in the test body, still runs when a route handler or
  489 |   // fixture error abandons the test mid-way.
  490 |   throwawayUser: async ({ baseURL, contextOptions }, use) => {
  491 |     const user = await createThrowawayUser({
  492 |       baseURL,
  493 |       httpCredentials: contextOptions.httpCredentials,
  494 |     });
  495 |     await use(user);
  496 |     await deleteThrowawayUser(user);
  497 |   },
  498 | 
  499 |   // Page already authenticated as `throwawayUser`, with the same guards as loggedInPage.
  500 |   throwawayPage: async (
  501 |     { browser, contextOptions, baseURL, storageStateFor, throwawayUser, diag },
  502 |     use,
  503 |   ) => {
  504 |     const statePath = await storageStateFor(throwawayUser.username, throwawayUser.password);
  505 |     const ctx = await browser.newContext({ ...contextOptions, storageState: statePath });
  506 |     diag.watch(ctx);
  507 |     const page = await ctx.newPage();
  508 |     await suppressIosBanner(page, baseURL);
  509 |     await suppressNextDevOverlay(page);
  510 |     await installCloudflareGuard(page);
  511 |     await installHud(page);
  512 |     await use(page);
  513 |     await ctx.close();
  514 |   },
  515 | });
  516 | 
  517 | export { expect };
  518 | export const base_expect = base.expect;
  519 | 
```