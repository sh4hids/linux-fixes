# linux-fixes

#### `nouveau 0000:01:00.0: bus: MMIO read of 00000000 FAULT at 6013d4 [ IBUS ]`

Replace `GRUB_CMDLINE_LINUX_DEFAULT="quiet splash"` on `/etc/default/grub` with:
```bash
GRUB_CMDLINE_LINUX_DEFAULT="quiet splash nomodeset"
```
