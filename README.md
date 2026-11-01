# Bibliotheca

A first-person 3D library for Common Entrance Latin. Open `index.html` in Chrome or Edge. It needs an internet connection, because it loads Three.js from jsDelivr.

## The building

- **The Entrance Hall** (south): where you start.
- **The Rotunda**: a domed hall with Archivarius Wren, the Librarian, at the central desk. Speak to him to travel to any section, or ask where a word or piece of grammar is kept. Type a Latin word, an English word or a grammar term (*puella*, *to love*, *pluperfect*, *fero*), and he tells you where it lives and can send you there with the book open.
- **The Grammar Hall** (north): seven alcoves, one for each part of the grammar (nouns, adjectives, pronouns, verbs, irregular verbs, prepositions, key syntax), with a lectern for every table.
- **The Vocabulary Wing** (west): all the CE words, shelved by kind (nouns by declension, verbs by conjugation, and so on), by level (Level 1, 2, 3 and Scholarship), and all together in the Great Register. Each word list has level filters, a search box and a button to cover the English for self-testing.
- **The Reading Room** (east): reading tables, a fire, and the noticeboard of resources.

Scholars browse and read throughout, and whisper short Latin lines as you pass.

## Level setting

The title screen and pause menu have a **Word lists show** setting: All levels, Level 1, Level 2, Level 3 or Scholarship. Every word list opens on that level, and the browser remembers the choice.

## Controls

WASD to walk, the mouse to look, Shift to walk faster, E or a click to read and speak, Esc to pause. On a tablet, the left circle walks, drag to look, and tap USE.

The title screen and pause menu offer two looks: **Painted** (a brush-stroke filter) and **Plain** (faster). The game switches to Plain on its own if a computer struggles.

## Replacing the textures

Every surface is painted in code when the page loads. Near the top of the script in `index.html` you will find a guide listing each texture with its size and whether it tiles, and a list called `TEXTURE_FILES`. To use your own picture, put its file name next to the texture's name, for example:

```js
wallpaper: 'textures/wallpaper.png',
```

Then put the picture in that folder, next to `index.html`. Ask for "seamless" or "tileable" pictures for the textures that tile. The painted version shows until your picture loads, and stays if the file can't be found.

## The content

The words and grammar tables are a snapshot of the CE word list site (cewordlist), taken on 20 October 2026. They sit in one block near the top of `index.html` (`window.__LIB_CONTENT`).

The Scholarship words (26, from the Additional Scholarship Checklist in *Prep School Latin* by R. C. Bass, CC BY-NC-SA) and the Level 3 and Scholarship grammar tables (passive in all five tenses, participles, deponents, fio, subjunctive clauses, indirect statement, ablative absolute) were added on 1 November 2026.
