# StikTalk

StikTalk by **Brootul** provides a dual-stick chat wheel with a complete message
preview, built-in phrase wheels and eight slots per custom wheel. Select a chat
destination with the left stick and a phrase with the right stick, then deliberately
confirm the displayed message. Custom wheels display as `Custom - <name>`.

## Availability and compatibility

Public beta preparation candidate: **1.4.0-rc.8**. No public download exists yet.
CurseForge will be the primary distribution channel; a verified link will be added
here when available. This repository does not distribute addon source or ZIPs.

The accepted implementation was tested on the Forever beta client **1.60.1,
build 70170, interface 16001**. Blizzard's announced beta testing period runs
through October 21, 2026; temporary server downtime is separate from that schedule.
The addon deliberately
guards its native controller handoff to that exact client; this is not a claim
of support for Retail, other Classic clients, or a later build. Compatibility
with an available client must be established before offering a download for it.

The author has completed in-game controller and settings/persistence acceptance
on the accepted implementation. rc.8 corrects distribution documentation following rc.7 metadata/licensing
changes; neither changes accepted gameplay behavior. **Battleground chat support is pending and is not part of this beta candidate.**
Live battleground acceptance is deferred until battlegrounds are available; it does
not block testing the current chat destinations.
Automated checks are separate from live-game acceptance. A local send attempt
does not prove server delivery; unavailable channels block sending. Frozen
whisper recipients can become unavailable and are never silently replaced.

## Controls

| Action | Control |
| --- | --- |
| Open | Menu, then D-pad Left while the native wheel is open |
| Destination / phrase | Left stick / right stick |
| Cycle included wheels | LT / RT |
| Send displayed message once | Fresh A press |
| Cancel without sending | B, Escape, or a fresh Menu press |
| Open settings | Y |
| Browse Reply recipients | LB / RB |
| Focus settings | D-pad / left stick |
| Adjust setting | Left/right / right stick |
| Select settings row or action | A |
| Include/exclude a wheel from rotation | X or checkbox |
| Back in settings | B / Escape / Y |

Custom names and phrases support keyboard text entry. An optional direct opener
can be configured; no gameplay binding is assigned automatically. `/stiktalk`
and the existing `/controllerchat` command remain available. `/stiktalk settings`
opens settings; `/stiktalk status` shows diagnostics. `/stiktalk reset` recovers
input state and does not factory-reset settings.

Settings edits are drafts: **Save settings** commits them, **Discard** restores
saved settings. Reset settings to defaults requires confirmation and remains a
draft until Save. Reset preserves custom wheels and phrases. Fresh/reset appearance
uses wheel size 0.90, horizontal position 96, vertical position 48, text size 20,
and opacity 1.00, with screen-boundary safeguards. Valid saved preferences survive
upgrades. Everyday and Campfire are included by default, starting with Everyday.

Nine premade wheels are protected. Copy a premade to customize it. New custom
wheels have eight slots and begin unchecked; at least one wheel must stay included.
New custom creation is limited to five, while existing excess and migration
preservation copies remain usable. Changing wheels requires a fresh phrase choice.

## Installation and upgrades

These instructions apply when an authorized package is available. They are not
a download announcement. Use only a package matching the supported game client.

1. Save wanted settings drafts and exit WoW completely.
2. Back up `Interface/AddOns/ControllerChat` and your `WTF` folder outside AddOns,
   including the account SavedVariables `ControllerChat.lua` and `.bak` files.
3. Extract the package into the matching client's `Interface/AddOns` folder.
   The result must be `Interface/AddOns/ControllerChat/ControllerChat.toc`, with
   no extra ZIP-name folder. Replace only this addon; preserve other addons.
4. Enable **StikTalk** in the addon list. Keep the installation folder named
   **ControllerChat**. The existing `ControllerChatDB` data identifier and saved
   bindings are intentional and must not be renamed.
5. Verify custom content, included wheels and appearance after loading. Save a
   deliberate change, reload, and restart to check persistence. Do not delete or
   overwrite SavedVariables as part of a normal upgrade.

For rollback across a migration, first back up current data, then restore the old
addon and its matching saved-data backup. Restoring a backup loses later edits;
do not assume a schema downgrade is reversible.

## Support and license

[GitHub Issues](https://github.com/mrdmarcus2013/Brootul-WoW-Addons/issues) is the
place for bugs and feature requests. Include addon version, game version/build,
controller, reproduction steps, and expected versus actual behavior. Logs and
screenshots are optional; redact private information before posting. Do not
attach complete SavedVariables or WTF folders.

Original StikTalk code and artwork: **Copyright (c) 2026 Brootul. All Rights
Reserved.** Download, installation and use are free of charge. Redistribution of
the addon/code/artwork, and publication or redistribution of modified versions,
require prior written permission from Brootul. See the LICENSE in an authorized
package for full terms. Third-party materials retain their own licenses; referenced
WoW client fonts/artwork are not bundled.
