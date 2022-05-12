# Notes on using these fonts

## Notes on fonts in crostini.

### Get and install font

1. Download the font, e.g. from https://rubjo.github.io/victor-mono/VictorMonoAll.zip.
2. Copy the OTF files to ~/.fonts
3. run `fc-cache -fv` ("force and verbose")

### Update font for terminal

1. Create fork of https://github.com/rubjo/victor-mono to use the css and fonts
  without silent interference.
2. Create github page at https://dan9323.github.io/victor-mono/ to host css.
3. From https://github.com/wernight/powerline-web-fonts
  Open crostini terminal. Press Ctrl+Shift+J and then enter

    ```
    term_.prefs_.set('user-css', 'https://dan9323.github.io/victor-mono/dist/index.css');
    term_.prefs_.set('font-family', '"Victor Mono", monospace');
    ```

## Notes on vscode under crostini

1. Go to settings. I'm using the font

    `'Victor Mono', 'Droid Sans Mono', 'monospace', monospace`
    
2. Search for "ligature", and change the json with

    `"editor.fontLigatures": true`
