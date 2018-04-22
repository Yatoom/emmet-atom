# Simplified Emmet plugin Atom editor

This is a fork of the [emmet-atom](https://github.com/emmetio/emmet-atom) package, and its main goal is to solve the keybinding conflicts with Atom itself that existed in the original package. The original package overwrote keybindings such as the <kbd>ctrl</kbd> + <kbd>shift</kbd> + <kbd>M</kbd> for toggling the Markdown preview, the <kbd>ctrl</kbd> +  <kbd>,</kbd> for opening the Settings View, and <kbd>tab</kbd> for [Atom's autocomplete](http://blog.atom.io/2015/05/15/new-autocomplete.html)

To solve these keybinding conflicts, the number of default keybindings is reduced to one, keeping the most important feature: expanding Emmet-style abbreviations. This feature is given a new unique key binding. For example:

```css
ul>li.item$@-3*5
```

is transformed into

```html
<ul>
    <li class="item7"></li>
    <li class="item6"></li>
    <li class="item5"></li>
    <li class="item4"></li>
    <li class="item3"></li>
</ul>
```
using the <kbd>shift</kbd> + <kbd>space</kbd> key combination.

This plugin will occasionally be synced with its upstream repository when new updates arrive. Furthermore, as a bonus, emmet expanding can also be triggered inside files with PHP, JS and JSX files. For JSX files, the package `language-babel` must be installed too, to make Atom recognize `.jsx` files.

All functionality of the emmet-atom package is still here, which means that you have the freedom to manually add any other Emmet triggers you want. To do so, go to _Edit_ > _Keymap..._ (or _Settings_ > _Keybindings_ > _your keymap file_) and refer to the [original default emmet-atom keymap](https://github.com/emmetio/emmet-atom/blob/master/keymaps/emmet.cson) for a complete list of commands.

Note that you could also just enable emmet expanding everywhere, by opening your keymap (_Edit > Open Your Keymap_) and adding the following piece of text:

```
'atom-text-editor:not([mini])':
   'shift-space': 'emmet:expand-abbreviation-with-tab'
```

### Installation
In Atom, open Preferences > Packages, search for the `emmet-simplified` package. Once found, click install to install package. Alternatively, you could run `apm install emmet-simplified`.

### Manual installation

You can install the latest emmet-simplified version manually from console:

```bash
cd ~/.atom/packages
git clone https://github.com/Yatoom/emmet-atom-simplified emmet-simplified
cd emmet-simplified
npm install
```

Then restart Atom editor.

## Features:

* Expand abbreviations with <kbd>shift</kbd> + <kbd>space</kbd>.

## Default Keybindings

You can disable these in Preferences > Emmet.

Command | Darwin | Linux/Windows
------- | ------ | -------------
Expand Abbreviation | <kbd>shift</kbd> + <kbd>space</kbd> | <kbd>shift</kbd> + <kbd>space</kbd>
