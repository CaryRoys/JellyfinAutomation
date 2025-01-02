# JellyfinAutomation

Cary's repo for storing various useful bits of automation related to running your own Jellyfin server on Windows.

`JellyFinRestHelper.ps1` - the functions as detailed on this blog post: https://medium.com/@caryroys/a-working-example-of-jellyfin-automation-196d72bf4542

`upgrade-jellyfinserver.ps1` - An auto-upgrade script for Jellyfin on AMD64 (the only platform with a NSIS installer) - mean to be registered with -register parameter, and then it will check weekly for new versions.  Note that I've observed an error regarding service startup which hangs the upgrade.  I'm not sure if this happens every time, but it appears to originate from nssm.exe helper executable.  I'm unsure of the proper workaround for now - but once solved, the auto-upgrade should be very reliable.
