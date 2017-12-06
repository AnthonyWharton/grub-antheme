# Grub Antheme

This is a little GRUB2 theme that I conjured up one afternoon when procrastinating. It was developed on a Dell XPS 13, with the crazy QHD 3200x1800 screen. This means this theme is optimised for 16:9 HiDPI screens, and may look a bit funny on smaller screens.

Nevertheless, at some point I may update it and make it a bit more portable, but for the time being it is what it is, and you can take from it as much or as little as you'd like.

## Installation

To install this theme, simply copy these files into your GRUB2 themes folder. This is usually something like:

```
/boot/grub/themes/antheme/
```

Note that you may need root permissions as it's generally good practise to have a locked down `boot` partition. Thus a cheeky `sudo su` may be in order, however if you do this and start poking around your boot folder, be careful!

Once the files are copied in, with your favourite editor, find:

```
vim /etc/default/grub
```

And find a line starting with `GRUB_THEME`, and modify it to show the path you put the theme at:

```
GRUB_THEME="/boot/grub/themes/antheme/theme.txt"
```

*Note: If you didn't find a `GRUB_THEME` line then add it in yourself! Go on, I believe in you!*

Finally now that this is done, now run (as root) `grub-mkconfig` and output it where your grub config lies, I've listed where it is for me below:

```
# grub-mkconfig -o /boot/grub/grub.cfg
```

And you're done! Probably.. You may find on a HiDPI screen that your fonts are funny, because I didn't include any fonts within this theme (yet). I'll write up some help for this in the future, and if I've forgotten then raise an issue!

## Licensing

> It's MIT, do whatever you want. HOWEVER, please note that the background and icons have been sourced from around the internet a long time ago and were just on my computer. Please note that I am not the author for these documents.
