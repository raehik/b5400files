Ethernet
--------

Default `r8169` driver doesn't work. Download the `r8168` package from Arch
repos and blacklist the incorrect one:

```text
[/etc/modprobe.d/r8169.conf]
blacklist r8169
```

EDIT: Actually, I'm not so sure. Looks like I blacklisted `rtl8169` years ago,
but it was loaded anyway? And so was r8168? Dunno.
