# XIV

Dalamud plugin catalog for [Shadowstar](https://shadowstar.io) FFXIV plugins. Source stays in each plugin repo. This repo is only the installer list.

## Install

In game: `/xlsettings` → **Experimental** → **Custom Plugin Repositories**, add:

```
https://raw.githubusercontent.com/ShadowstarIO/XIV/main/repo.json
```

Save, then `/xlplugins`. Search **LightsOn**, **StatusShift**, or **AndThen**. AndThen is testing only until a stable release, so turn on testing builds in the plugin installer to see it.

Do not also add each plugin’s own `repo.json`. Same `InternalName` in two catalogs duplicates in the installer.

The old `XozaShadow/XIV` URL still redirects. Use this one going forward.

## Plugins

| Plugin | What | Source |
| --- | --- | --- |
| **AndThen** | When conditions match, apply settings and run commands. Testing only. | [AndThen](https://github.com/ShadowstarIO/AndThen) |
| **LightsOn** | Occupancy for listed venues and short outdoor scenes | [LightsOn](https://github.com/ShadowstarIO/LightsOn) |
| **StatusShift** | Online status, search comment, and commands from zone, activity, and schedule | [StatusShift](https://github.com/ShadowstarIO/StatusShift) |

Zips come from each plugin’s GitHub Releases. This file only points at them.

A scheduled Action refreshes `repo.json` from those repos. Run **Sync plugin catalog** on Actions if a release just dropped and the list is stale.
