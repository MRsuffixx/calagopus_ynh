## Before you install Calagopus

**This package installs the Calagopus Panel only.**

To host game servers, you will also need to install **Wings** on at least one Linux host after the panel is set up. Wings is the daemon that runs and manages game server containers. Installation instructions are available in the [Calagopus documentation](https://calagopus.com/docs/wings/installation).

**Requirements:**
- A dedicated domain or sub-domain is recommended (e.g. `panel.yourdomain.tld`)
- At least **512 MB RAM** available at runtime (1 GB recommended)
- At least **1 GB free disk space**
- Architecture: **amd64** or **arm64** only

**Important:** The `APP_ENCRYPTION_KEY` generated during installation is used to protect sensitive data stored in the database. **Do not lose this key** — it cannot be recovered and rotating it requires re-encrypting all stored secrets.
