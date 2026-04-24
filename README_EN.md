# EdgeX

[中文](./README.md)

## Introduction

EdgeX is an LSPosed/Xposed module for Android 15+ that combines edge gestures, hardware key actions, an app freezer drawer, and several system shortcuts into one module as a tribute to Xposed Edge.

Currently implemented features:

- 6 edge trigger zones: top/middle/bottom on both the left and right sides.
- Each zone can be configured with single tap, double tap, long press, swipe up, swipe down, and inward swipe.
- Hardware key actions for Volume Up, Volume Down, and Power, each with click, double click, and long press triggers.
- Available actions include Back, Home, Recents, Lock Screen, Screenshot, Global Copy, Kill Foreground App, brightness control, volume control, app shortcuts, and custom shell commands.
- Freezer support for freezing/unfreezing apps, storing a freezer list, opening a Freezer Drawer from gestures or keys, and refreezing apps in one step.
- The Freezer Drawer supports both classic grid mode and arc layout mode.
- Extra features include theme presets, custom RGB accent color, gesture debug overlay, and update checking.

Notes:

- The module currently targets Android 15+.
- LSPosed/Xposed scope should include at least `android` and `com.android.systemui`.
- Root is required for Freezer, some shortcut discovery flows, and some shell-based actions.
