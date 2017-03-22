vscode-autoupdate
=================

This script allows easy update of Visual Studio Code from Microsoft as package
is not included in any repository.

To run it simply type:
```bash
./vscode-autoupdate
```

It is required to run it in elevated privileges mode (`sudo` or as root) so if
you are using it as a normal user type:
```bash
sudo ./vscode-autoupdate
```

It is also possible to run it in cron - for instance if you wish to autoupdate
`vscode` every day at 11:00 you can enter in your root's crontab:
```
0 11 * * * /opt/vscode-autoupdate/vscode-autoupdate > /dev/null 2>&1 || true
```
(entry above will work only if you put your files in `/opt/vscode-autoupdate`).

Warning: be sure to set it for root's crontab or edit your sudoers file!

installation
============

Place files in desired folder and grant execution permissions:
```bash
chmod +x vscode-autoupdate
```

PHP 5.3 or above is required.
