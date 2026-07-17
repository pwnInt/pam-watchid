PAM WatchID
-----------
A PAM plugin for authenticating using the new kLAPolicyDeviceOwnerAuthenticationWithBiometricsOrWatch API in macOS 10.15, written in Swift.

Would help when running on a MacBook with lid closed.

This is for **Apple Silicon devices** with **macOS 11+** only.

`TARGET = arm64-apple-macos11`

<details>
<summary>demo</summary>
  
![](demo.gif)
</details>

Installation
------------

1. `$ sudo make install`

~~2. Edit `/etc/pam.d/sudo` to include as the first line: `auth sufficient pam_watchid.so "reason=execute a command as root"`~~

_Note that you might have other `auth`, don't remove them._
