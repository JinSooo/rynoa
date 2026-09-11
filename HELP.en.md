# User guide

[简体中文](HELP.md) · English · [Product overview](README.en.md)

Rynoa lives in the menu bar at the top of your Mac screen. Click its icon to open the panel, or reopen Rynoa from Applications.

## Getting started

1. Read the getting-started screen after installation. You can reopen it from the help and about section in settings.
2. Allow Rynoa's **Input Monitoring** and **Accessibility** permissions under **System Settings → Privacy & Security**. Input Monitoring recognizes right Command / Option gestures; Accessibility sends the shortcuts and system actions you configure.
3. Click **+** beside an input group to add a gesture, then select an app, shortcut, or system action. Only configured bindings appear on the overview. Click one to edit it. App and system-action selections save immediately; finish recording a shortcut to save it, or go back to discard the change.
4. Start with one everyday gesture. The pause control on the overview temporarily stops all actions.

Reopening the panel within 5 seconds restores the previous page, search, and unsaved shortcut draft. After 5 seconds it returns to the overview. The app picker pins the currently bound app; use search to find others.

## Change language

Starting with beta.8, Rynoa supports English and Simplified Chinese and follows your macOS language by default. To set the language for Rynoa only:

1. Open **System Settings → General → Language & Region**.
2. Under **Applications**, click **+**, select **Rynoa**, and choose **English** or **Simplified Chinese**. If Rynoa is already listed, edit its language.
3. Fully quit Rynoa, then reopen it from Applications.

You do not need to change the language of your entire system.

## Keyboard gestures

Right Command and right Option each support single tap, double tap, triple tap, and hold. Each gesture can have its own action. A single tap waits briefly after release to distinguish it from repeated taps. Normal keyboard shortcuts take precedence when the key is used with other keys.

When upgrading to beta.5, existing bindings are preserved. The two new single-tap gestures start unassigned.

## Body taps

Double, triple, and quadruple taps are supported, without distinguishing left from right. Gently tap the palm rest or body of your Mac; no force is needed. Sensors run only after you configure a body-tap action. They remain on standby without a binding and stop sampling when paused. Wait for the ready status before trying a gesture.

Recognition can vary with your Mac, desk, and posture. Hardware testing is limited, and body taps are not guaranteed on every Mac. Keyboard gestures remain available if body taps are unavailable.

## If an action does not run

- Check that triggers are not paused, the gesture has an action, and you are using the **right-hand** Command / Option key.
- Check both Input Monitoring and Accessibility permissions. If macOS asks you to quit and reopen the app, follow that prompt.
- After an update, check that the permission entries refer to Rynoa in Applications. If necessary, remove the old entry and add the current app again.
- System actions depend on your macOS shortcut settings. External audio devices may not support system volume control, and actions such as full screen require support from the foreground app.
- Setting up Do Not Disturb for the first time requires adding the helper shortcut bundled with Rynoa, then returning to the app to complete the check. Keep the bundled shortcut's name unchanged.
- If the body sensor keeps reporting errors or reconnecting, quit and reopen Rynoa. If it still fails, report your Mac model, macOS version, and reproduction steps.

## Updates

The repository was renamed from `rynoa-releases` to `rynoa`. **Beta.6 and earlier may incorrectly report that you are up to date.** Beta.7 fixes the update address. For older versions, use [Releases](https://github.com/JinSooo/rynoa/releases) directly. Rynoa never downloads or installs updates automatically.

Beta builds check for later betas and stable releases; stable builds check only for stable releases. Only releases with a DMG attachment are recommended. If a network request fails, retry or open Releases directly.

Quit the old version, download the new DMG, replace Rynoa in Applications, and reopen it. Beta.7 removes six unreliable system actions: Mission Control, Show Desktop, Application Windows, Previous Desktop, Next Desktop, and Emoji & Symbols. It backs up the original settings locally and clears only bindings for these actions. Other bindings and preferences remain. Use **+** to reassign affected gestures. Keep your previous DMG if you may need to revert.

## Quit and uninstall

Choose the quit action in settings. To uninstall, first turn off launch at login, quit Rynoa, then move it from Applications to the Trash. Removing the app does not automatically erase local preferences. If you use a future licensed version, deactivate this Mac before switching devices or uninstalling.

For more help, see [support information](SUPPORT.en.md).
