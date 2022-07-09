<h1 align="center" style="font-family: Roboto">
CHROME DEV TOOLS CHEAT SHEET
</h1>


### Opening Devtools

To access the DevTools, on any web page or app in Google Chrome you can use one of these options:

- Open the **Chrome menu** at the top-right of your browser window, then select `Tools > Developer Tools`.
- Right-click on any page element and select **Inspect Element**.

|                                                            | Windows / Linux           |
|------------------------------------------------------------|---------------------------|
| Open Developer Tools                                       | `F12`, `Ctrl + Shift + I` |  
| Open / switch from inspect element mode and browser window | `Ctrl + Shift + C`        |  
| Open Developer Tools and bring focus to the console        | `Ctrl + Shift + J`        |  
| Inspect the Inspector (undock first one and press)         | `Ctrl + Shift + J`        |  

### All Panels

|                                                      | Windows / Linux               | Mac                |
|------------------------------------------------------|-------------------------------|--------------------|
| Show General Settings dialog                         | `?, F1`                       | `?`                |
| Next panel                                           | `Ctrl + ]`                    | `Cmd + `]          |
| Previous panel                                       | `Ctrl + [`                    | `Cmd + [`          |
| Backward in panel History                            | `Ctrl + Alt + [`              | `Cmd + Alt + [`    |
| Forward in panel history                             | `Ctrl + Alt + ]`              | `Cmd + Alt + ]`    |
| Jump to panel 1-9 (when enabled in General Settings) | `Ctrl + 1-9`                  | `Cmd + 1-9`        |
| Toggle Console / close settings dialog when open     | `Esc`                         | `Esc`              |
| Refresh the page                                     | `F5, Ctrl + R`                | `Cmd + R`          |
| Refresh the page ignoring cached content             | `Ctrl + F5, Ctrl + Shift + R` | `Cmd + Shift + R`  |
| Text search within current file or panel             | `Ctrl + F`                    | `Cmd + F`          |
| Text search across all sources                       | `Ctrl + Shift + F`            | `Cmd + Alt + F`    |
| Search by filename (except on Timeline)              | `Ctrl + O, Ctrl + O`          | `Cmd + O, Cmd + O` |
| Restore default text size                            | `Ctrl + 0`                    | `Shift + 0`        |
| Zoom in                                              | `Ctrl + + `                   | `Shift + +`        |
| Zoom out                                             | `Ctrl + - `                   | `Shift + -`        |

### Elements Panel

|                        | Windows / Linux                    | Mac                                |
|------------------------|------------------------------------|------------------------------------|
| Undo change            | `Ctrl + Z`                         | `Cmd + Z`                          |
| Redo change            | `Ctrl + Y`                         | `Cmd + Y, Cmd + Shift + Z`         |
| Navigate               | `Up, Down`                         | `Up, Down`                         |
| Expand / collapse node | `Right, Left`                      | `Right, Left`                      |
| Expand node            | `Single-click on tag`              | `Single-click on tag`              |
| Edit attribute         | `Enter, Double-click on attribute` | `Enter, Double-click on attribute` |
| Hide element           | `H`                                | `H`                                |
| Toggle edit as HTML    | `F2`                               |                                    |

Right-clicking an element you can: 

- Force element psuedo states: (`:active`, `:hover`, `:focus`, `:visited`)
- Set breakpoints on the elements: (Subtree modifications, Attribute modification, Node removal)
- Clear console

### Styles Sidebar

|                                                         | Windows / Linux                     | Mac                                 |
|---------------------------------------------------------|-------------------------------------|-------------------------------------|
| Edit rule                                               | `Single-click`                      | `Single-click`                      |
| Insert new property                                     | `Single-click on whitespace`        | `Single-click on whitespace`        |
| Go to line of style rule property declaration in source | `Ctrl + Click on property`          | `Cmd + Click on property`           |
| Go to line of property value declaration in source      | `Ctrl + Click on property value`    | `Cmd + Click on property value`     |
| Go to line of style rule property declaration in source | `Ctrl + Click on property`          | `Cmd + Click on property`           |
| Go to line of property value declaration in source      | `Ctrl + Click on property value`    | `Cmd + Click on property value`     |
| Cycle through the color definition value                | `Shift + Click on color picker box` | `Shift + Click on color picker box` |
| View auto-complete suggestions                          | `Ctrl + Space`                      | `Cmd + Space`                       |
| Edit next / previous property                           | `Tab, Shift + Tab`                  | `Tab, Shift + Tab`                  |
| Increment / decrement value                             | `Up, Down`                          | `Up, Down`                          |
| Increment / decrement value by 10                       | `Shift + Up, Shift + Down`          | `Shift + Up, Shift + Down`          |
| Increment / decrement value by 10                       | `PgUp, PgDown`                      | `PgUp, PgDown`                      |
| Increment / decrement value by 100                      | `Shift + PgUp, Shift + PgDown`      | `Shift + PgUp, Shift + PgDown`      |
| Increment / decrement value by 0.1                      | `Alt + Up, Alt + Down`              | `Opt + Up, Opt + Down`              |

