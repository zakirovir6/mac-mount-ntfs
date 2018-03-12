# mac-mount-ntfs
A little script which mounts ntfs disks in rw mode on macos high sierra.

To use it you must install **osxfuse** and **ntfs-3g** for example with [homebrew](brew.sh).
```
$ brew cask install osxfuse
$ brew install ntfs-3g
```
After that put ntfs-mount under your **PATH** env variable, exec it `$ ntfs-mount` and follow the instructions. You will be offered to type a device identifier. You can get it from the output of `$ diskutil list` which also will be shown you. Sudo is required for `umount` and `mount` operations.
