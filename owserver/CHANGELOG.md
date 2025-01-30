## Changes
- 🆕 Send discovery information to Home Assistant by @epenet in https://github.com/lrybak/hassio-owserver/pull/34 Closes #22 
- 🆕 Support passive USB serial adapter @s-anderss in https://github.com/lrybak/hassio-owserver/pull/35 Closes #33 
- ⬆️ Update hassio-addons/addon-base to v16.3.6
- 🛠️ Update service management to handle dependencies correctly by migrating from the legacy system to the s6-rc way.
- 🛠️ Resolved segmentation fault issues during image builds by switching the base image of action: docker/setup-qemu-action to tonistiigi/binfmt:qemu-v8.1.5. The default latest image, previously used, was causing segfaults (see [tonistiigi/binfmt#215](https://github.com/tonistiigi/binfmt/issues/215)).