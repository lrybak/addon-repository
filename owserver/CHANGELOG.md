### Changes
This change aims to update the add-on installation process. Currently, users have to manually add the repository https://github.com/lrybak/hassio-owserver/ to install the add-on.

With this pull request, three new repositories are introduced:

https://github.com/lrybak/addon-repository - containing stable releases of the add-on, which is recommended for most users.
https://github.com/lrybak/addon-repository-beta - containing release candidate versions of the add-on, which is recommended only for those who want to test new features.
https://github.com/lrybak/addon-repository-edge - containing bleeding edge builds of the add-on, suitable only for development purposes and may be unstable or not work at all.
This change makes it easier to release new updates for the add-on and provides a more streamlined installation process for users.

Please note that the current repository (https://github.com/lrybak/hassio-owserver) will remain up to date until the end of July 2023. After that time, all users will need to switch to the new repositories mentioned above to get updates.

### Breaking change:
After changing add-on repository in Home Assistant, the hostname of add-on will also change. You need to add the 1-wire integration again with the new hostname (simple method) or modify the one already installed integration (advanced method). Please note that the Home Assistant UI does not allow you to change the hostname. To modify an existing integration, edit the .storage/core.config_entries file. It's recommended to have copy of the file before making any changes. After making the change, remember to restart Home Assistant.

**Apart of the above this change brings below changes as well:**
- 🆕  added device type selector (usb)
- 🆕  added debug mode for owserver
- 🆕  added temperature scale selector
- ⚙️ changed auto_uart to uart to get rid of home assistant warning
- 📜 Update docs