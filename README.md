![IMG_20241009_134537](https://github.com/user-attachments/assets/2e1aa59f-633e-4d55-a696-e9930a093022)

A phone-focused theme for Obsidian

[Screenshots](#screenshots) | 
[Features](#features) | [Snippets](#Snippets) | [What's new](#changelog) | [Fonts](#fonts) | [Support me](#contribution)


[Lagom](https://en.wikipedia.org/wiki/Lagom) tries to focus on just the right amount of changes needed to make it look aesthetically more conventional and modern. It's not about reinventing the wheel or offering a unique or special theme. I simply think Obsidian is a diamond in the rough that needs to be polished to shine on its own.✨ 

**The theme attempts to follow the following principles:**

1. Avoid as much as possible an extreme minimalism that prevents me from recognizing what is and what is not in the UI.
  

2. Make subtle changes that are noticeable and make a difference both aesthetically and functionally but do not prove to be a distraction when using Obsidian.
   
3. Symmetry and visual consistency.
   
4. Focused exclusively for use on phones or tablets.
  
5. Do not follow a specific color palette or typeface (so you can use it with the one you prefer!) 

6. [Complementary and modular](Comparison)

*Work in progress...*

# Screenshots
![IMG_20241214_172439](https://github.com/user-attachments/assets/c828899f-c2e6-43ec-948f-b7cea6e612d7)

![IMG_20241009_142625](https://github.com/user-attachments/assets/622c6872-f15f-4129-81f8-cac6e4f6a03d)
![IMG_20241009_142756](https://github.com/user-attachments/assets/b83784ae-0f98-4709-8b40-ef25ff979c36)
![IMG_20241009_142848](https://github.com/user-attachments/assets/7e8465cf-e6a5-4cca-a0ca-59c3d2b318ed)
![IMG_20241009_142919](https://github.com/user-attachments/assets/cfc7eec7-4e88-4589-b1ec-cc9d29cac693)

# Fonts

**Main font:** Akrobat Semibold or Pragati Regular but *Interphases Pro Condensed Regular* It is more pleasant and perhaps more suitable for reading.

**Headers:** Play fair display 

**Mono:** Losevka Regular. 

**Code:** Jetbrains

**Quotes:** Caecelia 

[Download snippet](https://github.com/LeslyeCream/Lagom-Obsidian-Theme/blob/main/Fonts.css)

# Features

- The file panel occupies 100% of the screen to take advantage of the available space (optional pop-up style)

  ![Screenshot_20241022-092322](https://github.com/user-attachments/assets/34297bcd-458b-477d-97ea-c42d90a5404f)


- Files show their full name on multiple lines. No more unfinished titles or ellipses!

![IMG_20241010_165149](https://github.com/user-attachments/assets/6269362e-9edc-4973-bfe0-bb7808d1e7b8)


- Nested folders with a subtle open-folder indicator

  ![IMG_20241010_162206](https://github.com/user-attachments/assets/2ac5c144-f451-44ce-a2f0-c52c70850f04)


- Editor dims blocks of text that is not in focus (and slightly increases the font size of text in focus) 

- Separator inspired by the book *A Psalm for the Wild-Built*

![IMG_20241010_165116](https://github.com/user-attachments/assets/3bb1ae60-0999-417d-8014-5766fee9c06b)

  
- Code blocks more similar in appearance to a MacOS terminal (colorful for dark mode and monochromatic for light mode)

![IMG_20241014_091844](https://github.com/user-attachments/assets/7637aa52-3ff6-41c7-95d0-be6332659164)

- Quotes with classic style

![Screenshot_20241205-163738_cropped](https://github.com/user-attachments/assets/c4224921-b5a2-469d-be93-6e0169d496ac)

- Touching the right side of the header will collapse or expand their contents
![IMG_20250525_080615](https://github.com/user-attachments/assets/893aecea-094b-4c1c-bffe-c954ccba0590)

- Embedded notes have been slightly redesigned
![IMG_20250514_091523](https://github.com/user-attachments/assets/d29696ba-ad6d-47d2-b051-45745d62924e)

- Translucent navigation bar (optional)
![IMG_20250517_183412](https://github.com/user-attachments/assets/d2398cdc-8ccd-440e-aef8-9db6a2c8b6db)


# Note

It is recommended to use *Commander*, *Iconize*, *Custom file explorer sorting* and *File explorer note count* with this theme for a complete experience.

# Snippets 

To use the file name at the vault root to categorize a group of folders it is necessary to use a snippet:

```css
.nav-file-title[data-path*=".md"]:before {
	content: "";
}

.nav-file-title:not([data-path*="/"]) {
  margin: 0px;
  padding: 0px;
  left: 25px;
  font-size: calc(var(--default-font-size) + 1.2px);
  color: var(--text-accent);
  font-weight: 500 !important;
}
```
The following snippet can be pasted directly into the style settings to achieve the Lagom look as shown in the screenshots.

```json
{
  "files-folders@@nav-item-size": 15.4,
  "notes-values@@default-font-size": 15.4,
  "notes-values@@letter-spacing-note": -0.18,
  "notes-values@@line-height-note": 21,
  "others-values@@theme-dark-opacity": 0.65,
  "notes-values@@inline-title-always-uppercase": false,
  "notes-values@@inline-title-size": 20,
  "notes-values@@headers-align": "left",
  "notes-values@@p-spacing": 26,
  "notes-values@@separator-icon-color": "#6C6C6C6E",
  "notes-values@@icon-link-embed-notes": "block",
  "notes-values@@quote-hide-top-line": "1.5px",
  "notes-values@@quote-hide-down-line": "1.5px",
  "yaml-values@@hide-separator-yaml": "unset",
  "notes-values@@wrap-code-blocks": "pre",
  "notes-values@@code-size": 13,
  "notes-values@@code-size-edit-mode": 14,
  "notes-values@@h1-size": 24,
  "notes-values@@h2-size": 20,
  "notes-values@@h3-size": 18,
  "notes-values@@h4-size": 16,
  "notes-values@@h5-size": 14,
  "notes-values@@h6-size": 12,
  "notes-values@@page-style-read-mode": true,
  "notes-values@@page-style-card": false,
  "notes-values@@enable-shadows-borders-img": false,
  "notes-values@@hide-embed-title": false,
  "obsidian-borealis@@syntax-highlighting": "sh3",
  "notes-values@@padding-note-content": 25,
  "others-values@@navbar_blur_level": "8px",
  "hide-elements@@scrollbars": "none",
  "hide-elements@@files-bookmarks-search-bar": "none",
  "hide-elements@@show-explorer-buttons": "none",
  "hide-elements@@show-editor-text-bar": "none",
  "hide-elements@@hide-navbar": "block",
  "hide-elements@@icon-settings": "none",
  "others-values@@nav-bar-blur": false,
  "notes-values@@active-line-indicator": "\"\"",
  "notes-values@@show-dotted-line": "0px",
  "yaml-values@@hide-add-button": "None",
  "obsidian-borealis@@enable-alternative-checkboxes": false,
  "files-folders@@popup-explorer": true,
  "files-folders@@icon-file": "•",
  "hide-elements@@show-vault-name": "none"
}
```

# Comparison 

![IMG_20241014_094621](https://github.com/user-attachments/assets/861dcc25-2a73-4ecd-a180-2b290e330adf)

*If you want to use Lagom alongside another theme (Gruvebox, Rosé Pine, Borealis, etc.), you can simply move the theme.css file into your snippets folder and activate it.*

# Roadmap

- Clean and improve the css code 
- Adapt it for the rest of the platforms 
- [x] ~~Fix some aesthetic issues~~
- [x] ~~Add options for Style Settings~~

# Special thanks

[@Bluemoondragon07](https://github.com/Bluemoondragon07/obsidian-big-and-bold) For its fantastic theme that encouraged me to choose Obsidian as my replacement to Evernote.

@ariehen In this [post](https://forum.obsidian.md/t/properties-view-css-the-fall-collection/66512) for properties in the notes 

[@death_au](https://github.com/deathau)

[AlanG](https://forum.obsidian.md/t/how-to-disable-line-wrapping-in-code-blocks/69900) for its snippet for the code blocks

@LuisaKart By the code to modify the new tab view

# Changelog

**V1.6.4**
- **Collapsible Heading Indicators:**  A visual indicator now appears in headings when their content is collapsed. This indicator has been repositioned to the right margin for improved readability and to minimize interference with text.
- **Independent Page Style Selection:**  Users can now select page styles independently for both the editor and reading modes.
- **Title Corrections:** Minor corrections have been applied to the title display within notes.
- **Interface Enhancements:** Border lines have been added to several previously missing interface elements for improved visual consistency.

**V1.6.3**
- Option to enable a translucent glass effect on the navigation bar.
- Fixed the issue with the small selector icon in dates within properties.
- Option to adjust the padding of note content.
- Some aesthetic corrections to the appearance of global search.
- Fixed several inconsistencies when hiding or showing the settings button, vault name, number of notes, etc.

**V1.6.2**
- The version number in the GitHub changelog directly becomes the same as the one shown in Obsidian to avoid confusion regarding changes
- Improvements to the navigation bar: now it takes up less screen space with a floating design
- Added an option to turn off image borders and shadows (resolves problems with transparent images)
- You can now choose between two note styles for reading mode: page style and card style (though it still conflicts if the note has embedded notes)
- 
**V1.9 (May 2025)**
- Now the macOS style buttons in the Code Blocks (Light Mode) are images instead of symbols. It is no longer necessary to modify its size in Style Settings
- The line borders of code blocks, callouts and embed notes share the same design. 
- Some other small details fixed

**V1.8**
- Small fixes in the search and replace bar  
- Option to show or hide the link icon in embedded notes(!)  
- Option to choose text alignment in the notes list within the file explorer
  
**V1.7**
- Option to change the background color of the active line
- Now the images are centered by default and occupy all the width for a better visual consistency with the rest of the content.
- New option to activate gray-scale images when dark mode is active.
- Now you can choose the underlined style in local links
- Small changes in Style Settings

**V1.6** 
- Added option to prevent changes to the Inline-Title in reading mode.
- Fixed list inconsistency caused by the latest Obsidian update.

**V1.5**
- New design for quotes
- You can now modify the padding of the quote blocks.
- Option to choose a local image or url as note background in the text editor
- Now you can always capitalize the title inside the notes.
- Extra options to customize the dividing line between notes in the file explorer (style and thickness)
- Small changes in search boxes

**V1.4**
- Fix disproportionate margin in images

- New option to change the size of headers

- Removed the option to change the font size in the active line (apparently it is not useful?) and caused display problems in editor mode.
  
- New option to change the height in the new preview of opened tabs.
  
- The note name in the tab list is displayed on multiple lines.

- It is now possible to choose the font size of YAML metadata in editor mode.

- The icon next to each file was slightly misaligned, now it is centered correctly in relation to the text height.

- Some other minor changes
  
**V1.3**

- Fixed the position of the date and labels in properties. Now it is aligned with the other values

- A tiny correction in the embedded notes (the bottom padding was too short)

- Tables show vertical separator lines inside.

- New option to separately choose font size inside code blocks in edit mode and preview mode.

- Fixed top margin of Command palette 

- Small changes in tables

# Contribution

Contribute reporting bugs, code improvements and of course, feedback is welcome! 

Please open an issue on github or send me an [email](mailto:lagom.haggler091@slmail.me). I will try to fix it as soon as possible. 

If you really like this theme, please consider support me ᵔᴥᵔ

<a href='https://ko-fi.com/W7W349H97' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://storage.ko-fi.com/cdn/kofi1.png?v=6' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
