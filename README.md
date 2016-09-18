# Insert Time Stamp

## Features

Quick insertion of linux-like time stamp into Visual Studio Code editor.

## Example
```
###### Sun Sep 18 15:29:29 IDT 2016
```

Here is how it looks after markdown processing:
###### Sun Sep 18 15:29:29 IDT 2016

## Configure shortcuts
Default shortcut is `ctrl + f5`  

in your `Code/User/keybindings.json` file add the following:
```
{
    "key": "ctrl+f5", // specify shortcut you like here
    "command": "inserttimestamp.perform",
    "when": "editorTextFocus"
}
```

## Format
Currently supported timestamp format: `###### Www Mmm dd h:mm:ss Tz yyyy`  

where:  
    `######` — prefix (as is: "######")  
    `Www` — week day name (3 letters)  
    `Mmm` — month name (3 letters)  
    `dd` — day in month  
    `h` — hours (24h format)  
    `mm` — minutes  
    `ss` — seconds  
    `Tz` — Time zone abbreviation (3 letters, I am not sure if it is true for any time zone)   
    `yyyy` — year (4 digits)

## License
Extension licensed under [MIT](./LICENSE)

## Thanks
To [Nick Roach](https://www.elegantthemes.com/) for the great icon.

## Author
Vlad Zamskoi  
Site: [freeraven.com](https://www.freeraven.com/ "Developer website")