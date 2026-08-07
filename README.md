# canary-ortho-q

Variant of the [canary ortho](https://github.com/Apsu/Canary) layout, with two changes:

- W and Q swapped - the pinky is short and W is more common, so having W in the bottom row is more comfortable
- Keep colemak punctuation - not sure why the original canary layout permuted those, doesn't appear beneficial for my use at least

Layout:

```
q l y p b z f o u ;
c r s t g m n e i a
w j v d k x h , . /
```


## XKB (Linux)

To install:

```
sudo cp canary-ortho-q.xkb /usr/share/X11/xkb/symbols/canary-ortho-q
```

To try (X11):

```
setxkbmap canary-ortho-q
```

To set default:

```
sudo localectl set-x11-keymap canary-ortho-q
```


## KBD (Linux TTY)

To try:

```
sudo loadkeys canary-ortho-q.map
```

To set default (Arch Linux):

```
sudo cp canary-ortho-q.map /usr/share/kbd/keymaps/
vim /etc/vconsole.conf
```

-> set `KEYMAP=canary-ortho-q`
