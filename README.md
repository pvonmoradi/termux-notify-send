Description
-----------
Many shell scripts utilize `notify-send` command which depending
on the desktop environment and notification server, presents a notification
balloon to the user.

In [termux-api-package](https://github.com/termux/termux-api-package), there is
a
[termux-notification](https://github.com/termux/termux-api-package/blob/master/scripts/termux-notification.in)
script which uses Android's notification server.

`notify-send` is a POSIX sh wrapper over that script which mimics
[freedesktop](https://specifications.freedesktop.org/notification-spec/notification-spec-latest.html)
notify-send [CLI](https://ss64.com/bash/notify-send.html) so one should not need
to install X to issue notifications in a Termux environment.

Installation
------------
Put the script somewhere in `$PATH` and make it executable (`chmod +x
/path/to/script`)

Development
-----------
- linter   : `shellcheck`
- formatter: `shfmt -i 4 -bn -ci -sr`
- TODOs are in the script itself
