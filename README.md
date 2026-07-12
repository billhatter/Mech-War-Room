# Mech War Room

A Windows-only .NET 10 MAUI roster and reference application. Current release: **0.6.0-beta**.

## Features
- Browser-style named workspaces with isolated roster data, inline renaming, clean **+** creation, archiving/restoration, archive roster viewing, and permanent deletion.
- Startup-gated About this app disclosure with an automatic ten-second transition, randomized 7–14 day quieting, Discord, Patreon, and PayPal.Me links.
- Desktop File/Archives/View/Help menu, explicit Save/Archive/Exit actions, dynamic workspace/archive lists, reusable About page, update checks, and bundled documentation.
- Selectable Sarna.net and BattleTech Wiki on Fandom MediaWiki search with 350 ms debounce, cancellation, predictive suggestions, normalized article data, a controlled article thumbnail with click-to-expand viewing, loading/empty/error/offline states, and provider-specific source links.
- SQLite-backed Pilot/'Mech roster with catalog-backed Chassis/Variant selection, validated CRUD, header sorting, prefix filtering, and inclusive era filtering.
- Collapsible Add/Edit panel and bounded 'Mech Details table optimized for Windows desktop use.
- Original neutral charcoal/steel/copper industrial styling. No franchise artwork or copyrighted visual assets are included.
- Background designer placeholder at View > Backgrounds > Choose Background.

## Installation

Run `Mech-War-Room-0.6.0-beta-win-x64-setup.exe`. The per-user installer requires no administrator privileges and defaults to `%LocalAppData%\Dorian_Blade\Mech War Room\`. It contains the self-contained Release application payload and `USER_MANUAL.md`, creates a Start menu shortcut, offers an optional desktop shortcut, and registers uninstall support.

## Build and test
```bash
dotnet test MechWarriorWarRoom.Tests/MechWarriorWarRoom.Tests.csproj
dotnet build MechWarriorWarRoom/MechWarriorWarRoom.csproj -f net10.0-windows10.0.19041.0 -c Debug
```

## Release history
- [`MVP_CHANGELOG.md`](MVP_CHANGELOG.md) — frozen 0.0.x alpha/MVP history.
- [`BETA_CHANGELOG.md`](BETA_CHANGELOG.md) — active 0.1.x beta history.

## User documentation
- [`USER_MANUAL.md`](USER_MANUAL.md) — end-user guide bundled with the application.

## Architecture documentation
- [`MVP_ARCHITECT_DESIGN.md`](MVP_ARCHITECT_DESIGN.md) — historical 0.0.x alpha/MVP baseline.
- [`BETA_ARCHITECTURE_DESIGN.md`](BETA_ARCHITECTURE_DESIGN.md) — living 0.1.x beta architecture.

## Data and attribution
Article text, search results, and catalog-linked image references come from [Sarna.net BattleTech Wiki](https://www.sarna.net/wiki/Main_Page). Images are loaded remotely for display only and are not bundled or redistributed. Follow each linked Sarna page for content licensing and attribution details.
