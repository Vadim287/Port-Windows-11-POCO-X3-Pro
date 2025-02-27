# Uninstall Windows and revert your POCO X3 Pro to stock

## Why is this needed?

If you want to uninstall Windows, this is used instead of deleting partitions manually to avoid human error + writing a whole dedicated guide to just uninstalling.

If you want to relock your bootloader you'll need your partition table to be stock.

### Files/Tools Needed

- [ADB & Fastboot](https://developer.android.com/studio/releases/platform-tools)

Modified TWRP:

| File Name                                       | Android version |
|-------------------------------------------------|-----------------|
| [twrp-3.7.1_vap.img](https://github.com/woa-vayu/POCOX3Pro-Guides/releases/download/twrp/twrp-3.7.1_vap.img) | Android 12/12.1/13/14/15 |

## Flash and boot modified recovery

```cmd
fastboot flash recovery path\to\moddedtwrp.img reboot recovery
```

### Execute the restore script

```cmd
adb shell restore
```

#### Finished
