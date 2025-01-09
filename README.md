# Tangara Theme for Notepad++

![Tangara theme (medium dark) for Notepad++](https://i.ibb.co/vZ1QspX/github-Tangara-theme-for-NPP.png)

# Description

Unreasonably thoroughly picked colors to create the neatest color arrangement I can think of.
Designed for the sake of colors rather than for optimal ergonomics while keeping a fair degree of usability.

The background color is a bit different for each screen, but on a slightly warmer than neutral screen color
temperature it should be roughly as intended.

The name refers to the male swallow tanager (*fecsketangara* in Hungarian), although the theme is actually even
more similar to the blue-brested kingfisher.

# Supported languages

Assembly, Bash, Batch, C, C++, C#, CSS, HTML, INI, Java, JavaScript, Lua, Markdown\*, PHP, Python, Ruby, SQL, XML, YAML  
Everything else is usable but not arranged.  
If the theme gets somewhat popular, I'll optimize more languages. (Especially on request of course.)

> \* For Markdown, read the *Setting up Markdown* section at the bottom of this page.

# Installation

1. **Click** [`HERE`](https://github.com/benelaci/NPP-Tangara-Theme/archive/refs/heads/main.zip) to download all files in zip.
2. Go to **%APPDATA%\Notepad++**.
3. Open **themes** folder, or create a new folder named **themes** if it doesn't exists.
4. Install the xml in any of the following ways:
   - Copy the **.xml** file in the downloaded zip into the folder. Or
	- Import it to Notepad++ by going to *Menu -> Settings -> Import -> Import Style theme(s)*.
5. Install all font files in the *fonts* folder in any of the following ways:
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
Only exception is Markdown language, where I prefer replacing the bulky monospace font to a more readable sans serif.
**Font override can be used on Markdown.**

## Turn off DirectWrite

Make sure DirectWrite is turned off. (*Settings* -> *Misc* -> [  ] *use DirectWrite*)
![direct write off](https://i.ibb.co/8MhC3P9/github-Direct-Write-off.png)

Primarily because DirectWrite doesn't let the theme use the above mentioned hardcoded font faces for some weird reason. Hopefully this will be fixed in a future version of Notepad++, then I'll probably publish a version of this theme with *Fira Code* font, which has ligatures, like →, ⇒, ≥, etc.

# Setting up Markdown

In the downloaded zip there is a Markdown directory. Copy `markdown.tangara.udl.xml` to `%AppData%\Notepad++\userDefineLangs`

By default, if you open a Markdown file in NPP, the colors may be messed up, because another Markdown UDL is arbitrarily used instead of `Markdown (Tangara)`, and you have to select the correct UDL in the *Language* menu every time you open a .md file. As this practice is intolerable, it's worth putting a little work into avoiding it:

Open **all** Markdown UDLs in the `userDefineLangs` directory for editing, **except** `markdown.tangara.udl.xml`. There you can see the following code:

```
<NotepadPlus>
    <UserLang name="Markdown (Theme Name)" ext="md markdown" udlVersion="2.1">
```

Replace `ext="md markdown"` to `ext=""` in all opened documents.

This way the Tangara UDL will be the only relevant one to be associated with Markdown.

# Author / contact

Laci Bene · laci.bene![|](https://i.ibb.co/7WLcqb3/ch1.gif)mail![|](https://i.ibb.co/R45zkLX/ch2.gif)ee
