# EdgeX

[中文](./README.md)

## Introduction

EdgeX is an LSPosed/Xposed module for Android 15+ that combines edge gestures, hardware key actions, an app freezer drawer, and several system shortcuts into one module as a tribute to Xposed Edge.

Currently implemented features:

- 16 edge trigger zones: all four edges support three segmented zones, plus a low-priority full-edge fallback zone.
- Each zone can be configured with single tap, double tap, long press, and edge-appropriate swipe gestures.
- Sub-gesture support: chain a hold or second-stage up/down/left/right swipe after the primary gesture.
- Hardware key actions for Volume Up, Volume Down, and Power, each with click, double click, and long press triggers.
- Available actions include Back, Home, Recents, Expand Notifications, Lock Screen, Screenshot, Global Copy, Kill Foreground App, Clear Background Apps, brightness control, volume control, launch app, app shortcuts, music control, and custom shell commands.
- Freezer support for freezing/unfreezing apps, storing a freezer list, opening a Freezer Drawer from gestures or keys, and refreezing apps in one step.
- The Freezer Drawer supports both classic grid mode and arc layout mode.
- Extra features include theme presets, custom RGB accent color, gesture debug overlay, action icons, and update checking.

Notes:

- The module currently targets Android 15+.
- LSPosed/Xposed scope should include at least `android` and `com.android.systemui`.
- Root or system-level hook capability is required for Freezer, clearing background apps, some shortcut discovery flows, and some shell-based actions.
