# keyboard module

#### installation
```pip install keyboard```

#### usage
```import keyboard```\
```import keyboard as kb``` if you want to use short library name

#### commands example
Check if 'q' button is pressed
```keyboard.is_pressed('q')```\
Wait until 'p' is pressed than process the rest of the code\
`keyboard.wait("p")`\
`print("You pressed p")`
Run function on specific key pressed
```keyboard.on_press_key("p", function_name())```\
Stop all the "hooks" from working
```keyboard.unhook_all()```

---
_Last update: 23 Feb 2023_ 