Emulate an element's pseudo state (`:active`, `:hover`, `:focus`, `:visited`)

Add new style selectors

### Sources Panel

|                                     | Windows / Linux                                | Mac                                           |
|-------------------------------------|------------------------------------------------|-----------------------------------------------|
| Pause / resume script execution     | `F8, Ctrl + \`                                 | `F8, Cmd + \`                                 |
| Step over next function call        | `F10, Ctrl + '`                                | `F10, Cmd + '`                                |
| Step into next function call        | `F11, Ctrl + ;`                                | `F11, Cmd + ;`                                |
| Step out of current function        | `Shift + F11, Ctrl + Shift + ;`                | `Shift + F11, Cmd + Shift + ;`                |
| Select next call frame              | `Ctrl + .`                                     | `Opt + .`                                     |
| Select previous call frame          | `Ctrl + ,`                                     | `Opt + ,`                                     |
| Toggle breakpoint condition         | `Click on line number, Ctrl + B`               | `Click on line number, Cmd + B `              |
| Edit breakpoint condition           | `Right-click on line number`                   | `Right-click on line number  `                |
| Delete text on current line         | `Ctrl + D `                                    | `Cmd + D `                                    |
| Delete individual words             | `Alt + Delete`                                 | `Opt + Delete`                                |
| Comment a line or selected text     | `Ctrl + /`                                     | `Cmd + / `                                    |
| Save changes to local modifications | `Ctrl + S`                                     | `Cmd + S  `                                   |
| Go to line                          | `Ctrl + G `                                    | `Ctrl + G`                                    |
| Search by filename                  | `Ctrl + O`                                     | `Cmd + O  `                                   |
| Jump to line number                 | `Ctrl + P + :&lt;number&gt;`                   | `Cmd + P + :&lt;number&gt;`                   |
| Jump to column                      | `Ctrl + O + :&lt;number&gt; + :&lt;number&gt;` | `Cmd + O + :&lt;number&gt; + :&lt;number&gt;` |
| Go to member                        | `Ctrl + Shift + O`                             | `Cmd + Shift + O `                            |
| Toggle console                      | `Ctrl + Shift + E `                            | `Cmd + Shift + E   `                          |
| Run snippet                         | `Ctrl + Enter`                                 | `Cmd + Enter`                                 |
| Toggle comment                      | `Ctrl + /`                                     | `Cmd + /`                                     |

### Timeline Panel

|                        | Windows / Linux | Mac       |
|------------------------|-----------------|-----------|
| Start / stop recording | `Ctrl + E`      | `Cmd + E` |
| Save timeline data     | `Ctrl + S`      | `Cmd + S` |
| Load timeline data     | `Ctrl + O`      | `Cmd + O` |

### Search Shortcuts

Find or navigate to specific files, methods or line numbers in an web app within the Sources panel.

|                                                                       | Windows / Linux    | Mac             |
|-----------------------------------------------------------------------|--------------------|-----------------|
| Search scripts, stylesheets and snippets by filename                  | `Ctrl + O`         | `⌘ + O`         |
| Text search within current file                                       | `Ctrl + F`         | `⌘ + F`         |
| Text search across all sources                                        | `Ctrl + Shift + F  | `⌘ + Alt + F`   |
| Filter/navigate to a JavaScript function/CSS rule when viewing a file | `Ctrl + Shift + O` | `⌘ + SHift + O` |
| Launch line number dialog when viewing a file                         | `Ctrl + K`         | `⌘ + L`         |
| Evaluate code selected in scripts in the console                      | `Ctrl + Shift + E` | `⌘ + Shift + E` |

### Console

|                         | Windows / Linux | Mac                |
|-------------------------|-----------------|--------------------|
| Next suggestion         | `Tab`           | `Tab`              |
| Previous suggestion     | `Shift + Tab`   | `Shift + Tab`      |
| Accept suggestion       | `Right`         | `Right`            |
| Previous command / line | `Up`            | `Up`               |
| Next command / line     | `Down`          | `Down`             |
| Clear Console           | `Ctrl + L`      | `Cmd + K, Opt + L` |
| Multi-line entry        | `Shift + Enter` | `Ctrl + Return`    |
| Execute                 | `Enter`         | `Return`           |

Right-clicking on console:

- XMLHTTPRequest logging: Turn on to view the XHR log
- Preserve log upon navigation
- Filter: Hide and unhide messages from script files
- Clear console: Clear all console messages

