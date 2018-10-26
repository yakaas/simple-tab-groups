# [![](https://rawgit.com/Drive4ik/simple-tab-groups/master/addon/src/icons/icon.svg)](https://addons.mozilla.org/firefox/addon/simple-tab-groups/ "Simple Tab Groups addon page") Simple Tab Groups

[![Mozilla Add-on](https://img.shields.io/amo/v/simple-tab-groups.svg)](https://addons.mozilla.org/firefox/addon/simple-tab-groups/) [![](https://img.shields.io/amo/d/simple-tab-groups.svg)](https://addons.mozilla.org/firefox/addon/simple-tab-groups/statistics/?last=365) [![](https://img.shields.io/amo/users/simple-tab-groups.svg)](https://addons.mozilla.org/firefox/addon/simple-tab-groups/statistics/usage/?last=365) [![](https://img.shields.io/amo/rating/simple-tab-groups.svg)](https://addons.mozilla.org/firefox/addon/simple-tab-groups/reviews/)

[![https://addons.mozilla.org/firefox/addon/simple-tab-groups/](https://addons.cdn.mozilla.net/static/img/addons-buttons/AMO-button_2.png)](https://addons.mozilla.org/firefox/addon/simple-tab-groups/)

## Translations

Please, help me [translate this addon](https://drive4ik.github.io/simple-tab-groups/translate/index.html) into your language!

## Usage

```bash
$ cd addon
$ npm install
$ npm run build
```

### `npm run build`

Build the extension into `addon/dist` folder for **development**.

### `npm run build:prod`

Build the extension into `addon/dist` folder for **production**.

### `npm run watch`

Watch for modifications then run `npm run build`.

### `npm run watch:prod`

Watch for modifications then run `npm run build:prod`.

### `npm run build-zip`

Build a zip file following this format `<name>-v<version>-(dev|prod).zip`, by reading `name` and `version` from `manifest.json` file.
Zip file is located in `dist-zip` folder.


## Description

Simple Tab Groups works across browser instances/windows too. If you select a group in another window, the selected window will jump to the foreground with the chosen group selected. You can even select the specific tab within that group in background browser windows. GIF example

This allows for easy switching between active and pre-loaded tabs across multiple browser windows.

### This extension has these plugins:

 * [Create new group](https://addons.mozilla.org/firefox/addon/stg-plugin-create-new-group/)
 * [Load custom group](https://addons.mozilla.org/firefox/addon/stg-plugin-load-custom-group/)
 * [Open Manage groups](https://addons.mozilla.org/firefox/addon/stg-plugin-open-manage-groups/)

**NEW** Allow support message actions from Gesturify addon.

**NEW** Allow import groups from addons "Panorama View" and "Sync Tab Groups".

[Preview: how to configure the work with the plugin Gesturefy](https://user-images.githubusercontent.com/7843031/44263498-dffb1b00-a227-11e8-95c7-1b9474199ef0.png)

Supported actions:
 * add-new-group
 * load-first-group
 * load-last-group
 * load-next-group
 * load-prev-group
 * load-custom-group
 * delete-current-group
 * open-manage-groups
 * move-active-tab-to-custom-group

This extension may conflict with other programs similar in functionality.
Conflicted addons:
 * Tab Open/Close Control
 * Panorama View (etc.)

Open popup shortcut: `F8`. You can change this hotkey in addon options.

Current list of functionality / development notes:

 * New Design (fork old add-on design "Tab Groups")
 * Added colored group icon
 * Added the ability to import the backup groups of the old plug-in "Tab Groups"
 * Added support of "Firefox Multi-Account Containers"
 * Now fully supports multiple windows
 * Saves last active tab after change group
 * Show currently used group in addon icon (see screenshot)
 * Specially NOT supported Private (Incognito) Mode
 * Added close tab by middle mouse click
 * Added simple switching between groups and tabs in search mode using the up, down, right and left keys
 * "Manage groups" functional is here! (so far only "Grid")
 * Added support Drag&Drop for tabs and groups in popup window
 * Added support sorting groups (context menu in popup window)
 * Added field for search/filter tabs in "Manage Groups"
 * Added support to Backup/Restore tabs, groups and settings to/from json file
 * Custom group icons, set group icon from tab icon (by context menu)
 * Added undo remove group by context menu browser button (see in screenshots)
 * Added support for catch tabs by containers (#76)
 * Implement hide tabs api
 * **NEW! Added dark theme**
 * Added more settings :)


Permissions used:
 * **tabs**: for tab handling
 * **tabHide**: for hide tabs
 * **<all_urls>(Access your data for all websites)**: for tab thumbnails
 * **contextualIdentities & cookies**: for work with Firefox Multi-Account Containers
 * **notifications**: for notification on move tab to group etc.
 * **menus**: for creating tabs context menus
 * **sessions**: for save session data (last used group, etc)
 * **downloads**: for create auto backups
 * **storage**: for saving groups localy
 * **unlimitedStorage**: for save tab thumbnails

## License and Credits

This project is licensed under the terms of the [Mozilla Public License 2.0](LICENSE).
