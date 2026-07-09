## Before upgrading Calagopus

The panel will be **briefly unavailable** while the new version installs and the service restarts. Plan accordingly if game servers are actively being used — active sessions will be interrupted but running game servers managed by Wings will **not** be affected.

**No manual steps are required.** The upgrade fetches the latest `calagopus-panel` package from the APT repository, re-renders the configuration, and restarts the service automatically.

If you have manually edited `/etc/calagopus/.env`, those changes will be backed up by YunoHost but the file will be overwritten with the rendered template. Move any custom values into YunoHost app settings before upgrading.
