# Firefox Sidebar (Edge-Like Vertical Tabs)

**Note as of 2025.02.09:** 

This version is now available in atleast the developer-edition, unknown in stable. The actition of the new native vertical tab subsystem is now even easier, the instructions below are updated. **This overrides the default vertical tab subsystem, replaces it with Sidebery (or TST), and allows for *dynamic indentation*.   

- This is now using (and replaces!) the new built in Firefox 134<?)+  vertical tabs, make sure you are updated. 
- This allows you to replace it with any of your preferred vertical tab extension options:
    - Sidebery (preferred), TreeStyleTabs, etc. 
- If you are still on an older version of Firefox, please check the releases page for the older versions. 

## Example

https://user-images.githubusercontent.com/4322153/205100497-f56637c4-1d46-4c15-b349-d0b53f2838a0.mp4

Note: This is an older version, but the effect and design is still roughly the same.

## Features:

  - Edge-like vertical tab design
  - Tree style tab layout support (works with Sideberry & TST)
  - *Dynamic Indentation*
  - Automatic theme configuration for light and dark themes
  - Custom theme configuration using Sidebery, or any other. 
  - Support for tab groups
  - Support for Tab Containers with visual identification
  - Pinned tabs (right click to close)
  - Simplified design (smallest compared to any other) by using Firefox 133, for older versions.
  - Longest lasting and oldest (and first?) major dynamic firefox sidebar extension w/ regular updates. 

# Instructions (setup)

To use FirefoxSidebar you will need to clone this repo into your Firefox profile as the `chrome` folder and then follow the Sideberry section below. Both are outlined below in how to do so.

1. Activate experimental sidebar 
    1. Right click on any open space on the tab bar
    2. Select "Turn on vertical tabs"
    
2. Update userChrome.css 
    1. Navigate to [about:profiles](about:profiles) `(about:profiles)`in your address bar
    2. Click on the 'open root folder` button for your current profile
    3. Open this folder in your terminal
    4. Clone this repo with the following command: `git clone https://github.com/wizrdsh/FirefoxSidebar.git "chrome"`

3. Activate userChrome.css modification flag
    1. In Firefox navigate to [about:config](about:config) in your address bar
    2. Search for the characteristic `toolkit.legacyUserProfileCustomizations.stylesheets`
    3. Double click, or change this to `true`
    4. Restart Firefox

You could skip the clone step entirely if you manually add the FirefoxSidebar files to the "chrome" folder in your Firefox Profile (you will need to make a `chrome` folder if it doesn't exist!).

Visit [userchrome.org](https://www.userchrome.org/how-create-userchrome-css.html) if you have any questions.

4. Load the custom sidebery theme and settings (optional, suggested!)
    1. Navigate to sidebery settings - [moz-extension://d6dfc617-d672-45b6-8293-f37e07a55dce/page.setup/setup.html#settings_appearance](moz-extension://d6dfc617-d672-45b6-8293-f37e07a55dce/page.setup/setup.html#settings_appearance)
    2. Click on "Help" in the sidebar 
    3. Click on "Import addon data"
    4. Load the `sidebery-data.json` file

If you dislike any of the theme presets for dark or light themes, or you have a particular color scheme in mind then navigate to Sideberry Settings > Style Editor (found at the end of the settings sidebar). The preference is to replace the values in the right panel, not in the theme editor to the left - this way you can easily update to newer versions in the future.

## How to use 

1. Follow the installation instructions above
2. To switch your sidebar choice, hover over the bottom "settings" icon in the sidebar. 


## Custom Modifications

Add any additional Firefox modifications into `custom.css`, these will not be overwritten on future sidebar updates.

## Extensions  & Preferences

These have been removed as of v2.2025.01.07. 

## TreeStyleTabs (Legacy)

Either add the firefox/treestyletabs.css to your TST addon preferences or import the treestyletabs-\*.json preferences to your TST addon.

## Updates

Release notes have migrated to [here](https://github.com/wizrdsh/FirefoxSidebar/releases). You can find prior release notes before v12021.12.22 [here](https://github.com/wizrdsh/FirefoxSidebar/releases/tag/v12021.12.22).
