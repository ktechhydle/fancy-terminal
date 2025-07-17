```
glang install fancy-terminal
```

# `fancy-terminal`
Colorize the terminal - in GLang!

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
