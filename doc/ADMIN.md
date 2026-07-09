# Post-installation instructions

Calagopus is now running at `https://__DOMAIN____PATH__`.

## First-time setup

Open the URL above in your browser. You will be greeted by the **Out-Of-Box Experience (OOBE)** wizard, which lets you:

1. Create the first administrator account.
2. Configure global settings (SMTP, branding, etc.).
3. Add your first Wings node to start hosting game servers.

## Adding a Wings node

Calagopus requires at least one **Wings** daemon running on a Linux host to actually launch game servers. The panel itself only manages configuration — Wings is what runs the containers.

Install Wings on a separate Linux server (or the same host for a single-node setup) by following the [official Wings documentation](https://calagopus.com/docs/wings/installation).

## Environment file

The panel's configuration lives at `/etc/calagopus/.env`.  
**Do not edit it by hand** — YunoHost will overwrite it on the next upgrade. Use the YunoHost admin panel or re-run `yunohost app config set calagopus` if you need to change a setting.

## Logs

Application logs are written to `/var/log/__APP__/__APP__.log` and are rotated automatically by logrotate.
