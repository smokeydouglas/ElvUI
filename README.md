# ElvUI for AzerothCore

This repository maintains a focused ElvUI 6.09 distribution for AzerothCore and World of Warcraft Wrath of the Lich King 3.3.5a.

It is intended for private-server operators and players who need a stable interface for the 3.3.5a client. Changes are kept narrow: fix AzerothCore compatibility problems, preserve the established ElvUI behavior, and avoid importing unrelated rewrites from divergent forks.

## Compatibility

- AzerothCore WotLK
- World of Warcraft 3.3.5a, build 12340
- AddOn interface 30300
- ElvUI 6.09
- ElvUI_OptionsUI 1.06

Modern Battle.net, Retail, and current Classic clients are not supported.

## Changes in this fork

- Druid Cat Form detection uses the localized form name instead of relying on a server-dependent form index.
- The Cat Form lookup is guarded when `GetShapeshiftForm()` returns `0`, preventing an error while the player is unshifted.
- Nameplate castbars initialize their font strings before applying font settings.
- The installer includes a fourth theme named `Modern`, with blue-charcoal surfaces, slate framing, and a restrained blue accent.
- In-game update and support links point to this AzerothCore-focused fork.
- Simplified and Traditional Chinese locale packages are not included.

## Installation

1. Download the ZIP from the [latest release](https://github.com/smokeydouglas/ElvUI/releases/latest).
2. Fully exit World of Warcraft.
3. Back up or remove any existing `Interface/AddOns/ElvUI` and `Interface/AddOns/ElvUI_OptionsUI` folders.
4. Extract the release into `Interface/AddOns`.
5. Confirm that these paths exist:

   ```text
   Interface/AddOns/ElvUI/ElvUI.toc
   Interface/AddOns/ElvUI_OptionsUI/ElvUI_OptionsUI.toc
   ```

6. Enable both addons on the character-select AddOns screen and start the game.

Do not install the repository root as a single addon folder. The client must see the two addon directories separately.

## Configuration

- `/ec` opens the ElvUI configuration.
- `/moveui` unlocks movable frames.
- `/kb` starts keybinding mode.
- `/reload` reloads the interface after configuration changes.

To apply the custom theme, open `/ec`, choose `Install`, advance to Theme Setup, and select `Modern`.

## Reporting a problem

Open an issue in this repository and include:

- the release or commit you installed;
- the AzerothCore revision and enabled server modules;
- confirmation that the client is build 12340;
- exact reproduction steps;
- the full Lua error, if one appears;
- whether the problem remains with only ElvUI and ElvUI_OptionsUI enabled.

Server behavior and addon behavior can look similar. Note whether the client frame rate drops or whether only game actions and movement pause.

## Languages

The distribution includes English, German, Spanish, French, Korean, Portuguese, and Russian locale files. English is the fallback for untranslated strings. zhCN and zhTW packages are intentionally excluded.

## Development

The default branch is `master`. `origin` is the maintained fork and `upstream` tracks [ElvUI-WotLK/ElvUI](https://github.com/ElvUI-WotLK/ElvUI).

Before submitting a change:

```bash
git diff --check
luacheck . -q
```

Keep fixes small and specific to the 3.3.5a/AzerothCore target. Avoid broad merges from server-specific UI rewrites unless each change has been reviewed independently.

## Upstream

This project is based on the ElvUI WotLK backport maintained by ElvUI-WotLK and on the original work of the ElvUI authors and contributors. Upstream project and bundled-library attribution remains in the source tree. This fork is independently maintained and is not an official AzerothCore project.
