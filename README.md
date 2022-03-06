## kdialogs

Scripts to pick files and directories with `nnn` or `ranger` in chromium-based browsers. Because the default `GtkFileChooser` is [unaesthetic](https://github.com/lxqt/lxqt/issues/1314#issuecomment-460261180) and does not have the keybindings.

The idea is to impersonate `kdialog` and implement their interface, `kdialog` being the file-picker dialog that pops up if `XDG_CURRENT_DESKTOP=KDE` is set.

### Installation

- Place `nnn-kdialog` or `ranger-kdialog` as `/usr/local/bin/kdialog`.
- Set `XDG_CURRENT_DESKTOP=KDE`.
- Make sure that arguments are passed correctly to your `$TERMINAL` of choice.

### Issues

`ranger`:
- No way to cancel directory selection (and thus download), because in `ranger` a directory is selected by quitting.
- Not possible to set the name of the saved file.

`nnn` and `ranger`:
- No option to download a webpage in full, with css, js, etc.
- No mime filtering.
- No way to select multiple files.

### nnn-kialog

Being my preference, `nnn-kdialog` has more features (for better or worse), namely:
- Default download directory
- Ability to set the filename with `dmenu`
