# Changelog

**IMPORTANT**
If you encounter any issue while installing, you might have to install additionnal packages on your environment since the main dependency of it depends on canvas library which is not available for all configurations. See there for more details : [canvas compiling](https://github.com/Automattic/node-canvas#compiling).

For use in the [oznu/homebridge](https://github.com/oznu/docker-homebridge) Docker image (Alpine Linux) please add the following line to your `startup.sh` script and restart the container. You can edit this file in directly in the Homebride UI by selecting the drop down menu in the upper-right-corner and selecting _Startup Script_.

```
apk add build-base cairo-dev jpeg-dev pango-dev giflib-dev librsvg-dev
```

You can also use the [PACKAGES](https://github.com/oznu/docker-homebridge#optional-settings) env variable directly with docker

```bash
-e PACKAGES=build-base,cairo-dev,jpeg-dev,pango-dev,giflib-dev,librsvg-dev
```

All notable changes to this project will be documented in this file.

## 1.0.2

- [FIX] adding wrong characteristic to service

## 1.0.1

- [NEW] cleaning lost devices from cache

## 1.0.0

**platform name change from HomebridgeDeebotsEcovacs to DeebotEcovacs**

- [NEW] first non pre-version release, platform name change

## 0.1.4

- [FIX] fixing more bugs

## 0.1.3

- [FIX] fixing bugs #14 and others

## 0.1.2

- [FIX] fixing bugs

## 0.1.1

- [FIX] fixing some bugs, but a lot remains :)

## 0.1.0

- [NEW] add motion sensor for notifications #12
- [NEW] add a stateless switch for beep function #11
- [NEW] Add a switch service to handle charge / start #10 . fans top now pause the deebot
- [NEW] Implement rotation direction for edge / auto mode

## 0.0.6

- [FIX] library change for better support
- [FIX] nick is not always there #7

## 0.0.5

- [FIX] some early fixes

## 0.0.4

- [FIX] fixing update of cleaning status

## 0.0.3

- [FIX] fixing platform name

## 0.0.2

- [NEW] adding config schema for Config UI-X

## 0.0.1

- [NEW] First Version
