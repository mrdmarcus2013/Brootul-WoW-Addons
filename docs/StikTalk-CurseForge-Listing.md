# StikTalk — CurseForge submission draft

Prepared October 2, 2026 (America/New_York). This is listing preparation, not a download announcement. No CurseForge submission has been made.

## Project fields

- Name: StikTalk
- Author credit: Brootul
- Game: World of Warcraft
- Class: Addons
- Suggested main category: Chat & Communication (confirm the exact available category in the author console).
- Additional category: use a relevant controller/interface category only if offered; avoid unrelated categories.
- License selection: All Rights Reserved. The packaged LICENSE grants free download, installation and use.
- Issue tracker: https://github.com/mrdmarcus2013/Brootul-WoW-Addons/issues
- Documentation: https://github.com/mrdmarcus2013/Brootul-WoW-Addons/blob/main/docs/StikTalk.md
- Logo: approved 512×512 branding/StikTalk-CurseForge.png from the private source project. Keep it outside the addon ZIP.
- No external addon dependency.

## Summary — paste into the summary field

A controller-friendly chat wheel for WoW Forever. Choose a channel and send preset or custom phrases without typing.

## Description — paste into the description field

**Chat with your controller.**

StikTalk by **Brootul** puts everyday conversation on a dual-stick chat wheel. Choose a chat destination with your left stick, choose a phrase with your right stick, review the message, then press A to send.

### Features

- Seven chat destinations: Say, Yell, Party, Raid, Guild, Reply, and Whisper Target.
- Nine built-in phrase wheels, including Everyday, Campfire, Dungeon Tank, and Healer.
- Choose which wheels appear in your rotation, then cycle through them with LT and RT.
- Create up to five custom wheels with eight phrase slots each.
- Copy a built-in wheel to make your own version.
- Adjust wheel size, position, text size, and opacity.
- Preview the message and destination before sending.
- Cancel without sending; unavailable destinations block sending.

Custom names and phrases are entered with the keyboard. Once configured, phrases can be selected and sent with your controller.

### Controls

| Action | Xbox-style control |
| --- | --- |
| Open StikTalk | Menu, then D-pad Left while the native wheel is open |
| Select destination | Left stick |
| Select phrase | Right stick |
| Switch included wheels | LT / RT |
| Send the displayed message | A |
| Cancel | B or Menu; Escape also works |
| Open settings | Y |
| Browse Reply recipients | LB / RB |

Use `/stiktalk settings` to open settings. Settings changes apply when you choose **Save settings**; **Discard** cancels the draft. Resetting settings preserves custom wheels and phrases.

### Public beta compatibility

This candidate is **StikTalk 1.4.0-rc.8** for the WoW Forever beta client **1.60.1, build 70170, interface 16001**. Its controller integration is guarded to this exact client. Other builds, Retail, and other Classic clients are not claimed supported.

**Battleground chat support is pending and is not included in this candidate. Voice-to-text is not included.**

The author has completed in-game controller and settings/persistence acceptance on the accepted implementation. Wider beta testing is intended to collect feedback on controller setups, UI scales, and everyday use.

### Installation

Install into the matching Forever beta client. For manual installation, extract the ZIP so that the addon is at:

`Interface/AddOns/ControllerChat/ControllerChat.toc`

Enable **StikTalk** in the addon list. The folder name **ControllerChat** is intentional; keep it unchanged. When upgrading, preserve your saved settings and custom phrases.

When an approved download is available, select the matching Forever installation and opt into beta files in the CurseForge app. App availability and the matching upload tag must be verified before distribution. Manual ZIP installation is also supported.

### Feedback

[Report a bug or suggest a feature on GitHub Issues](https://github.com/mrdmarcus2013/Brootul-WoW-Addons/issues/new/choose).

Include the addon version, game version/build, controller, and steps to reproduce the issue. Screenshots and Lua errors are helpful when relevant. Redact private information; do not upload your complete WTF folder or SavedVariables.

**Free to download and use. Original code and artwork are All Rights Reserved by Brootul. See the packaged LICENSE for terms.**

## File fields and beta changelog

- ZIP: StikTalk-v1.4.0-rc.8.zip
- Display name: StikTalk 1.4.0-rc.8 — Forever Beta
- Release type: Beta
- Game flavor: Forever; confirm the matching version tag in the live upload form.
- Reviewed client: 1.60.1 / 70170 / interface 16001.
- Reported ZIP SHA-256: 446707916d2db8afe777b0c93360e099b791f94adf948a9d2db08222c52915bb
- Never substitute a Retail or unrelated Classic version tag.
- The actual installed addon folder remains ControllerChat.

Paste-ready changelog:

> First public beta candidate of StikTalk by Brootul.
>
> Dual-stick destination and phrase selection, seven chat destinations, nine premade wheels, checked-wheel rotation, and up to five custom wheels with eight slots each. Includes message previews, adjustable appearance, and draft-based settings with Save, Discard, and Reset to Defaults.
>
> rc.8 corrects distribution documentation following rc.7 author, license, and support metadata changes, preserving the accepted gameplay behavior and artwork. Existing ControllerChat settings and custom content retain their established saved-data identifiers.
>
> Supported client: WoW Forever beta 1.60.1, build 70170, interface 16001. Battleground chat and voice-to-text are not included. Please report bugs through the linked GitHub issue forms.

## Screenshot plan

Use actual in-game captures of the accepted version, not simulated renders.

1. Main wheel: a selected phrase with full preview, channel color and controller footer visible. Caption: "Choose a destination with the left stick and a phrase with the right stick."
2. Settings: rotation checkboxes with Everyday, Dungeon Tank and Campfire included. Caption: "Keep your favorite wheels in rotation."
3. Custom wheel: show Custom - Casual and its eight phrase slots. Caption: "Create your own eight-phrase wheels."

Crop for legibility while leaving enough game context to show placement. Hide or redact unrelated chat and private details. Inspect the approved logo at thumbnail size.

## Upload gate and post-upload work

- Confirm current available client using GetBuildInfo and confirm rc.8 works on that exact build. The reported prior acceptance does not establish compatibility with a later patch.
- Inspect the actual CurseForge author-console flavor/version choices. Forever app support does not prove a particular upload tag exists.
- Verify ZIP hash, folder structure, author, LICENSE and version against the chosen artifact.
- Attach approved logo and real screenshots.
- Keep the RC suffix and Beta classification.
- Do not wait for battleground acceptance to distribute this candidate with its stated limitations.
- Upload only after the final compatibility/tag check and publication authorization.
- After approval, add the actual verified CurseForge download URL to the support README and guide.
- Monitor reports; new artifacts receive new versions.

## Sources for submission preparation

- https://support.curseforge.com/support/solutions/articles/9000197241-creating-and-submitting-a-project
- https://support.curseforge.com/support/solutions/articles/9000197242
- https://blog.curseforge.com/app-release-notes-1-321/
- https://worldofwarcraft.blizzard.com/en-us/news/24304160

The newer File & Project Types guidance allows an approved Beta or Release for a new project to sync to the app; testers must opt into Beta files. The older project-submission article still says a Release file is required, so verify actual beta visibility after approval rather than relabeling an RC as stable.
