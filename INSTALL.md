### [Windows Terminal](https://learn.microsoft.com/en-us/windows/terminal/)

#### Download

Download using the [GitHub .zip download](https://github.com/scottgriv/Dark-Castle-Windows-Terminal/archive/master.zip) option.

#### Install

Start Windows Terminal and click on the down arrow symbol `˅` from menu bar. This will open a drop down menu from which select Settings option. Alternatively use `Ctrl + ,` to open Settings directly.

On the bottom left hand side of the Settings window, select `Open JSON File`.

In the `settings.json` settings file for Windows Terminal, find the `schemes` section and paste the content of `copy.json`.

Example:

```json
"schemes": [
  {
    "name": "Dark Castle",
    "cursorColor": "#FF8040",
    "selectionBackground": "#292929",
    "background": "#000000",
    "foreground": "#FFD580",
    "black": "#1A1A1A",
    "blue": "#2D449B",
    "cyan": "#007B88",
    "green": "#08D220",
    "purple": "#AA1B86",
    "red": "#FF000F",
    "white": "#9C9C9C",
    "yellow": "#DFC200",
    "brightBlack": "#292929",
    "brightBlue": "#4164FF",
    "brightCyan": "#4DBCED",
    "brightGreen": "#BAE67E",
    "brightPurple": "#9354FF",
    "brightRed": "#EF6B73",
    "brightWhite": "#FFFFFF",
    "brightYellow": "#FFD580"
  }
]
```

#### Activate

Once the color scheme has been defined, it's time to enable it. Find the `profiles` section and add a `colorScheme` value to the default profile.

Example:

```json
"profiles": {
    "defaults": {
        "colorScheme" : "Dark Castle"
    }
}
```

If the profiles are listed as below:

```jsonc
"profiles": [
    // list of profiles
]
```

Change it to:

```jsonc
"profiles": {
    "defaults": {
      "colorScheme": "Dark Castle"
    },
    "list": [
      // list of profiles
    ]
  },
```

You can also set your color scheme by clicking `Color Schemes` in the navigation menu on the left hand side and then select `Dark Castle`. Scroll down and click `Set as default`.

Once `Dark Castle` is set to your default `Color Scheme`, it will be available in `Command Prompt`, `PowerShell`, `bash`, etc.