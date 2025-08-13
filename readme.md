# [Firefox Sidebar (w/ Dynamic Indentation)](https://codeberg.org/macleod/FirefoxSidebar)

**As GitHub is now officially just a Microsoft Copilot feeder *product* instead of a universal, global,  code repository, we have migrated this project to Codeberg, a non-profit.**

While we understand that companies and organizations inevitably use our **public** code anywhere to seed their models, we would prefer not directly helping the organizations do it on the platform of their choosing, and make them work just a *smidge* harder to get it. As GH also hosts the most number of private repositories, there is an ethical issue with allowing any of our code reside here, public or not. 

## **[ :: All new releases will be found here :: ](https://codeberg.org/macleod/FirefoxSidebar)**

***TO SET YOUR NEW ORIGIN URL, USE THE FOLLOWING COMMAND:***

```
git remote set-url origin https://codeberg.org/macleod/FirefoxSidebar.git
```

Previous readme with updated (git) instructions:

---

# Firefox Sidebar (w/ Dynamic Indentation)


## Features:

  - Longest lasting, oldest, and possibly first, major dynamic Firefox sidebar w/ regular updates.
  - *Dynamic Indentation*: Unfurls tab names and indentations on hover of the sidebar, saving you space while you browse.
  - Native Vertical Tabs: Now built on top of the native Firefox vertical tab system.
  - Tree style tabs: Tree style tab support by using Sidebery & TreeStyleTabs (legacy)
  - Automatic themes: Automatically matches your Firefox theme colors!
  - Custom theming: Custom theme configuration using Sidebery, or any other
  - Tab Power Features: Tab groups and tab containers (both with visual identifiers), bookmarks, history, and more.
  - Pinned Tabs: Pinned tabs stay at the top (right click to close)
  - Sidebar Switching: switch between different sidebars by hovering over the switcher at the bottom.
  - Cross-Platform: Should work on Windows, Linux, and Mac. 

**Note as of 2025.02.09**: This is now using (and replaces!) the new built in Firefox 134+ vertical tabs, make sure you have updated. If you are still on an older version of Firefox, please check the releases page for the older versions. 

# Instructions (guide/setup)

The instructions may seem like quite a lot, but the entire proces takes less than a few minutes and does not require you to be overly technical. Most guides will entirely skip the first three main steps and expect you to know what you are doing, I don't, so I hope this helps as much as possible.

1. Activate vertical tabs and install sidebery:
    1. Right click on any open space on the tab bar
    2. Select "Turn on vertical tabs"
    3. [Install Sidebery from Firefox Addons](https://addons.mozilla.org/en-US/firefox/addon/sidebery/)

2. Allow modifying your Firefox appearance:
    1. In Firefox navigate to `about:config` in your address bar
    2. Search for `toolkit.legacyUserProfileCustomizations.stylesheets`
    3. Double click or manually change this to `true`

3. Add the FirefoxSidebar settings:
    1. Navigate to `(about:profiles)`in your address bar
    2. Click on the `open root folder` button for your current profile
    3. Open this folder location in your terminal
    4. Clone this repo with the following command: `git clone https://codeberg.org/dxfiers/FirefoxSidebar "chrome"`
        1. *You may need to install `git` for this to work* -> [Git Downloads](https://git-scm.com/downloads)
        2. If installing `git` is not possible, then download the latest `Source Code (zip)` files from [Releases](https://codeberg.org/macleod/FirefoxSidebar/releases), create a folder called `chrome` inside your current profile, unzip and move the files into that folder.

4. Load the custom Sidebery theme and settings *(optional, suggested!)*:
    1. Navigate to Sidebery settings (Right click on the Sidebery extension icon > "Open Settings")
    2. Click on "Help" in the sidebar (Settings > Help)
    3. Click on "Import addon data"
    4. Select and load the `sidebery-data.json` file located in your 'chrome' folder from step 3.

5. Restart Firefox, and click on the 'Sidebery' extension, everything should now be working as expected. 

# FAQ 

## Sidebery Themes

If you dislike any of the theme presets for dark or light themes, or you have a particular color scheme in mind then navigate to `Sidebery Settings > Style Editor` (found at the end of the settings sidebar).

## Custom Modifications

Add any additional Firefox modifications into `custom.css`, these will not be overwritten on future sidebar updates (when using `git pull`)

Visit [userchrome.org](https://www.userchrome.org/how-create-userchrome-css.html) if you have any questions.

## TreeStyleTabs (Legacy)

Either add the firefox/treestyletabs.css to your TST addon preferences or import the treestyletabs-\*.json preferences to your TST addon.

This is a legacy support theme and not often changed. 

## Updates

Release notes have migrated to [here](https://codeberg.org/macleod/FirefoxSidebar/releases). 
