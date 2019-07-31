# Sublime

[![N](https://img.shields.io/badge/%F0%9F%91%8D%F0%9F%8F%BE-NetOperatorWibby/Sublime-07d0eb.svg?style=flat-square)](https://code.webb.page/NetOperatorWibby/Sublime)
> My [Sublime Text](https://www.sublimetext.com) setup



### Introduction

[Package Control](https://packagecontrol.io/installation) needs to be installed on first boot. For Sublime Text 3, the installation script for PC is:

```
import urllib.request,os,hashlib; h = '6f4c264a24d933ce70df5dedcf1dcaee' + 'ebe013ee18cced0ef93d5f746d80ef60'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```

Open ST's console by visiting `View > Show Console`.



### Typeface

Input Mono is one of my favorite typefaces to code in. The version included in this repo is customized. I forget the parameters I chose but you can [create your own here](http://input.fontbureau.com/preview). Slashed zero is best zero.



### Sublime Settings

These files should be placed in `~/Library/Application Support/Sublime Text 3/Packages/User/` after Package Control is installed. Note that I am unsure if the settings files will get overwritten if done this way (the packages wouldn't be installed yet).

- `Color Highlight.sublime-settings`
- `Package Control.sublime-settings`
- `Preferences.sublime-settings`
- `SublimeLinter.sublime-settings`

Alternative method:

- `Preferences > Settings`
  - paste the contents of `Preferences.sublime-settings`.
- `Preferences > Package Settings > Package Control > Settings — User`
  - paste the contents of `Package Control.sublime-settings`

At this point, you will have to restart the app to get packages to install. Wait a couple seconds upon startup and tabs will appear, indicating packages were installed.

Now, you can update the other packages with their settings files!
- `Preferences > Package Settings > Color Highlight Settings`
  - paste the contents of `Color Highlight.sublime-settings`
- `Preferences > Package Settings > SublimeLinter > Settings`
  - find your Node path via `which node`
  - paste the contents of `SublimeLinter.sublime-settings`
