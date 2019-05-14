# Info
Template files for Linux Systemd.

# Usage

1. Fill your template accordingly.
2. `sudo cp your-service-file.service /lib/systemd/system`
3. `sudo systemctl daemon-reload` this should be run everytime `.service` file is modified
4. `sudo systemctl enable your-service-file`
5. `sudo systemctl start your-service-file`

# Status of your service

`systemctl status your-service-file`

# Logs

1. From start: `journalctl -u your-service-file`
2. From end (reverse): `journalctl -u your-service-file -r`
3. Live feed: `journalctl -u your-service-file -f`
