# Sublime

[![N](https://img.shields.io/badge/%F0%9F%91%8D%F0%9F%8F%BE-NetOperatorWibby/Sublime-07d0eb.svg?style=flat-square)](https://git.inc.sh/NetOperatorWibby/Sublime)
> My Sublime Text setup



### Introduction

[Package Control](https://packagecontrol.io/installation) needs to be installed on first boot. For Sublime Text 3, the installation script for PC is:

```
import urllib.request,os,hashlib; h = '6f4c264a24d933ce70df5dedcf1dcaee' + 'ebe013ee18cced0ef93d5f746d80ef60'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```

Open ST's console by pressing `Ctrl+\`` or visiting `View > Show Console`.



### Typeface

Input Mono is my coding typeface of choice. The version included in this repo is a customized. I forget the parameters I chose but you can [create your own here](http://input.fontbureau.com/preview). Slashed zero is best zero.



### Sublime Settings

These three files should be placed in `~/Library/Application Support/Sublime Text 3/Packages/User/` after Package Control is installed.

- `Package Control.sublime-settings`
- `Preferences.sublime-settings`
- `SublimeLinter.sublime-settings`
