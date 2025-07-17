# fancy_terminal
Colorize the terminal - in GLang!

```
glang install fancy_terminal
```

## Usage
Create any string, then add your colors!

```
obj my_string = "Hello in red";

bark(RED + my_string + RESET);
```

Supports bold, italic, strikethrough, and underlined lettering:

```
bark(BOLD + ITALIC + UNDERLINE + "Hello, world!" + RESET);
```

You can even make lettering blink!

```
bark(BLINK + "I'm blinking!" + RESET);
```
