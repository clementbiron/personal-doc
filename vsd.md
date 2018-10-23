**Tutos**

- Make Visual Studio Code Your Editor https://scotch.io/courses/make-visual-studio-code-your-editor
- Visual Studio Code for PHP Developers : https://laracasts.com/series/visual-studio-code-for-php-developers
- All the best things about Visual Studio Code that nobody ever bothered to tell you : https://vscodecandothat.com/

**Extensions**

- Alignemment de code : Better Align (wwm.better-align)
- Sass intellisence (auto complétion / refacto) : SCSS IntelliSense (mrmlnc.vscode-scss)
- Plusieurs terminaux sous Windows avec Shell Launcher https://marketplace.visualstudio.com/items?itemName=Tyriar.shell-launcher
User settings :
```
 "shellLauncher.shells.windows": [
        {
            "shell": "C:\\WINDOWS\\system32\\cmd.exe",
            "label": "cmd"
        },
        {
            "shell": "C:\\Windows\\SysWOW64\\WindowsPowerShell\\v1.0\\powershell.exe",
            "label": "PowerShell"
        },
        {
            "shell": "C:\\Program Files\\Git\\bin\\bash.exe",
            "label": "Git bash"
        },

    ]
 ```
 Key binding
 ```
 {
    "key": "ctrl+shift+t",
    "command": "shellLauncher.launch"
}
```

**Shortcuts**

- `ctrl + shift + =` align assignement (avec l'extension Better Align) 
- `ctrl + d` selects next occurrence of word under cursor or of the current selection
