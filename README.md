# Simplified Emmet plugin Atom editor

[Emmet](http://emmet.io) support for [Atom](http://atom.io). This is a fork of the emmet-atom package. It has one key-binding, and one key-binding only: the <kbd>shift</kbd> + <kbd>space</kbd> key for emmet expanding. This solves all keybinding conflicts with the Atom Core, such as the <kbd>ctrl</kbd> + <kbd>shift</kbd> + <kbd>M</kbd> for toggling the Markdown preview, the <kbd>ctrl</kbd> +  <kbd>,</kbd> for opening the Settings View, and recently <kbd>tab</kbd> for [Atom's new autocomplete](http://blog.atom.io/2015/05/15/new-autocomplete.html).

Other than that, there are - as of yet - no differences with emmet-atom, which means that you have the freedom to manually add any other Emmet triggers you want. To do so, go to _Edit_ > _Open Your Keymap_ and refer to the [original default emmet-atom keymap](https://github.com/emmetio/emmet-atom/blob/master/keymaps/emmet.cson) for a complete list of commands.

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

* Expand abbreviations by <kbd>shift</kbd> + <kbd>space</kbd>.

## Shift-space key

Simplified Emmet expands abbreviations by shift-space key only for HTML, CSS, Sass/SCSS and LESS syntaxes.

## Default Keybindings

You can change these Preferences > Emmet.

Command | Darwin | Linux/Windows
------- | ------ | -------------
Expand Abbreviation | <kbd>shift</kbd> + <kbd>space</kbd> | <kbd>shift</kbd> + <kbd>space</kbd>
