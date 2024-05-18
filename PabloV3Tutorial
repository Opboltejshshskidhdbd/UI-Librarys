# PabloLibV3Tutorial
<[[UPDATE LOGS]]>
------------------------------
1. And finally... I added dropdown! Huge thanks to WhiteHat | AnyaDev to making it
-------------------------
Hello! In this tutorial I will show how to use the "Pablo Lib V3"!

Let's start!

### 1. To create the lib use this code:
```lua
local PabloLib = loadstring(game:HttpGet("https://raw.githubusercontent.com/BatuKvi123/PabloLibV3/main/PabloLibV3"))()
```

###  2. To get the lib use this code:
```lua
local window = PabloLib:Create(
"Name", -- Name here.
"Enabled", -- If you want draggable set here to "Enabled" if you dont want set to "Disabled".
"p" -- You can put any keybind here to open close.
)
```

### 3 . To create a tab use this following code:
```lua
local tab1 = window:CreateTab("Tab1")
```
### 4. To create a button use this following code:
```lua
tab1:CreateButton("Button", function()
print("Hello World")
end)
```

### 5. To create a toggle use this following code:
```lua
tab1:CreateToggle("Toggle", function(state)
if state then
print("Enabled!")
else
print("Disabled!")
end)
```

### 6. To create a slider use this following code:
```lua
tab1:CreateSlider("Slider", 0, 100, function(arg)
print(arg)
end)
```

### 7. To create a textbox use this following code:
```lua
tab1:CreateTextbox("Textbox", function(a)
print(a)
end)
```

### 8. To create a label use this following code:
```lua
tab1:CreateLabel("Label")
```

### 9. To create an Info use this following code:
```lua
tab1:CreateInfo("Info")
```

### 10. To create an Warning use this following code:
```lua
tab1:CreateWarning("Warning")
```

### 11. To create an Dropdown use this following code:
```lua
tab1:CreateDropdown("Dropdown", {"Option 1", "Option 2", "Option 3"}, function(selected)
print(selected)
end
```

### OR

# Want to make it like every option has a script? Well.. Theres a way! Just use this following code:
```lua
getgenv().selected = nil

function DetectOption()
if getgenv().selected == "Option 1" then
print("Setting walkspeed to 100!")
game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 100
elseif getgenv().selected == "Option 2" then
print("Setting jumppower to 100!")
game.Players.LocalPlayer.Character.Humanoid.JumpPower = 100
elseif getgenv().selected == "Option 3" then
print("Resetting!")
game.Players.LocalPlayer.Character.Humanoid.Health = 0
end
end)

tab1:CreateDropdown("Dropdown", {"Option 1", "Option 2", "Option 3"}, function(selectedopt)
getgenv.selected = selectedopt
DetectOption()
end
```


# EXTRAS
### Extra 1. Deleting an any tab element(button, slider, textbox, Toggle, label, info, warning)
```lua
local button = tab1:CreateButton("Print hi", function()
print("hi")
end)

tab1:CreateButton("Delete print hi button", function()
button:Delete()
end)
```
### NOTE: THIS IS NOT ONLY WORKS ON BUTTON THIS IS WORKING ON BUTTON, TOGGLE, SLIDER, TEXTBOX, LABEL, INFO, WARNING!

### Extra 2. Deleting a Tab
```lua
local tab1 = window:CreateTab("Tab")
tab1:CreateButton("Destroy this tab", function()
tab1:DeleteTab()
end)
```

### NOTE: THIS IS WORKS ON ANY TAB!

### Extra 3. Closing the Pablo Lib
```lua
PabloLib:Close()
```
# READY SCRIPTS
### 1. Making a key system
```lua
local PabloLib = loadstring(game:HttpGet("https://raw.githubusercontent.com/BatuKvi123/PabloLibV3/main/PabloLibV3"))()
local key = "PabloLibKey" -- Put your key here.
local window = PabloLib:Create(
"Key System",
"Enabled"
"p"
)

local tab1 = window:CreateTab("Key System")
tab1:CreateWarning("Please put key to contiune.")
tab1:CreateTextbox("Put key here:", function(a)
if a == key then
-- Put your code here what happens after you entered the correct key.
window:CreateTab("TestTab")
else
local warning = tab1:CreateWarning("Wrong key! Please try again.") -- If the key is wrong it will creates a warning says "Wrong Key! Please try again." after 2 seconds it deletes. 
wait(2)
warning:Delete() 
end
end)
```
Thats all for now! I hope yall like the new updates and new ui!
Have a good day! :)
