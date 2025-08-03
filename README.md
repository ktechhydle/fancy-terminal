# `fancy-terminal`

```
glang install fancy-terminal
```

**Colorize the terminal - in GLang!**

```
fetch fancy_terminal;

bark(GREEN + "All systems running" + RESET);
```

## Usage

Create any string, then add your colors, backgrounds, or effects!

```
obj my_string = "Hello in red";

bark(RED + my_string + RESET);

# can be used in chain
bark(BOLD + ITALIC + "This is important" + RESET);
```

## Supported Styles

| **Name**               | **Escape Code** | **Description**                               |
|------------------------|------------------|-----------------------------------------------|
| RESET                  | `\e[0m`          | Reset all styles                              |
|                        |                  |                                               |
| **Bold**               |                  |                                               |
| BOLD                   | `\e[1m`          | Make text bold                                |
| NO_BOLD                | `\e[21m`         | Disable bold                                  |
|                        |                  |                                               |
| **Dim**                |                  |                                               |
| DIM                    | `\e[2m`          | Make text dim                                 |
| NO_DIM                 | `\e[22m`         | Disable dim                                   |
|                        |                  |                                               |
| **Italic**             |                  |                                               |
| ITALIC                 | `\e[3m`          | Make text italic                              |
| NO_ITALIC              | `\e[23m`         | Disable italic                                |
|                        |                  |                                               |
| **Underline**          |                  |                                               |
| UNDERLINE              | `\e[4m`          | Underline text                                |
| NO_UNDERLINE           | `\e[24m`         | Remove underline                              |
|                        |                  |                                               |
| **Blink**              |                  |                                               |
| BLINK                  | `\e[5m`          | Make text blink                               |
| NO_BLINK               | `\e[25m`         | Disable blinking                              |
|                        |                  |                                               |
| **Reverse**            |                  |                                               |
| REVERSE                | `\e[7m`          | Swap foreground and background                |
| NO_REVERSE             | `\e[27m`         | Disable reverse                               |
|                        |                  |                                               |
| **Hide**               |                  |                                               |
| HIDE                   | `\e[8m`          | Make text invisible                           |
| NO_HIDE                | `\e[28m`         | Make text visible                             |
|                        |                  |                                               |
| **Strikethrough**      |                  |                                               |
| STRIKETHROUGH          | `\e[9m`          | Cross out text                                |
| NO_STRIKETHROUGH       | `\e[29m`         | Remove strikethrough                          |
|                        |                  |                                               |
| **Text Colors (Bright)**|                 |                                               |
| BLACK                  | `\e[90m`         | Bright black text                             |
| RED                    | `\e[91m`         | Bright red text                               |
| GREEN                  | `\e[92m`         | Bright green text                             |
| YELLOW                 | `\e[93m`         | Bright yellow text                            |
| BLUE                   | `\e[94m`         | Bright blue text                              |
| MAGENTA                | `\e[95m`         | Bright magenta text                           |
| CYAN                   | `\e[96m`         | Bright cyan text                              |
| WHITE                  | `\e[97m`         | Bright white text                             |
| DEFAULT                | `\e[99m`         | Default text color                            |
|                        |                  |                                               |
| **Text Colors (Dim)**  |                  |                                               |
| DIM_BLACK              | `\e[30m`         | Dim black text                                |
| DIM_RED                | `\e[31m`         | Dim red text                                  |
| DIM_GREEN              | `\e[32m`         | Dim green text                                |
| DIM_YELLOW             | `\e[33m`         | Dim yellow text                               |
| DIM_BLUE               | `\e[34m`         | Dim blue text                                 |
| DIM_MAGENTA            | `\e[35m`         | Dim magenta text                              |
| DIM_CYAN               | `\e[36m`         | Dim cyan text                                 |
| DIM_WHITE              | `\e[37m`         | Dim white text                                |
| DIM_DEFAULT            | `\e[39m`         | Default dim text color                        |
|                        |                  |                                               |
| **Backgrounds (Bright)**|                 |                                               |
| BG_BLACK               | `\e[100m`        | Bright black background                       |
| BG_RED                 | `\e[101m`        | Bright red background                         |
| BG_GREEN               | `\e[102m`        | Bright green background                       |
| BG_YELLOW              | `\e[103m`        | Bright yellow background                      |
| BG_BLUE                | `\e[104m`        | Bright blue background                        |
| BG_MAGENTA             | `\e[105m`        | Bright magenta background                     |
| BG_CYAN                | `\e[106m`        | Bright cyan background                        |
| BG_WHITE               | `\e[107m`        | Bright white background                       |
| BG_DEFAULT             | `\e[109m`        | Default background color                      |
|                        |                  |                                               |
| **Backgrounds (Dim)**  |                  |                                               |
| BG_DIM_BLACK           | `\e[40m`         | Dim black background                          |
| BG_DIM_RED             | `\e[41m`         | Dim red background                            |
| BG_DIM_GREEN           | `\e[42m`         | Dim green background                          |
| BG_DIM_YELLOW          | `\e[43m`         | Dim yellow background                         |
| BG_DIM_BLUE            | `\e[44m`         | Dim blue background                           |
| BG_DIM_MAGENTA         | `\e[45m`         | Dim magenta background                        |
| BG_DIM_CYAN            | `\e[46m`         | Dim cyan background                           |
| BG_DIM_WHITE           | `\e[47m`         | Dim white background                          |
| BG_DIM_DEFAULT         | `\e[49m`         | Default dim background                        |
