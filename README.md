# **asciitoart**

```
 ______                              ______            ______         __
/\  _  \                  __  __    /\__  _\          /\  _  \       /\ \__
\ \ \L\ \    ____    ___ /\_\/\_\   \/_/\ \/   ___    \ \ \L\ \  _ __\ \ ,_\
 \ \  __ \  /',__\  /'___\/\ \/\ \     \ \ \  / __`\   \ \  __ \/\`'__\ \ \/
  \ \ \/\ \/\__, `\/\ \__/\ \ \ \ \     \ \ \/\ \L\ \   \ \ \/\ \ \ \/ \ \ \_
   \ \_\ \_\/\____/\ \____\\ \_\ \_\     \ \_\ \____/    \ \_\ \_\ \_\  \ \__\
    \/_/\/_/\/___/  \/____/ \/_/\/_/      \/_/\/___/      \/_/\/_/\/_/   \/__/

```

## **Synopsis**


python. It takes text and renders it in ASCII art fonts (like
the title above, which is the 'larry3d' font).


## **Usage**

You can use asciitoart in one of two ways. First, as commandline and as a library ,
Run with `--help` to see a full list of tweaks.  Mostly you will only
use `-f` to change the font. It defaults to standard.flf.

### commandline

```
asciitoart 'text to render'
asciitoart "Ascii" -f ansi_shadow
asciitoart "Ascii" -f big_money-ne -c cyan
asciitoart "Ascii" -f big_money-se -c black:light_blue
```


### asciitoart is also a library that can be used in python code:

```py
from asciitoart import AsciitoArt
f = AsciitoArt(font='ansi_shadow')
print(f.renderText('text to render'))
```

or

```py
import asciitoart
f = asciitoart.asciitoart_format("text to render",font="slant")
print(f)
```

If you have found some new fonts that you want to use, you can use the
command line interface to install your font file as follows:

`asciitoart -L <font file>`

The font file can be a ZIP file of lots of fonts or just a single font.
Depending on how you installed asciitoart, you may find that you need
root access to install the font - e.g. `sudo asciitoart -L <font file>`.


## **License**
The MIT License (MIT)
Copyright © 2007-2023
(see LICENSE for full details)