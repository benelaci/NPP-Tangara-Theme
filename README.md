# Tangara Theme for Notepad++

![Tangara theme for Notepad++](https://i.ibb.co/GkhPmpn/github-full.jpg)

# Description
Unreasonably thoroughly picked colors to create the neatest color arrangement I can think of.
Designed for the sake of colors rather than for optimal ergonomics while keeping a fair degree of usability.

Unfortunately this particular background color is very different from screen to screen, but should more or less
work on 6000 K screen color temperature (less is greener, more is bluer).

The name refers to the male swallow tanager (fecsketangara in Hungarian), although the theme is actually even
more similar to the blue-brested kingfisher.


# Installation

1. **Click** [`HERE`](https://github.com/benelaci/NPP-Tangara-Theme/archive/refs/heads/main.zip) to download all files in zip.
2. Go to **%APPDATA%\Notepad++**.
3. Open **themes** folder, or create a new folder named **themes** if it doesn't exists.
4. Copy the **.xml** file in the downloaded zip into the folder.
5. Install all font files in the *fonts* folder using one of the following methods:
   - open **Font Settings** (Press `Win` key, and start typing *"font"*) and drag all 4 font files at once.
   - launch the font files one by one, and click **Install**.
6. Restart Notepad++.
7. Open *Settings -> Style Configurator*.
8. Select theme **Tangara** from the theme drop-down box.
9. Click **Save & Close**.

# The thing about fonts

## Why install fonts?

The theme uses four different font weights instead of two to make text bolding more subtle.

Because of this, the theme depends on the four type faces of *Roboto Mono* inside the zip.
In a theme, only two font weights can be used dynamically, i.e. independently of fonts: bold / not bold.
To use more font weights, the exact font face names have to be specified in the theme.

## Whether to use font overrides

Font overrides unbold all text thinner than full bold, which kinda ruins the look of the theme. So **don't use font overrides**, you should stick to the theme font.
Only exception is Markdown language, where I find it useful to replace the bulky monospace font to a more readable sans serif.
**Font override can be used on Markdown.**

## Turn off DirectWrite

Make sure DirectWrite is turned off. (*Settings* -> *Misc* -> [ ] *use DirectWrite*)
![direct write off](https://i.ibb.co/bmGhTDW/github-Direct-Write-off.png)

Primarily because DirectWrite doesn't let the theme use the above mentioned hardcoded font faces for some weird reason. Hopefully this will be fixed in a future version of Notepad++, then I'll probably publish a version of this theme with *Fira Code* font.

----
