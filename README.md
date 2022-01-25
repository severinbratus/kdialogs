## ranger-kdialog

A script to pick files and directories with `ranger` in chromium-based browsers. Because the default `GtkFileChooser` is [unaesthetic](https://github.com/lxqt/lxqt/issues/1314#issuecomment-460261180) and does not have the keybindings. The script can be easily adapted for `nnn`.

The idea is to impersonate `kdialog`, and implement their interface.

### Installation

- Place `kdialog` as `/usr/local/bin/kdialog`.
- Set `XDG_CURRENT_DESKTOP=KDE`.
- Make sure that arguments are passed correctly to your `$TERMINAL` of choice.

### Issues

- No way to cancel directory selection (and thus download), because in `ranger` a directory is selected by quitting.
- Not possible to set the name of the saved file.
- No option to download a webpage in full, with css, js, etc.
- No mime filtering.
