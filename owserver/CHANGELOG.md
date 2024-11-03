## Changes
- 🆕 ⚠️ : Ability to add multiple 1-Wire devices - **breaking change**, requires addon re-configuration. Closes #22 
- ⬆️ Update hassio-addons/addon-base to v15.3.4

### Breaking change: read before you upgrade!

This update introduces the ability to add multiple 1-Wire devices which required changes to to add-on configuration.
Devices now need to be specified as a YAML list. Please refer to the documentation page for more details before you upgrade.